<h1 id="27k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here $\Lambda$ is planar [Lebesgue measure](../../../../../../lebesgue-measure.md). For a Borel set $B\subseteq[0,\infty)$, [polar coordinates](../../../../../../polar-coordinates.md) give

$$
\begin{aligned}
f_*\Lambda(B)
&=\int_{\mathbb R^2}\mathbf1_B(x_1^2+x_2^2)\,dx_1\,dx_2\\
&=\int_0^{2\pi}\int_0^\infty\mathbf1_B(r^2)r\,dr\,d\theta\\
&=\pi\int_Bdt.
\end{aligned}
$$

The pushforward is therefore locally finite and atomless. By the [mapping theorem for Poisson point processes](../../../../../../mapping-theorem-point-process.md), $f(\Pi)$ is a homogeneous [Poisson process](../../../../../../poisson-process.md) on $[0,\infty)$ with **constant intensity $\pi$**. This is the two-dimensional [radial volume transform of a homogeneous Poisson point process](../../../../../../radial-volume-transform-of-a-homogeneous-poisson-point-process.md).

Put $S_k=R_k^2$. The variable $S_k$ is the $k$th arrival time of that rate-$\pi$ Poisson process, hence has the [gamma distribution](../../../../../../gamma-distribution.md) with shape $k$ and rate $\pi$:

$$
g_k(s)=\frac{\pi^k}{(k-1)!}s^{k-1}e^{-\pi s},
\qquad s>0.
$$

Since $s=r^2$ and $ds/dr=2r$, the [change-of-variables formula for a probability density](../../../../../../change-of-variables-formula-for-a-probability-density.md) gives the [Kth-nearest-neighbour distance in a homogeneous Poisson point process](../../../../../../kth-nearest-neighbour-distance-in-a-homogeneous-poisson-point-process.md)

$$
\boxed{h_k(r)=2r\,g_k(r^2)
=\frac{2\pi r(\pi r^2)^{k-1}e^{-\pi r^2}}{(k-1)!},
\qquad r>0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27K](../../27k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
