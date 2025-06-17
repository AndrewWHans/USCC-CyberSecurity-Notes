# How do we analyze a program?

Two approaches:
1) Static

2) Dynamic

## Concepts

We look for bugs (revolving memory corruption, rounding errors, null pointers, inf loop, etc)

## The SAT Problem

Lets say we are given a problem or formula that contains binary variables connected to logical relations like *OR* or *AND*.
The aim is to establish if there is any way to set the variables for that the formula **evaluates** to be *true*.
The Algorithms that're applied to this problem are known as *SAT solvers*.

In relevance to machine learning:
1) machine learning algo's rely on optimization.
2) machine learning techniques are often used as components of SAT solvers.





[What is Black Box Fuzzing?](https://www.fortra.com/solutions/application-security/dynamic-application-security-testing/black-box-fuzzing)<br>
[Static vs Dynamic Analysis](https://rahulsinghinfosec.github.io/hackme/reverse-engineering/static-vs-dynamic-analysis.html) <br>
[What is data-driven programming?](https://stackoverflow.com/questions/1065584/what-is-data-driven-programming) <br>
[SAT Solvers Introduction](https://rbcborealis.com/research-blogs/tutorial-9-sat-solvers-i-introduction-and-applications/) <br>
[SMT Solvers and Z3](https://de-engineer.github.io/SMT-Solvers/)
