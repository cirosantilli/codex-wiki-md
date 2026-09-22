<h1 id="26k/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Now assume $X_n\to X$ [almost surely](../../../../../../../almost-sure-convergence.md) and $\mathbb E[X_n^2]\to\mathbb E[X^2]$. In particular, $(X_n)$ is bounded in $L^2$, so it is [uniformly integrable](../../../../../../../uniform-integrability-from-bounded-second-moments.md) in $L^1$. Almost-sure convergence and [uniform integrability](../../../../../../../uniform-integrability.md) therefore give

$$
\mathbb E|X_n-X|\longrightarrow0.
$$

We next show that $X_n$ converges weakly to $X$ in the [L2 space](../../../../../../../l2-space-is-a-hilbert-space.md). For $Y\in L^2$, let $Y_M=Y\mathbf1_{\{|Y|\leq M\}}$. Then

$$
|\mathbb E[(X_n-X)Y_M]|\leq M\mathbb E|X_n-X|\longrightarrow0,
$$

while the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) gives, uniformly in $n$,

$$
|\mathbb E[(X_n-X)(Y-Y_M)]|
\leq(\lVert X_n\rVert_2+\lVert X\rVert_2)\lVert Y-Y_M\rVert_2.
$$

Letting first $n\to\infty$ and then $M\to\infty$ proves $\mathbb E[X_nY]\to\mathbb E[XY]$. Taking $Y=X$ and expanding the square now gives

$$
\mathbb E[(X_n-X)^2]
=\mathbb E[X_n^2]+\mathbb E[X^2]-2\mathbb E[X_nX]
\longrightarrow0.
$$

Consequently

$$
\boxed{X_n\longrightarrow X\text{ in }L^2.}
$$

This proves the [almost-sure convergence and convergence of second moments](../../../../../../../almost-sure-convergence-and-convergence-of-second-moments.md) criterion.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [26K](../../../26k.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
