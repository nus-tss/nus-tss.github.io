---
layout: page
title: "Fuzz Testing"
permalink: /fuzzing/index.html
---

## Fuzz Testing

<table style="border: none">
  <tr>
    <td style="border: none"><a href="/fuzzing"><u><b>Overview</b></u></a></td>
    <td style="border: none"><a href="/fuzzing/news"><b>News</b></a></td>
    <td style="border: none"><a href="/fuzzing/publications"><b>Publications</b></a></td>
    <td style="border: none"><a href="/fuzzing/people"><b>People</b></a></td>
    <td style="border: none"><a href="/fuzzing/summerschool"><b>Summer School</b></a></td>
    <td style="border: none"><a href="/fuzzing/vacancies"><b>Vacancies</b></a></td>
    <td style="border: none"><a href="/fuzzing/contact"><b>Contact</b></a></td>
  </tr>
</table>

<img src="{{ 'images/fuzzing_overview.jpg' | relative_url }}" width="200" alt="Fuzzing" style="float:left; margin: 0px 15px 0px 0px;" />

Software almost always has vulnerabilities. Many of these cause serious problems such as software crash and leaking sensitive user information. To fix bugs, software engineers have been fighting an endless battle with bugs. The cost of this battle is enormous—$312 billion per year globally as of 2012 according to [Cambridge University research](http://insight.jbs.cam.ac.uk/2013/financial-content-cambridge-university-study-states-software-bugs-cost-economy-312-billion-per-year/) (in comparison, the GDP of Singapore is $308 billion as of 2014). This high cost is due to that software developers spend about 50% of their time debugging. We are conducting research on automatically finding vulnerabilities in program binaries by combining black-box or grey-box fuzzing with symbolic execution approaches. In black-box or grey-box fuzzing, the logic of the program is not analyzed, whereas symbolic execution approaches proceed by a semantic analysis of the program behavior. A lot of our research can be seen as a targeted search where we are trying to reach target locations, either to reproduce a crash or to uncover more behavior so that vulnerabilities can be uncovered.

One of the key innovations in our approach is that the analysis for finding vulnerabilities works directly on the program binaries - no source code is needed. Another key innovation is the development of scalable search strategies to guide the symbolic analysis for common file-format processing programs such as PDF, PNG, WAV. We are also working on improving grey-box fuzzing technology in its weak-point, namely behavioral coverage. Grey-box fuzzing technology generates many inputs with the goal to crash the program, but may end up covering few paths in the program since no semantic analysis is involved. In our latest work, we have improved the search heuristics inside fuzzers to drastically improve the coverage without resorting to costly symbolic analysis. Thus, our approach for finding vulnerabilities is two pronged - improve the scalability of the symbolic execution or semantic approaches, and improve the behavioral coverage of fuzzing or syntactic approaches.

---
<br>


<img src="{{ 'images/nrf_logo.png' | relative_url }}" width="250" alt="Fuzzing" style="float:left; margin: 0px 30px 15px 0px;" />

Our research in **fuzz testing** is funded with a grant from **National Research Foundation (NRF) Cybersecurity R&D**, (2023-27).

<br>

---
<br>

<!--## Viewpoint-->

<img src="{{ 'images/fuzzing_article.png' | relative_url }}" width="250" alt="Fuzzing" style="float:left; margin: 0px 30px 15px 0px;" />

Check our [IEEE Software Article](https://www.computer.org/csdl/magazine/so/2021/03/09166552/1mgaKsMFDYA) reflecting on fuzzing as a field.
We summarize the open challenges and opportunities for fuzzing and symbolic execution as they emerged in discussions among researchers and practitioners in a Shonan Meeting and that were validated in a subsequent survey.

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

---
<br>

## Recent News

* July, 2023: <a href="news/#july-2023">News research project funded!</a>

<br>

---
<br>





## Relevant Technology

* [AFLGo](https://github.com/aflgo/aflgo): Directed fuzzer

* [AFLFast](https://github.com/mboehme/aflfast): Integrated into AFL now

* [TimeMachine](https://github.com/DroidTest/TimeMachine):  Android app fuzzing

* [AFLSmart](https://github.com/aflsmart/aflsmart): Structure aware fuzzing

* [AFLNet](https://github.com/aflnet/aflnet): Response code based stateful fuzzing

* ...  < more to come, watch this space>