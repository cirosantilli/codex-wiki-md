<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [nontangential limit](../../../../../nontangential-limit.md) at $\xi\in\partial\mathbb D$ restricts approach to a fixed [Stolz region](../../../../../stolz-region.md) $\Gamma_A(\xi)=\{z\in\mathbb D:|z-\xi|<A(1-|z|)\}$, where $A>1$. Radial approach is a special case. The [Fatou theorem for bounded holomorphic functions](../../../../../fatou-theorem-for-bounded-holomorphic-functions.md) says that every $f$ in [H-infinity space](../../../../../h-infinity-space.md) has a finite boundary value $f^*(\xi)$ for almost every $\xi$, with convergence through every fixed [Stolz region](../../../../../stolz-region.md) and $|f^*|\le\|f\|_\infty$ [almost everywhere](../../../../../almost-everywhere.md).

Here is a proof outline. Write $f=u+iv$ with bounded real [harmonic functions](../../../../../harmonic-function.md) $u,v$. Take a sequence $R_j\uparrow1$. The bounded functions $u(R_j\xi)$ have a subsequence converging in the [weak-star topology](../../../../../weak-star-topology.md) of $L^\infty(\partial\mathbb D)$ by the [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) and [weak-star metrizability of the dual ball](../../../../../weak-star-metrizability-of-the-dual-ball.md); its $L^1$ predual is [separable](../../../../../separable-topological-space.md). Denote the limit by $U$. For $|z|<R_j$, the [Poisson integral on the unit disk](../../../../../poisson-integral-on-the-unit-disk.md) gives

$$
u(z)=\int_{\partial\mathbb D}P_{z/R_j}(\xi)u(R_j\xi)\,dm(\xi).
$$

The [Poisson kernels](../../../../../poisson-kernel-for-the-upper-half-plane.md) converge uniformly for this fixed interior point and the boundary functions stay uniformly bounded, so the [weak-star topology](../../../../../weak-star-topology.md) permits passage to the limit:

$$
u(z)=\int_{\partial\mathbb D}\frac{1-|z|^2}{|\xi-z|^2}U(\xi)\,dm(\xi).
$$

Repeat for $v$, obtaining $V$. Thus $f$ is the [Poisson integral](../../../../../poisson-integral.md) of $F=U+iV\in L^\infty$.

The [Lebesgue differentiation theorem](../../../../../lebesgue-differentiation-theorem.md) makes almost every boundary point a [Lebesgue point](../../../../../lebesgue-point.md) of $U$ and $V$. The lemma that a [Poisson integral converges nontangentially at Lebesgue points](../../../../../poisson-integral-converges-nontangentially-at-lebesgue-points.md) then gives $f(z)\to F(\xi_0)$ in every fixed [Stolz region](../../../../../stolz-region.md). To see why, put $\delta=1-|z|$ and let $d(\xi,\xi_0)$ be the shorter angular distance. In $\Gamma_A(\xi_0)$ the kernel satisfies

$$
P_z(\xi)\le C_A\frac{\delta}{\delta^2+d(\xi,\xi_0)^2}.
$$

Split the circle into a central arc of radius comparable to $\delta$ and annuli with radii $2^k\delta$. For a [Lebesgue point](../../../../../lebesgue-point.md), averages of $|F-F(\xi_0)|$ on sufficiently small arcs are arbitrarily small. The annular contributions are bounded by these averages times a summable geometric sequence $C_A2^{-k}$. On the remaining fixed distant arc the kernel is $O(\delta)$, so its contribution vanishes. This proves the claimed [nontangential limit](../../../../../nontangential-limit.md). The same [Lebesgue points](../../../../../lebesgue-point.md) work for every integer aperture $A\ge2$, hence for all finite apertures.

These boundary values recover the interior by the [Poisson integral](../../../../../poisson-integral.md), so they determine $f$ uniquely. They satisfy $\|f^*\|_{L^\infty}=\|f\|_\infty$: one inequality follows by taking limits of the bounded interior values, and the other from positivity and unit integral of the [Poisson kernel](../../../../../poisson-kernel-for-the-upper-half-plane.md). The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) also gives $f(r\xi)\to f^*(\xi)$ in every finite $L^p$ norm. Its negative [Fourier coefficients](../../../../../fourier-coefficient.md) vanish, because the [Taylor series](../../../../../taylor-series.md) of $f$ has only nonnegative powers. This explains the boundary realization of analytic [Hardy spaces](../../../../../hardy-space.md).

The exceptional set cannot generally be removed. For example, $f(z)=\exp(i\operatorname{Log}(1-z))$ is bounded and [holomorphic](../../../../../complex-differentiability-at-a-point.md) on the [unit disc](../../../../../unit-disc.md), using the [holomorphic logarithm](../../../../../holomorphic-logarithm.md) on the right half-plane: $|f(z)|=e^{-\arg(1-z)}$ lies between $e^{-\pi/2}$ and $e^{\pi/2}$. At the boundary point one its radial values $e^{i\log(1-r)}$ oscillate without a limit. Nor does the theorem assert convergence along arbitrary tangential paths or a continuous boundary extension. Its strength is almost-everywhere control on every fixed approach cone.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
