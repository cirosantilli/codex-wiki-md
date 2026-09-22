<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For each fixed $t\in[0,1]$, the variables $\mathbf1_{\{X_k\leq t\}}$ are [independent and identically distributed random variables](../../../../../../../independent-and-identically-distributed-random-variables.md) with [Bernoulli distribution](../../../../../../../bernoulli-distribution.md) of parameter $t$. Their [expected value](../../../../../../../expected-value.md) is $t$, and the [strong law of large numbers](../../../../../../../strong-law-of-large-numbers.md) gives $F_n(t)\to t$ [almost surely](../../../../../../../almost-sure-convergence.md).

For a finite set $F$, intersect these probability-one events over its finitely many elements. On the resulting single event, every one of the finitely many errors tends to zero, so their maximum tends to zero:

$$
\boxed{\sup_{t\in F}|F_n(t)-t|\longrightarrow0\quad\text{almost surely}.}
$$

If $F$ is empty, take the displayed maximum to be zero. The important point is simultaneous convergence on one event; pointwise convergence at an uncountable collection of arguments would not alone imply the uniform claim in part (ii).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
