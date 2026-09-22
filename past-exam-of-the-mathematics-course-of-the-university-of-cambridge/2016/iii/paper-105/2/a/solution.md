<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an integer $s\geq0$, the [Sobolev space](../../../../../../sobolev-space-split.md) is

$$
W^{s,p}(\mathbb R^d)=\{u\in L^p:D^\beta u\in L^p\text{ for every multi-index }|\beta|\leq s\},
$$

where $D^\beta$ is a [weak derivative](../../../../../../weak-derivative.md). For $p<\infty$ one may use the [Sobolev norm](../../../../../../sobolev-norm.md) $(\sum_{|\beta|\leq s}\|D^\beta u\|_p^p)^{1/p}$; for $p=\infty$ use the maximum of the finitely many essential-supremum norms.

For $1\leq p<d$, the [Sobolev inequality](../../../../../../sobolev-inequality.md) is $\|u\|_{p^*}\leq C_{d,p}\|\nabla u\|_p$, with [Sobolev conjugate exponent](../../../../../../sobolev-conjugate-exponent.md) $p^*=dp/(d-p)$. For $d<p<\infty$, [Morrey's inequality](../../../../../../morrey-s-inequality.md) supplies a continuous representative satisfying

$$
|u(x)-u(y)|\leq C_{d,p}|x-y|^{1-d/p}\|\nabla u\|_p,
\qquad
\|u\|_\infty\leq C_{d,p}(\|u\|_p+\|\nabla u\|_p).
$$

At $p=\infty$ the representative is [Lipschitz continuous](../../../../../../lipschitz-continuity.md). At the critical exponent $p=d>1$, first-order Sobolev regularity gives every finite $L^q$ embedding for $q\geq d$, with an inhomogeneous norm, but generally no $L^\infty$ embedding. The one-dimensional endpoint $W^{1,1}(\mathbb R)\hookrightarrow L^\infty(\mathbb R)$ is an exception.

For the proof of [Morrey's inequality](../../../../../../morrey-s-inequality.md), start with a smooth $u$ and write $u_{B(x,r)}$ for its average on a ball. Averaging the [fundamental theorem of calculus along a line segment](../../../../../../fundamental-theorem-of-calculus-along-a-line-segment.md) and changing radial variables gives

$$
|u(x)-u_{B(x,r)}|
\leq C_d\int_{B(x,r)}\frac{|\nabla u(z)|}{|x-z|^{d-1}}\,dz
\leq C_{d,p}r^{1-d/p}\|\nabla u\|_p.
$$

The last step is the [Holder inequality](../../../../../../holder-inequality.md); integrability of the kernel to power $p'$ is exactly $(d-1)p'<d$. For $r=|x-y|$, translate the averaging ball along the segment from $x$ to $y$. The [fundamental theorem of calculus along a line segment](../../../../../../fundamental-theorem-of-calculus-along-a-line-segment.md) and the [Holder inequality](../../../../../../holder-inequality.md) give

$$
|u_{B(x,r)}-u_{B(y,r)}|\leq r|B_r|^{-1/p}\|\nabla u\|_p.
$$

Combining the two point-to-average bounds and this average-to-average bound proves the required Hölder estimate. The point-to-average bound with $r=1$, together with $|u_{B(x,1)}|\leq|B_1|^{-1/p}\|u\|_p$, gives the supremum estimate. [Density of smooth functions in a Sobolev space](../../../../../../density-of-smooth-functions-in-a-sobolev-space.md) then gives a uniformly convergent sequence of smooth representatives, preserving both bounds. For $p=\infty$, mollification gives the Lipschitz version.

For the decay conclusion assume $d<p<\infty$. The representative is uniformly continuous. If $|u(x_j)|\geq2\theta>0$ along points escaping to infinity, the Hölder bound gives a radius $\rho>0$, independent of $j$, on which $|u|\geq\theta$. A subsequence has disjoint radius-$\rho$ balls, each contributing at least $\theta^p|B_\rho|$ to $\|u\|_p^p$, a contradiction. This is [uniformly continuous integrable functions vanish at infinity](../../../../../../uniformly-continuous-integrable-functions-vanish-at-infinity.md).

**The finite-$p$ restriction is necessary.** If the printed range includes $p=\infty$, its decay assertion is false: $u\equiv1$ belongs to $W^{1,\infty}$ but does not tend to zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
