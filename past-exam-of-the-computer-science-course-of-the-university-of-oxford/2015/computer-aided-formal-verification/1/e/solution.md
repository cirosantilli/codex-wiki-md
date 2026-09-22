<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose the [variable ordering of a binary decision diagram](../../../../../variable-ordering-of-a-binary-decision-diagram.md) $y<x<z$. The [Boolean cofactor](../../../../../boolean-cofactor.md) with $y=1$ is the constant one, while the [Boolean cofactor](../../../../../boolean-cofactor.md) with $y=0$ is $x\land z$. Consequently the right panel in part (d) has the following arrows:

$$
\boxed{y:\ (0\to x,\ 1\to1),\qquad
x:\ (0\to0,\ 1\to z),\qquad
z:\ (0\to0,\ 1\to1).}
$$

Here an entry such as $0\to x$ denotes the zero arrow to the $x$ [decision node](../../../../../decision-node.md). There are $\boxed{3+2=5}$ [vertices](../../../../../vertex-graph-theory.md): three [decision nodes](../../../../../decision-node.md) and two [terminal nodes](../../../../../terminal-node.md), saving one [decision node](../../../../../decision-node.md) relative to either of the previous orderings. Testing $y$ first is effective because its one branch settles the entire [Boolean function](../../../../../boolean-function.md) immediately. The ordering $y<z<x$ works equally well.

This is also minimal among ordinary [binary decision diagrams](../../../../../binary-decision-diagram.md) for this [Boolean function](../../../../../boolean-function.md). Each [Boolean variable](../../../../../boolean-variable.md) is essential: setting $y=0,z=1$ leaves $f=x$; setting $y=0,x=1$ leaves $f=z$; and setting $x=z=0$ leaves $f=y$. If a [Boolean variable](../../../../../boolean-variable.md) were never tested, the represented [Boolean function](../../../../../boolean-function.md) could not depend on it. Thus at least three [decision nodes](../../../../../decision-node.md) are necessary, and the construction attains that bound.

## ↑ Ancestors (11)

1. [E](../e.md)
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
