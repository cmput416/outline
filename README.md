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
* Participation: 10%
* Seminars: 20%
* Course Project: 40%
  * Proposal: 5%
  * Final Presentation: 10%
  * Final Report: 25%

## Course Plan
| Date | Lecture |
| ---- | -------- |
| Week 1 | Intro + Sample Analysis + Intermediate Representations |
| Week 2 | Lattices + Data Flow Analysis Framework |
| Week 3 | Call Graph Construction |
| Week 4 | Pointer Analysis |
| Week 5 | Inter-procedural Finite Distributed Subset prblems (IFDS) |
| Week 6 | Inter-procedural Distributed Envorionment prolems (IDE) |
| Week 7 | Non-distributive Program Analyses |
| Week 8 | Project Proposals |
| Week 9 | Usability of Program Analysis Tools |
| Week 10 | Paper Discussions |
| Week 11 | Paper Discussions |
| Week 12 | Paper Discussions |
| Week 13 | Final Project Presentations |
