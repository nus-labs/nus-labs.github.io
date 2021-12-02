---
layout: page
title: Laser Attack Benchmark Suite (LABS)
---
<center><img src="/images/overview.jpg" width="500" height="300"></center>

Laser fault injection is one of the most dangerous means to introduce faults into a target system due to the fact that laser shots can be fired at the right time and location with repeatability. Attackers can exploit faults induced by lasers to, for example, retrieve confidential information from an AES cryptographic algorithm or degrade neural network performance.

With most of the current design flows, security evaluation against laser fault injection is done after fabrication, which requires costly, sophisticated equipment and skilled technicians. Design respins are inevitable when vulnerabilities are found at this stage to integrate countermeasures. These limitations make this current security evaluation impractical. A framework that facilitates circuit designers to test their designs during the pre-fabrication stage is critically needed.

We propose the Laser Attack Benchmark Suite (LABS) that aims to complete the security evaluation loop against laser fault injection. LABS allows circuit designers to test their designs against well-known laser fault injection attacks and automatically integrate a hardware-based redundancy technique at the early RTL design stage. The modified design can be run with a Verilog simulator or on an FPGA without manual modifications. 

LABS is open for extensions and can be found in <a href="https://github.com/nus-labs/labs">the Github repository</a>.

<hr>
  <div class="container">
    <h3><b>Recent News</b></h3>
        <div class="inner">
          <div class="fauxcrop">
            <center><img alt="News Entry" src="/images/nus_news.jpg" width="350" height="200"></center>
          </div>
          <div class="ct-blog-content">
            <div class="ct-blog-date">
              <span>December</span><strong>28</strong>
            </div>
            <h3 class="ct-blog-header">
              <a href="https://news.nus.edu.sg/nus-scientists-develop-computational-tool-to-help-design-safer-devices/">NUS scientists develop computational tool to help design safer devices</a>
            </h3>
        </div>
        <div class="inner">
          <div class="fauxcrop">
            <center><img alt="News Entry" src="/images/nus_computing_news.jpg" width="350" height="220"></center>
          </div>
          <div class="ct-blog-content">
            <div class="ct-blog-date">
              <span>December</span><strong>28</strong>
            </div>
            <h3 class="ct-blog-header">
              <a href="https://www.comp.nus.edu.sg/news/features/2020-trevor-iot-attacks/">Protecting IoT devices from attack</a>
            </h3>
          </div>
  </div>

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
<div class="scrollmenu">
<h5><pre><code>@inproceedings{10.1145/3400302.3415646,
author = {Amornpaisannon, Burin and Diavastos, Andreas and Peh, Li-Shiuan and Carlson, Trevor E.},
title = {Laser Attack Benchmark Suite},
year = {2020},
isbn = {9781450380263},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3400302.3415646},
doi = {10.1145/3400302.3415646},
booktitle = {Proceedings of the 39th International Conference on Computer-Aided Design},
articleno = {50},
numpages = {9},
keywords = {laser fault attack, benchmark suite, integrated circuits, hardware security},
location = {Virtual Event, USA},
series = {ICCAD '20}}</code></pre></h5>
</div>

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

<link href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" rel="stylesheet">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>
