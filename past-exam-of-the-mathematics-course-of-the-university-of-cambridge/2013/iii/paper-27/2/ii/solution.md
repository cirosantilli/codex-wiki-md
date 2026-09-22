<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a simple [Loewner trace](../../../../../../trace-of-a-loewner-chain.md), the domain mapped by $g_t$ is $D_t=\mathbb H\setminus\gamma[0,t]$. For a non-simple [Loewner trace](../../../../../../trace-of-a-loewner-chain.md), use instead the unbounded component $D_t=\mathbb H\setminus K_t$; the map $g_t$ is not defined on swallowed bounded components. This is the necessary domain interpretation when $\kappa>4$.

The function $\operatorname{Im}\log(g_t(z)-\xi_t)$ is [harmonic](../../../../../../harmonic-function.md) in $D_t$ because the logarithm is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) on the [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md). Let $S_t^-$ and $S_t^+$ be the intrinsic boundary sets mapped to $(-\infty,\xi_t)$ and $(\xi_t,\infty)$ respectively. The [Dirichlet problem](../../../../../../dirichlet-problem.md) has boundary data

$$
\boxed{h_t=\pi\text{ on }S_t^-,
\qquad h_t=0\text{ on }S_t^+.}
$$

For a simple [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) these are the left bank of the [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) together with the negative real boundary, and the right bank together with the positive real boundary. Left and right refer to the orientation from the starting point towards the tip. The tip and infinity correspond to discontinuities of the data; no unique limit is imposed there. They have zero [harmonic measure](../../../../../../harmonic-measure.md).

More precisely, the bounded solution is

$$
h_t(z)=\pi\,\omega_{D_t}(z,S_t^-),
$$

by the [Poisson kernel for the upper half-plane](../../../../../../poisson-kernel-for-the-upper-half-plane.md) and [conformal invariance of planar Brownian motion](../../../../../../conformal-invariance-of-planar-brownian-motion.md). This establishes the boundary values in the intrinsic sense and uniqueness among bounded solutions of the [Dirichlet problem](../../../../../../dirichlet-problem.md), without treating the two banks as one Euclidean boundary point.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
