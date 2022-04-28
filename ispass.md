---
layout: page
title: Hardware Security Tutorial in ISPASS-2022
permalink: /ispass2022/
---

The 2022 IEEE International Symposium on Performance Analysis of Systems and Software (ISPASS-2022), which will be hosting at the National University of Singapore in Singapore on 22-24 May 2022, will be organizing a hardware security tutorial session on 22 May. The authors are looking forward to sharing the works and having an in-person discussion during the tutorial session. The list below shows the topics that will be discussed in the tutorial session.

- Laser Attack Benchmark Suite (LABS)
- Efficient Security Protocol Realization for Secure Processors
- A multi-level evaluation framework for side-channel evaluations on embedded devices

### Laser Attack Benchmark Suite (LABS)
#### Presenter: Burin Amornpaisannon

Laser fault injection is one of the most dangerous techniques for fault injection as laser shots can be fired at the precise location and at the right time.

Security evaluation against laser attacks requires costly, sophisticated equipment, and is typically evaluated during the post fabrication stage, which occurs too late. If a vulnerability is found during this stage, the circuit designers inevitably have to restart the entire time-consuming design stages. It is therefore impractical to evaluate chips solely during this stage.

Laser attack benchmark suite (LABS) is proposed to overcome these limitations. LABS is a framework that allows circuit designers to evaluate their designs and protections at early RTL stage or on an FPGA against laser attacks without manual modifications. It supports both processors and accelerators, and covers various widely used applications. From the potential use-case scenarios attacking a processor and accelerator, simulation of the attacks supported by LABS only takes minutes to finish.

LABS also consists of automatic hardware-based redundancy integration, supporting a variety of techniques, that helps protect the design against laser attacks. When a vulnerability is found from the attacks, it can automatically integrate redundancy techniques to a specific part of the design based on the user’s configuration. 

LABS is an open-source modular framework open for extensions. The users can easily add more features, for instance, attacks and defenses to LABS to meet their needs. The attacks and defenses together that LABS provides will automate the entire pre-silicon security evaluation flow against laser fault injection attacks.

During this tutorial, the background on general and laser fault injection attacks is described, comprehensive comparisons between different approaches are elaborated, as well as LABS is presented and demonstrated. 

### Efficient Security Protocol Realization for Secure Processors
#### Presenter: Naina Gupta

Modern microprocessors present various layers of trusted computing, based on a fundamental root-of-trust. The root-of-trust is typically implemented through a lightweight crypto co-processor. Despite the best efforts, the currently available commercial processors with trusted computing support - face continuously increasing attacks as well as report high performance overhead. In this talk, we will study two new directions in cryptography, namely lightweight cryptography and post-quantum cryptography. Based on these advances, we will present how the current trusted computing protocols are being adapted to take advantage of these cryptographic advances. We will present detailed comparison for two specific protocols, namely, transparent memory encryption and post-quantum secure boot.

### A multi-level evaluation framework for side-channel evaluations on embedded devices
#### Presenter: Shivam Bhasin

In this talk, we take a holistic look at evaluation of embedded systems against side-channel attacks. We propose a generic framework to guide side-channel evaluations at three different levels.  At the basic level, test are designed to be provide a high-level security estimate of the target at hand. Based on basic information like targeted algorithm, signal to noise ratio, implementation style, a quick and rough estimate of the security can be learned. Educated evaluation takes this evaluation deeper by providing reliable hints about underlying protection mechanism to the evaluator. Finally advanced evaluation provides the worst case security guarantees by running lengthy and tedious test. Such a multi-level evaluation framework prevents fault sense of security by a limited evaluation as for example with a basic evaluation.

### Presenter Bios
Burin is a third year Ph.D. student at the National University of Singapore, Singapore. His research interests include physical attacks, graph accelerator, neuromorphic computing and computer architecture. Prior to joining the Ph.D. programme, Burin graduated from Chulalongkorn University, Thailand, with a bachelor's degree in computer engineering.

Naina Gupta received the bachelor's degree from Guru Gobind Singh Indraprastha University (GGSIPU), India, in 2013 and the master's degree from IIIT-Delhi, India, in 2015. She is currently pursuing Ph.D. degree from School of Computer Science and Engineering (SCSE), Nanyang Technological University (NTU), Singapore from 2018 onwards. Prior to that she has worked as a researcher in IIIT-Delhi from 2015 to 2017 and as an intern in NTU, Singapore from 2017 to 2018. Her research interests are cryptography, side-channel attacks, hardware security, post-quantum cryptography and efficient implementations of cryptographic algorithms.

Dr. Shivam Bhasin is a Senior Research Scientist and Programme Manager (Cryptographic Engineering) at Centre for Hardware Assurance, Temasek Laboratories, Nanyang Technological University Singapore. He received his PhD in Electronics & Communication from Telecom Paristech in 2011, Advanced Master in Security of Integrated Systems & Applications from Mines Saint-Etienne, France in 2008. Before NTU, Shivam held position of Research Engineer in Institut Mines-Telecom, France. He was also a visiting researcher at UCL, Belgium (2011) and Kobe University (2013). His research interests include embedded security, trusted computing and secure designs. He has co-authored several publications at recognized journals and conferences. Some of his research now also forms a part of ISO/IEC 17825 standard.

<link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
