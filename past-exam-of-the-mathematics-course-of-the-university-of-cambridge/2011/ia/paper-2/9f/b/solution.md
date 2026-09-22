<h1 id="9f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $N$ denote the mattress count and $U$ the event of undisturbed sleep. Use the intended model in which the presence of the pea is independent of $N$, with probability $1/2$, and without a pea sleep is undisturbed. Conditioning on $N$ gives

$$
\mathbb P(U\mid N=6)=\frac12,\qquad
\mathbb P(U\mid N=7)=\frac12+\frac12\frac15=\frac35,\qquad
\mathbb P(U\mid N=8)=\frac12+\frac12\frac25=\frac7{10}.
$$

The [law of total probability](../../../../../../law-of-total-probability.md) and the equal prior probabilities give

$$
\boxed{\mathbb P(U)=\frac13\left(\frac12+\frac35+\frac7{10}\right)=\frac35.}
$$

By [Bayes' theorem](../../../../../../bayes-theorem.md), the posterior probabilities of $N=6,7,8$ given $U$ are respectively $5/18,6/18,7/18$. Therefore the [conditional expectation](../../../../../../conditional-expectation.md) is

$$
\boxed{\mathbb E[N\mid U]=6\frac5{18}+7\frac6{18}+8\frac7{18}=\frac{64}{9}.}
$$

Undisturbed sleep shifts the posterior toward larger mattress counts because those counts make the observation more likely.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9F](../../9f.md)
3. [Section II](../../section-ii.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
