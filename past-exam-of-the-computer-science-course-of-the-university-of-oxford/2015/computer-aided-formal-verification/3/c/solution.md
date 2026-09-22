<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Every [state](../../../../../state-computer-science.md) has at least one successor, so $\operatorname{Post}(s)\nsubseteq\varnothing$ for every $s\in S$. Therefore

$$
\boxed{H(\varnothing)=A\cap\varnothing=\varnothing.}
$$

The [empty set](../../../../../empty-set.md) is always a [fixed point](../../../../../fixed-point.md). Whenever $G_\Phi$ is nonempty, it is therefore an additional, distinct [fixed point](../../../../../fixed-point.md).

For an explicit example, take a one-[state](../../../../../state-computer-science.md) [transition system](../../../../../transition-system.md) with $S=\{s\}$, the [self-loop](../../../../../loop-graph-theory.md) $s\to s$, and $A=S$. Then $G_\Phi=S$ and $H$ has the two distinct [fixed points](../../../../../fixed-point.md) $\varnothing$ and $\{s\}$. This example meets the requirement of no [terminal states](../../../../../terminal-state.md).

The wording does not guarantee distinct additional [fixed points](../../../../../fixed-point.md) for every instance. For example, if $A=\varnothing$, then $H(X)=\varnothing$ for every $X$ and its only [fixed point](../../../../../fixed-point.md) is $G_\Phi=\varnothing$. Thus **additional fixed points can occur, but need not occur**. The universal example $\varnothing$ is distinct precisely when the desired [satisfaction set](../../../../../satisfaction-set.md) is nonempty, as also follows from the [greatest fixed point](../../../../../greatest-fixed-point.md) argument below.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Computer aided formal verification](../../../computer-aided-formal-verification-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
