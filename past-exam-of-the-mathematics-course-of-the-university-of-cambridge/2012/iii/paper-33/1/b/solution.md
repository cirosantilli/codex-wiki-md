<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [stopped martingale](../../../../../../stopped-martingale.md)

$$
\boxed{M_n=1-S_{n\wedge T_1}.}
$$

It is nonnegative: before the first visit to $1$, the nearest-neighbour [random walk](../../../../../../random-walk.md) is at most $0$, and afterwards the stopped position is $1$. Each $M_n$ is integrable, with $|M_n|\leq n+1$. Moreover

$$
M_{n+1}-M_n=-\mathbf1_{\{T_1>n\}}X_{n+1}.
$$

The indicator is $\mathcal F_n$-measurable and the increment has conditional mean zero, so $M_n$ is a [martingale](../../../../../../martingale-split.md) with $\mathbb E M_n=M_0=1$.

Part (a) shows $T_1<\infty$ almost surely, so every such path eventually has $M_n=0$. Thus $M_n\to0$ almost surely. But $\mathbb E|M_n-0|=1$ for every $n$, so there is no [convergence in L1](../../../../../../convergence-in-l1.md). Any possible [L1 convergence](../../../../../../convergence-in-l1.md) limit would agree with the almost sure limit. This is a **nonnegative [martingale](../../../../../../martingale-split.md) with [almost sure convergence](../../../../../../almost-sure-convergence.md) but no [convergence in L1](../../../../../../convergence-in-l1.md)**, and hence it is not [uniformly integrable](../../../../../../uniform-integrability.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
