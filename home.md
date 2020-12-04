---
layout: page
title: Laser Attack Benchmark Suite (LABS)
permalink: /
---

<center><img src="/images/overview.jpg" width="500" height="300"></center>

Laser fault injection is one of the most dangerous means to introduce faults into a target system due to the fact that laser shots can be fired at the right time and location with repeatability. Attackers can exploit faults induced by lasers to, for example, retrieve confidential information from an AES cryptographic algorithm or degrade neural network performance.

With most of the current design flows, security evaluation against laser fault injection is done after fabrication, which requires costly, sophisticated equipment and skilled technicians. Design respins are inevitable when vulnerabilities are found at this stage to integrate countermeasures, making this current security evaluation impractical. A framework that facilitates circuit designers to test their designs during the pre-fabrication stage is critically needed.

We propose the laser attack benchmark suite (LABS) that tries to complete the security evaluation loop against laser fault injection. LABS allows circuit designers to test their designs agaist well-known laser fault injection attacks and automatically integrate a hardware-based redundancy technique at the early RTL design stage. The modified design can be run with a Verilog simulator or on an FPGA without manual modifications. 

LABS is open for extensions, and can be found in <a href="https://github.com/nus-labs/labs">the Github repository</a>.

<hr>
<h3><b>Video</b></h3>
The 15-minute technical talk at ICCAD 2020. 
<div class="video-container">
  <iframe src="https://www.youtube.com/embed/pXdiQUBTQw8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

<hr>
<h3><b>Our Paper</b></h3>
<a href="https://www.comp.nus.edu.sg/~tcarlson/pdfs/amornpaisannon2020labs.pdf">Laser Attack Benchmark Suite</a>
<br>
2020 IEEE/ACM International Conference On Computer Aided Design (ICCAD)
<br>
Burin Amornpaisannon, Andreas Diavastos, Li-Shiuan Peh and Trevor E. Carlson
<h5><pre><code>@INPROCEEDINGS{9256786,
  author={B. {Amornpaisannon} and A. {Diavastos} and L. -S. {Peh} and T. E. {Carlson}}, 
  booktitle={2020 IEEE/ACM International Conference On Computer Aided Design (ICCAD)}, 
  title={Laser Attack Benchmark Suite}, 
  year={2020}, 
  volume={},
  number={},
  pages={1-9}, 
  doi={}}</code></pre></h5>

<hr>
<h3>Team</h3>
The team is with the Department of Computer Science, National University of Singapore.

<div class="row">
  <div class="column">
    <center>
      <img src="/images/amornpaisannon2.jpg" width="200" height="200">
      <br>
      <a href="https://bamornpa.github.io/"> Burin Amornpaisannon </a>
    </center>
  </div>
  <div class="column">
    <center>
      <img src="/images/diavastos.jpg" width="200" height="200">
      <br>
      <a href="https://www.linkedin.com/in/diavastos/"> Andreas Diavastos </a>
    </center>
  </div>
</div>

<div class="row">
  <div class="column">
    <center>
      <img src="/images/peh2.jpg" width="200" height="200">
      <br>
      <a href="https://www.comp.nus.edu.sg/~peh/"> Li-Shiuan Peh </a>
    </center>
  </div>
  <div class="column">
    <center>
      <img src="/images/carlson.jpg" width="200" height="200">
      <br>
      <a href="https://www.comp.nus.edu.sg/~tcarlson/"> Trevor E. Carlson </a>
    </center>
  </div>
</div>

<hr>
<h3>Acknowledgements</h3>
The authors acknowledge the support from the Singapore National Research Foundation (“SOCure” grant NRF2018NCR-NCR002-0001 – www.green-ic.org/socure).
