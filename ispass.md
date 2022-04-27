---
layout: page
title: Hardware Security Tutorial in ISPASS-2022
permalink: /ispass2022/
---

The 2022 IEEE International Symposium on Performance Analysis of Systems and Software (ISPASS-2022), which will be hosting at the National University of Singapore in Singapore on 22-24 May 2022, will be organizing a hardware security tutorial session on 22 May. The authors are looking forward to sharing the works and having an in-person discussion during the tutorial session. The list below shows the topics that will be discussed in the tutorial session.

- Laser Attack Benchmark Suite (LABS)
- Efficient Security Protocol Realization for Secure Processors

### Laser Attack Benchmark Suite (LABS)
Laser fault injection is one of the most dangerous techniques for fault injection as laser shots can be fired at the precise location and at the right time.

Security evaluation against laser attacks requires costly, sophisticated equipment, and is typically evaluated during the post fabrication stage, which occurs too late. If a vulnerability is found during this stage, the circuit designers inevitably have to restart the entire time-consuming design stages. It is therefore impractical to evaluate chips solely during this stage.

Laser attack benchmark suite (LABS) is proposed to overcome these limitations. LABS is a framework that allows circuit designers to evaluate their designs and protections at early RTL stage or on an FPGA against laser attacks without manual modifications. It supports both processors and accelerators, and covers various widely used applications. From the potential use-case scenarios attacking a processor and accelerator, simulation of the attacks supported by LABS only takes minutes to finish.

LABS also consists of automatic hardware-based redundancy integration, supporting a variety of techniques, that helps protect the design against laser attacks. When a vulnerability is found from the attacks, it can automatically integrate redundancy techniques to a specific part of the design based on the user’s configuration. 

LABS is an open-source modular framework open for extensions. The users can easily add more features, for instance, attacks and defenses to LABS to meet their needs. The attacks and defenses together that LABS provides will automate the entire pre-silicon security evaluation flow against laser fault injection attacks.

During this tutorial, the background on general and laser fault injection attacks is described, comprehensive comparisons between different approaches are elaborated, as well as LABS is presented and demonstrated. 

### Efficient Security Protocol Realization for Secure Processors
Modern microprocessors present various layers of trusted computing, based on a fundamental root-of-trust. The root-of-trust is typically implemented through a lightweight crypto co-processor. Despite the best efforts, the currently available commercial processors with trusted computing support - face continuously increasing attacks as well as report high performance overhead. In this talk, we will study two new directions in cryptography, namely lightweight cryptography and post-quantum cryptography. Based on these advances, we will present how the current trusted computing protocols are being adapted to take advantage of these cryptographic advances. We will present detailed comparison for two specific protocols, namely, transparent memory encryption and post-quantum secure boot.

### Presenters
Burin is a third year Ph.D. student at the National University of Singapore, Singapore. His research interests include physical attacks, graph accelerator, neuromorphic computing and computer architecture. Prior to joining the Ph.D. programme, Burin graduated from Chulalongkorn University, Thailand, with a bachelor's degree in computer engineering.

<link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
