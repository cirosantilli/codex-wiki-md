<h1 id="3/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The bounded-time [optional sampling theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) says that for an [integrable](../../../../../integrability.md) discrete-time [martingale](../../../../../martingale-split.md) $(U_n)$ and a [bounded stopping time](../../../../../bounded-stopping-time.md) $S$, $\mathbb E[U_S]=\mathbb E[U_0]$. It requires no assumption about an eventual unbounded [stopping time](../../../../../stopping-time.md).

Apply this theorem with $S=n\wedge\tau$, or simply take the [expectation](../../../../../expected-value-split.md) of the [stopped martingale](../../../../../stopped-martingale.md) in part (ii). For $N>0$ we obtain

$$
\mathbb E[P_{n\wedge\tau}]+\frac N3\mathbb E[n\wedge\tau]=abc.
$$

Since $P_{n\wedge\tau}\geq0$,

$$
\mathbb E[n\wedge\tau]\leq\frac{3abc}{N}.
$$

The [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) now yields $\mathbb E[\tau]\leq3abc/N<\infty$. In particular $\tau<\infty$ [almost surely](../../../../../almost-sure-convergence.md), which has been established without assuming that [optional stopping](../../../../../optional-sampling-theorem-for-a-supermartingale.md) is valid at $\tau$.

For each [sample path](../../../../../sample-path.md) with finite $\tau$, $P_{n\wedge\tau}$ eventually equals $P_\tau=0$. Also $0\leq P_{n\wedge\tau}\leq N^3$. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives $\mathbb E[P_{n\wedge\tau}]\to0$. Taking the [limit of a sequence](../../../../../limit-of-a-sequence.md) in the earlier identity therefore proves

$$
\boxed{\mathbb E[\tau]=\frac{3abc}{a+b+c}.}
$$

For example, initial holdings $(1,1,1)$ give [expectation](../../../../../expected-value-split.md) one, as the first transfer must eliminate its giver. This computes the first elimination time, rather than the later time when one player owns all tokens.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
