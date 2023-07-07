---
layout: fuzzing
title: "Fuzz Testing"
permalink: /fuzzing/index.html

download: <i class="fa fa-download"></i>
pdf: <i class="fa fa-file-pdf-o"></i>
---

<img src="{{ 'images/fuzzing_overview.jpg' | relative_url }}" width="200" alt="Fuzzing" style="float:left; margin: 0px 15px 0px 0px;" />

Software almost always has vulnerabilities. Many of these cause serious problems such as software crash and leaking sensitive user information. To fix bugs, software engineers have been fighting an endless battle with bugs. To date, the most known mechanism for testing against security vulnerabilities is grey-box fuzz testing (fuzzing) — a proven and practical bug detection methodology. At its core, fuzz testing uses a biased random search to uncover inputs that are likely to cause the program to misbehave (e.g., crash), thereby allowing bugs to be discovered and fixed before potential exploitation.  In recent years, most software vulnerabilities are found using fuzz testing. Our research program seeks to build next generation fuzz testing technologies, specifically in the light of supply-chain attacks witnessed recently.

<a href="https://www.computer.org/csdl/magazine/so/2021/03/09166552/1mgaKsMFDYA"><img src="{{ 'images/fuzzing_article.png' | relative_url }}" width="230" alt="IEEE Software Article" style="float:right; margin: 0px 0px 0px 15px;" /></a>

From a technical standpoint, this program will develop new techniques in testing and analysis, for detecting security vulnerabilities, specifically for concurrent, stateful and reactive software systems. Traditionally these systems have been checked via verification methods which store the state space in some form. Since common usage of the verification methods is in bug finding, we propose to develop smart fuzzing methods to validate stateful systems. Technically this will involve various innovations in (a) identifying state variables in programs (b) inferring stateful behavior and state machines even when state variables may not be accurately identified, (c) being able to fuzz concurrent systems to capture the space of interleavings and (d) designing test oracles and automated testing techniques to find various kinds of bugs in data-centric software. Being able to validate concurrent / distributed / stateful systems, allows us to deeply test the impact of a vendor provided component on (stateful) software. The proposed research is of importance in the context of recent well-known supply chain attacks, such as Solarwinds. Fuzz testing and binary analysis techniques can be employed to prevent such attacks (and others) - to mitigate their impact. 

The research program also looks at sound statistical basis for comparing evaluation of fuzzer tools, so that practitioners can choose fuzzers which are useful for their specific application set-up to find vulnerabilities effectively. This can also impact the way fuzzer evaluations are currently conducted in well-known computational infrastructures including Google’s Fuzzbench.

Check our [IEEE Software Article](https://www.computer.org/csdl/magazine/so/2021/03/09166552/1mgaKsMFDYA) reflecting on fuzzing as a field.
We summarize the open challenges and opportunities for fuzzing and symbolic execution as they emerged in discussions among researchers and practitioners in a Shonan Meeting and that were validated in a subsequent survey.



---
<br>


<img src="{{ 'images/nrf_logo.png' | relative_url }}" width="250" alt="Fuzzing" style="float:left; margin: 0px 30px 15px 0px;" />

Our research in **fuzz testing** is funded with a grant from **National Research Foundation (NRF) Cybersecurity R&D**, (2023-27).

<br>

---
<br>


<div class="row">
    <div class="col-sm-8">
        <div class="news-details">
Check Prof. Abhik Roychoudhury's <a href="{{ '../files/NUSJuly2023.pdf' | relative_url }}">{{page.download}} slides</a> for his <a href="https://events.comp.nus.edu.sg/view/20906">CS Seminar</a> talk about <b>Fuzz Testing</b>. He describes the story about how he started his research in fuzz testing and highlights several impactful research outcomes.
        </div>
    </div>
    <div class="col-sm-4 mx-auto my-auto" align="center">      
<a href="{{ '../files/NUSJuly2023.pdf' | relative_url }}"><img src="{{ '../files/NUSJuly2023.jpg' | relative_url }}" width="250" alt="Fuzzing Slides" style="float:left; margin: 15px 15px 15px 0px;" /></a>
    </div>
</div>

<br>

---
<br>


## Recent News

* July  2023: <a href="news/#july-2023">New research project funded!</a>
* April, 2022: <a href="news/#april-2022">Abhik Roychoudhury honored with IEEE New Directions Award</a>


<br>

---
<br>





## Relevant Technology

* [AFLGo](https://github.com/aflgo/aflgo): Directed fuzzer

* [AFLFast](https://github.com/mboehme/aflfast): Integrated into AFL now

* [TimeMachine](https://github.com/DroidTest/TimeMachine):  Android app fuzzing

* [AFLSmart](https://github.com/aflsmart/aflsmart): Structure aware fuzzing

* [AFLNet](https://github.com/aflnet/aflnet): Response code based stateful fuzzing

* [SQLancer](https://github.com/sqlancer/sqlancer): Automated testing to find logic bugs in database systems

* ...  < more to come, watch this space>
