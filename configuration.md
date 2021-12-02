---
layout: post
title: Configuration
permalink: /configuration/
---
LABS uses JSONs to read a configuration. A configuration consists of a variety of annotation classes with different fields which are described below. Note that some classes may be different from the figure in the paper as LABS has been updated. The implementation of all the annotations for LABS can be found in /src/main/scala/labs/passes/Annotations.scala.

### ClockAnnotation and ResetAnnotation
As a FIRRTL design generated from Yosys may not be fully compatible with the FIRRTL compiler especially due t clock and reset ports, ClockAnnotation and ResetAnnotation are used to help.

```code5
  {
    "class":"labs.passes.ClockAnnotation",
    "target":"None.None.<clock_name>"
  }
```

ClockAnnotation has one field which requires the user to indicate the clock name of the entire design. LABS converts <clock\_name> to "clock" and makes the signal compatible with FIRRTL internal representation requirements.

```code6
  {
    "class":"labs.passes.ResetAnnotation",
    "target":"None.None.<reset_name>",
    "posedge_reset": <0/1>
  }
```

ResetAnnotation has two fields. The "target" field requires the user to indicate the reset name of the entire design. Similar to ClockAnnotation, in this example, LABS converts <reset\_name> to "reset" and makes the signal compatible with FIRRTL internal representation requirements. The "posedge\_reset" field is used to indicate whether the given design uses positive or negetive edge reset. All of the generated modules will have the same reset logic based on this.

### FaultInjectionAnnotation and ScanChainAnnotation
These two annotations are from a fault injection framework, [https://github.com/IBM/chiffre](Chiffre), that LABS relies on, which are used to integrate fault controllers and fault injectors.

```code7
  {
    "class":"chiffre.passes.FaultInjectionAnnotation",
    "target":"<circuit_name>.<module_name>.<component_name>",
    "id":"main",
    "injector":"chiffre.inject.<injector_name>"
  }
```

FaultInjectionAnnotation is used to indicate the target component that will be attacked. The "target" field indicates the target component, and the "injector" field indicates the fault injector to be used.

```code8
  {
    "class":"chiffre.passes.ScanChainAnnotation",
    "target":"aes.FaultController.scan",
    "ctrl":"master",
    "dir":"scan",
    "id":"main"
  }
```

### FaultControllerAnnotation
FaultControllerAnnotation has 2 types, FaultControllerUDAnnotation and FaultControllerProbAnnotation, which are read to configure a fault controller. The former is used when using user-defined faults, and the latter is used when using random or probabilistic faults.

```code9
  {
    "class":"labs.passes.FaultControllerUDAnnotation",
    "target":["<circuit_name>.<module_name>.<component_name>", "<circuit_name>.<module_name>.<component_name>"],
    "data_target":["h_<value>", "h_<value>"],
    "affected_bits": [[0], [1], [2], [<indices_to_be_injected>]],
    "durations": [1, 1, 1, <duration_in_cycle>]
  }
```

FaultControllerUDAnnotation consists of 4 fields. The "target" field is used to indicate the signals to be observed by the fault controller. The "data\_target" field indicates the condition of each target signal. The fault controller sends a signal to a fault injector when all of the signals in the "target" field equal to its associated value (in hex) in the "data\_target" field. The "affected\_bits" specifies the indices of faults to be injected to the component indicated in FaultInjectionAnnotation, and the "durations" indicates how long each injection takes in cycles. In this case, the fault injector can fire at most 3 times when the conditions are met. The first fault is injected to the bit index 0, second fault to index 1 and third fault to index 2 with 1 cycle duration.

TODO Explain FaultControllerProbAnnotation

### FaultTolerantAnnotation
FaultTolerantAnnotation consists of 3 types, FaultTolerantDMRAnnotation, FaultTolerantTMRAnnotation and FaultTolerantTemporalAnnotation, to integrate DMR, TMR and temporal redundancy, respectively.

```code10
  {
    "class":"labs.passes.FaultTolerant<DMR/TMR>Annotation",
    "target":"<circuit_name>.<module_name>.<component_name>",
    "feedback_target":[<target_port>],
    "feedback":<0/1/2>
  }
```

To integrate DMR or TMR, 3 fields are needed. The "target" field indicates the target location that will be protected. The <component\_name> can be a component name or "None". If "None" is found, the entire <module\_name> will be protected. The "feedback\_target" field is used to indicate the ports that need a feedback mechanism. The "feedback" field indicates the feedback mechanism to be used. Currently, there are 3 feedback mechanisms, 0 no feedback mechanism, 1 static feedback mechanism and 2 random feedback mechanism.

TODO Explain FaultTolerantTemporalAnnotation

<link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
