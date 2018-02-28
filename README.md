# CMPUT 4XX : Foundations of Program Analysis

## Term: Winter 2019
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
- Selected papers from [this reading list](https://github.com/staticanalysisseminar/resources/blob/master/papers.md).

## Format
Two lectures per week (Tuesdays and Thursdays). Lectures will include introducing new material, hands-on work with program analysis tools, and, later on in the course, paper discussions.

## Evaluation
* Assignments: 30%
* Paper Discussions: 30%
* Course Project: 40%
  * Proposal: 5%
  * Presentation: 10%
  * Report: 25%

## Important Deadlines
* Assignment 1  : Jan 25 @ 5pm
* Assignment 2  : Feb 15 @ 5pm
* Assignment 3  : Mar 08 @ 5pm
* Project Report: Apr 12 @ 5pm

## Schedule
| Date | Lecture |
| ---- | ------- |
| Jan 08 | Intro + Sample Analyses |
| Jan 10 | Intermediate Representations |
| Jan 15 | Lattices and Fixpoints |
| Jan 17 | Intra-procedural Analysis |
| Jan 22 | Type-based Call Graph Construction |
| Jan 24 | Propagation-based Call Graph Construction |
| Jan 29 | Pointer Analysis |
| Jan 31 | Alias Analysis |
| Feb 05 | Grad Project Proposals |
| Feb 07 | Inter-procedural Analysis |
| Feb 12 | Context-Sensitivity with Call Strings Approach |
| Feb 14 | Context-Sensitivity with Functional Approach |
| Feb 19 | Reading Week |
| Feb 21 | Reading Week |
| Feb 26 | Inter-procedural Finite Distributed Subset problems (IFDS) |
| Feb 28 | Inter-procedural Distributed Environment problems (IDE) |
| Mar 05 | Non-Distributive Analyses |
| Mar 07 | Usability of Program Analysis Tools |
| Mar 12 | Undergrad Project Proposals |
| Mar 14 | Undergrad Project Proposals |
| Mar 19 | Paper Discussions (Usability) |
| Mar 21 | Paper Discussions (Security) |
| Mar 26 | Paper Discussions (Dynamic Languages) |
| Mar 28 | Paper Discussions (Predictive Program Analysis) |
| Apr 02 | Paper Discussions (Program Synthesis) |
| Apr 04 | Paper Discussions (Probabilistic Programming) |
| Apr 09 | Project Presentations |
| Apr 11 | Project Presentations |

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
