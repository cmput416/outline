# CMPUT 416 : Foundations of Program Analysis

## Term: Fall 2020
## Course Weight: 3 credits
## Instructor: [Karim Ali](http://karimali.ca)

## Description
One can ask many interesting questions about a given program such as:
- Does this program terminate?
- Can the pointer `p` be `null`?
- Will the value of the variable `v` be read in the future?
- Do the variables `x` and `y` point to the same location in memory?
- Could the secret data pointed to by `s` leak to some unauthorized party?

Answering any of those interesting questions about a program is undecidable as stated by Rice's Theorem. However, people usually use program analysis to get approximate answers to those questions, which works well in many cases. For example, many bug finding tools (e.g., FindBugs) use various program analysis techniques to detect, and possibly fix, bugs in a given program. Additionally, security analysis tools (e.g., AppScan, FlowDroid) also use program analysis to detect security vulnerabilities and data leaks.

This course will introduce the main concepts behind program analysis including intermediate representations, inter-procedural and intra-procedural analysis techniques, call graphs, pointer analysis, and analysis frameworks. We will also discuss some relevant research papers that introduce both classical and state-of-the-art research in the field. The course will give an overview of the program analyses that work and those that do not work in practice and how to design program analyses for modern software systems (e.g., Android).

## Prerequisites
- CMPUT 275 or CMPUT 201
- CMPUT 229
- CMPUT 272

