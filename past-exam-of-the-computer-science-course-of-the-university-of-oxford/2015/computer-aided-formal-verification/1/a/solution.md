<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Follow the [binary decision diagram](../../../../../binary-decision-diagram.md) from its top [decision node](../../../../../decision-node.md) to a [terminal node](../../../../../terminal-node.md), choosing the outgoing arrow specified by each tested [Boolean variable](../../../../../boolean-variable.md). If $x=0$, the left $y$ [decision node](../../../../../decision-node.md) returns $y$, independently of $z$. If $x=1$, the right $y$ [decision node](../../../../../decision-node.md) returns one when $y=1$ and otherwise returns $z$. Thus the [truth table](../../../../../truth-table.md), with rows in the order $(x,y,z)$, is:

| $x$ | $y$ | $z$ | $f(x,y,z)$ |
| --- | --- | --- | --- |
| 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 0 |
| 0 | 1 | 0 | 1 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 0 | 0 |
| 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 1 |

Thus the output column of the [truth table](../../../../../truth-table.md), in the displayed order, is $\boxed{(0,0,1,1,0,1,1,1)}$. In particular, the skipped $z$ test on the left does not constrain $z$: both values give the same result.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Computer aided formal verification](../../../computer-aided-formal-verification-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
