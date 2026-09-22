<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The time $T$ is the [waiting time for two consecutive successes](../../../../../../waiting-time-for-two-consecutive-successes.md) in [independent](../../../../../../independent-random-variables.md) fair trials. First note its integrability: if any one of the disjoint pairs $(X_1,X_2),\ldots,(X_{2k-1},X_{2k})$ is $++$, then $T\leq2k$. Thus $\mathbb P(T>2k)\leq(3/4)^k$.

Let $e_0$ be the expected additional waiting time with no trailing positive step, and let $e_1$ be the expected additional time when the preceding step was positive. Conditioning on the next [independent](../../../../../../independent-random-variables.md) increment gives

$$
e_0=1+\tfrac12e_0+\tfrac12e_1,\qquad e_1=1+\tfrac12e_0.
$$

A negative step returns either state to state $0$; a positive step moves state $0$ to state $1$ and completes the pattern from state $1$. Substitution yields $e_0=2+e_1=3+e_0/2$, so $e_0=6$. The original process starts in state $0$, and therefore

$$
\boxed{\mathbb E T=6.}
$$

Overlapping pairs are dependent, so regarding each successive pair as a fresh trial of success [probability](../../../../../../probability.md) $1/4$ would give the wrong [expectation](../../../../../../expected-value.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