## Reference Materials
- Uday Khedker, Amitabha Sanyal, and Bageshri Karkare. Data Flow Analysis: Theory and Practice. CRC Press (Taylor and Francis Group). 2009.
- Alfred V. Aho, Ravi Sethi, and Jeffrey D. Ullman. Compilers: Principles, Techniques, and Tools. Addison-Wesley. 2006. (https://www.library.ualberta.ca/catalog/2320584)
- Matthew S. Hecht. Flow Analysis of Computer Programs. Elsevier North-Holland Inc. 1977. (https://www.library.ualberta.ca/catalog/176283)
- Steven S Muchnick and Neil D Jones. Program Flow Analysis: Theory and Applications, chapter 7, pages 189-233. 1981. (https://www.library.ualberta.ca/catalog/385204)
- Flemming Nielson, Hanne Riis Nielson, and Chris Hankin. Principles of Program Analysis, 2005.
- Benjamin C. Pierce. Types and Programming Languages. MIT Press. 2002.
- Selected papers from [this reading list](https://github.com/cmput416/resources/blob/master/papers.md).

## Format
Two lectures per week (Tuesdays and Thursdays). Lectures will include introducing new material, hands-on work with program analysis tools, and, later on in the course, paper discussions.

## Evaluation
* Assignments: 35%
* Paper Discussions: 20%
* Course Project: 45%
  * Proposal Presentation = 5%
  * Proposal Document = 5%
  * Final Presentation = 10%
  * Final Document = 20%
  * GitHub Repository = 5%

## Course Schedule
<table border="1">
    <thead>
        <tr>
            <th style="text-align:center">Week</th>
            <th>Monday</th>
            <th>Tuesday</th>
            <th>Wednesday</th>
            <th>Thursday</th>
            <th>Friday</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="text-align:center">31.08--04.09</td>
            <td></td>
            <td><a href="https://youtu.be/bspS8eNgnkE" target="_blank">Intro</a></td>
            <td></td>
            <td><a href="https://youtu.be/-zyMw_0RmeY" target="_blank">Sample Analyses + Intermediate Representations</a></td>
            <td></td>
        </tr>
        <tr>
            <td style="text-align:center">07.09--11.09</td>
            <td></td>
            <td><a href="https://youtu.be/YCNeXeL66WU" target="_blank">Intra-Procedural Analysis</a></td>
            <td></td>
            <td><a href="https://youtu.be/PqpN5vKvAT0" target="_blank">Lattice Theory 1</a></td>
            <td><code>A1</code></td>
        </tr>
        <tr>
            <td style="text-align:center">14.09--18.09</td>
            <td></td>
            <td><a href="https://youtu.be/WqEm5zn1zUM" target="_blank">Lattice Theory 2</a></td>
            <td></td>
            <td><a href="https://youtu.be/89aLM1et1ds" target="_blank">Monotone Flow Functions</a><br></td>
            <td></td>
        </tr>
        <tr>
            <td style="text-align:center">21.09--25.09</td>
            <td></td>
            <td><a href="https://youtu.be/KGNkH7eHU_Y" target="_blank">Call Graph Construction</a></td>
            <td></td>
            <td><a href="https://youtu.be/8du-qmduhcQ" target="_blank">CG Hands-On</a><br></td>
            <td><code>A2</code></td>
        </tr>
        <tr>
            <td style="text-align:center">28.09--02.10</td>
            <td></td>
            <td><a href="https://youtu.be/OEFpWWnyVo4" target="_blank">Pointer Analysis</a><br></td>
            <td></td>
            <td><a href="https://youtu.be/Is9yqpNFQhQ" target="_blank">Inter-Procedural Analysis</a><br></td>
            <td><code>A3</code></td>
        </tr>
        <tr>
            <td style="text-align:center">05.10--09.10</td>
            <td></td>
            <td><a href="https://youtu.be/wgnbTv-kNAU" target="_blank">Context Sensitivity</a></td>
            <td></td>
            <td><a href="https://youtu.be/y7iLreS37MA" target="_blank">Inter-procedural Finite Distributed Subset problems (IFDS) 1</a></td>
            <td><code>A4</code></td>
        </tr>
        <tr>
            <td style="text-align:center">12.10--16.10</td>
            <td></td>
            <td><a href="https://youtu.be/lJbiwYa6mVM" target="_blank">IFDS 2</a><br></td>
            <td></td>
            <td><a href="https://youtu.be/76x95LO-NI0" target="_blank">Inter-procedural Finite Distributed Environment problems (IDE)</a><br></td>
            <td><code>Proposal Document</code></td>
        </tr>
        <tr>
            <td style="text-align:center">19.10--23.10</td>
            <td></td>
            <td><code>Proposal Presentations</code></td>
            <td></td>
            <td>Guest Lecture</td>
            <td><code>A5</code></td>
        </tr>
        <tr>
            <td style="text-align:center">26.10--30.10</td>
            <td></td>
            <td><code>Paper Seminars</code></td>
            <td></td>
            <td><code>Paper Seminars</code></a></td>
            <td></td>
        </tr>
        <tr>
            <td style="text-align:center">02.11--06.11</td>
            <td></td>
            <td><code>Paper Seminars</code></td>
            <td></td>
            <td><code>Paper Seminars</code></td>
            <td><code>A6</code></td>
        </tr>
        <tr>
            <td style="text-align:center">09.11--13.11</td>
            <td colspan="6" style="text-align:center"><strong>&lt;= Reading Week =&gt;</strong></td>
        </tr>
        <tr>
            <td style="text-align:center">16.11--20.11</td>
            <td></td>
            <td><code>Paper Seminars</code></td>
            <td></td>
            <td><code>Paper Seminars</code></td>
            <td><code>A7</code></td>
        </tr>
        <tr>
            <td style="text-align:center">23.11--27.11</td>
            <td></td>
            <td><code>Paper Seminars</code></td>
            <td></td>
            <td><code>Paper Seminars</code></td>
            <td></td>
        </tr>
        <tr>
            <td style="text-align:center">30.11--04.12</td>
            <td></td>
            <td><code>Final Presentations</code></td>
            <td></td>
            <td><code>Final Presentations</code></td>
            <td><code>Final Report</code></td>
        </tr>
    </tbody>
</table>

## Paper Discussions
Most in-class paper discussions suffer from the lack of attention from most students except the presenter. To provide a more interactive environment for the paper discussions in this course, student will take the following roles:

*   **Presenter** (20 mins): give a presentation about the paper.
*   **Historian** (10 mins): position the paper in the context of related work (either prior to the paper, or later work that extends/critiques the paper). You will present your findings in class.
*   **Reviewer** (10 mins): review the paper as if you are serving on the Program Committee. Tell us why the committee should accept/reject the paper. These are some useful links that contain tips on how to read and review academic papers: [link1](http://www.cgl.uwaterloo.ca/smann/Research/review-conference.txt), [link2](http://homes.cs.washington.edu/~mernst/advice/meier-paper.review.html), [link3](http://www.cl.cam.ac.uk/~ey204/teaching/ACS/R212_2015_2016/aid/stevens.pdf), [link4](http://library.queensu.ca/inforef/criticalreview.htm), [link5](http://cseweb.ucsd.edu/~wgg/CSE210/howtoread.html).
*   **Researcher** (10mins): propose one project that extends or is inspired by the work discussed in the paper, and is related to your research area (for grad students). Pitch that project idea to us in class!
*   **Validator** (20 mins): search for, download, and validate any artifacts that are published with the work (e.g., an official artifact, source code available on the internet, scripts to mine data/code, proofs, tools, survey data/methodology). If you can't find anything online, contact the authors. In class, you will walk us through your findings, and demo any tools that were published with the paper.
*   **All students**: come up with one question about the core ideas presented in the paper, and pose that question during class.

Each paper discussion will end with a 10-minute open discussion to open the floor to further questions from the audience.

*Note: this structure is inspired by the [Machine Learning for Interactive Systems and Advanced Programming Tools Seminar at ETH](https://ait.ethz.ch/teaching/courses/2016-FS-ML-IS-PL/).*
