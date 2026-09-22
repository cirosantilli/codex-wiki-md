<h1 id="4/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $d_j$ be the number of events at potential time $a_j$ and let $r_j$ be the size of the [risk set](../../../../../../../risk-set.md) immediately before that time, including observations censored at $a_j$. Define the discrete conditional event probability

$$
q_j=\mathbb P(T=a_j\mid T\geq a_j).
$$

Under [independent censoring](../../../../../../../independent-censoring.md), and ignoring the separate censoring distribution, the [survival likelihood](../../../../../../../survival-likelihood.md) factorizes as

$$
L(\{q_j\})\propto\prod_j q_j^{d_j}(1-q_j)^{r_j-d_j}.
$$

This follows by multiplying a survival factor for each individual at risk who does not fail at $a_j$, and an event factor for each failure. The log factor $d_j\log q_j+(r_j-d_j)\log(1-q_j)$ is maximized at $\widehat q_j=d_j/r_j$, with the corresponding boundary values when $d_j=0$ or $d_j=r_j$.

The [survival function](../../../../../../../survival-function.md) is the product of successive conditional survival probabilities. Therefore

$$
\boxed{\widehat F(t)=\prod_{a_j\leq t}\left(1-\frac{d_j}{r_j}\right).}
$$

This is the [Kaplan–Meier estimator](../../../../../../../kaplan-meier-estimator.md). A product over no event times is 1. If everyone remaining experiences an event, the product becomes zero and stays zero; subsequent empty [risk sets](../../../../../../../risk-set.md) supply no additional factor.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
