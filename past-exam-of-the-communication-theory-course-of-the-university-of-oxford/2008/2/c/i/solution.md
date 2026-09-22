<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The capacity of a [discrete memoryless channel](../../../../../discrete-memoryless-channel.md) is $C=\max_{P_X}I(X;Y)$, in bits per channel use. For the [binary symmetric channel](../../../../../binary-symmetric-channel.md) with crossover probability $p$, $H(Y\mid X)=h(p)$ and $H(Y)\le1$. A uniform input makes the output uniform, attaining

$$
\boxed{C_M=1-h(p)}.
$$

For the [binary erasure channel](../../../../../binary-erasure-channel.md), let $E$ be its erasure indicator. This flag is visible in the output and [independent](../../../../../independent-random-variables.md) of the input. If there is no erasure, the output reveals the input; otherwise it reveals nothing. Consequently

$$
I(X;Y)=(1-\epsilon)H(X),\qquad\boxed{C_N=1-\epsilon},
$$

again attained by a uniform input. These formulas include crossover probabilities zero and one, and complete erasure.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
