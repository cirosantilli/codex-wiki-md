<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The integrand is an [entire function](../../../../../../entire-function.md), so the defining contour is immaterial. A rectangular contour, closed far to the right where the [Gaussian function](../../../../../../gaussian-function.md) decays, gives the exact horizontal-tail identity

$$
f(z)=\frac{\sqrt\pi}{2}-e^{-z^2}\int_0^\infty e^{-2zs-s^2}\,ds\qquad(\operatorname{Re}z\ge0).
$$

The constant is the half-line [Gaussian integral](../../../../../../gaussian-integral.md). Expand the endpoint amplitude $e^{-s^2}=1-s^2+\cdots$ in this [Watson lemma](../../../../../../watson-s-lemma.md). Alternatively, repeated [integration by parts](../../../../../../integration-by-parts.md) gives the same expansion, including purely imaginary $z$, because every derivative of $e^{-s^2}$ is integrable on the positive real axis. Thus, on each fixed ray in the stated quadrant,

$$
f(z)=\frac{\sqrt\pi}{2}-\frac{e^{-z^2}}{2z}\left(1-\frac1{2z^2}+O(|z|^{-4})\right).
$$

The remainder is measured on the exponential endpoint scale. When that scale grows, this formula does not resolve terms exponentially small relative to it.

Write $z=re^{i\theta}$. The endpoint term has modulus $e^{-r^2\cos2\theta}/(2r)$. For $0\le\theta<\pi/4$ it is exponentially small, and at $\theta=\pi/4$ it is oscillatory of order $r^{-1}$. For $\pi/4<\theta\le\pi/2$ it dominates the constant. The [quadrant asymptotics of the error function](../../../../../../quadrant-asymptotics-of-the-error-function.md) therefore give the requested leading [asymptotic expansions](../../../../../../asymptotic-expansion.md)

$$
\boxed{f(re^{i\theta})\sim\begin{cases}\sqrt\pi/2,&0\le\theta\le\pi/4,\\-e^{-r^2e^{2i\theta}}/(2re^{i\theta}),&\pi/4<\theta\le\pi/2.\end{cases}}
$$

The boundary ray $\theta=\pi/4$ belongs to the constant-dominated case because of the extra factor $1/r$. On the imaginary axis this gives $f(ir)\sim i e^{r^2}/(2r)$, consistent with $f(ir)=i\int_0^r e^{s^2}ds$. The constant/exponential dominance exchange is an [anti-Stokes line](../../../../../../anti-stokes-line.md) phenomenon; it should not be confused with dropping the constant everywhere in the quadrant.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
