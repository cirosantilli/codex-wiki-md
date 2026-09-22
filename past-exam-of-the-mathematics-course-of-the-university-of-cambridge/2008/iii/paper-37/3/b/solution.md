<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $D=d\mathbb Q/d\mathbb P$ on $\mathcal F$. The [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) is nonnegative and $\mathbb E_{\mathbb P}D=1$. For $A\in\mathcal F_t$,

$$
\mathbb Q(A)=\mathbb E_{\mathbb P}(D\mathbf1_A)=\mathbb E_{\mathbb P}\bigl(\mathbb E_{\mathbb P}(D\mid\mathcal F_t)\mathbf1_A\bigr).
$$

Uniqueness of the restricted [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) therefore identifies

$$
\boxed{Z_t=\mathbb E_{\mathbb P}(D\mid\mathcal F_t)\geq0.}
$$

For $s\leq t$, the tower property of [conditional expectation](../../../../../../conditional-expectation.md) gives $\mathbb E_{\mathbb P}(Z_t\mid\mathcal F_s)=Z_s$, and $\mathbb E_{\mathbb P}Z_t=1$. Thus $Z$ is a nonnegative true [martingale](../../../../../../martingale-split.md), indeed a [uniformly integrable martingale](../../../../../../uniformly-integrable-martingale.md), since it consists of conditional expectations of one integrable random variable. This is the [Radon-Nikodym density martingale](../../../../../../radon-nikodym-density-martingale.md). Under the [usual conditions for a filtration](../../../../../../usual-conditions-for-a-filtration.md), it has the standard càdlàg version; continuity is the additional assumption in part (c), not a consequence of absolute continuity alone.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
