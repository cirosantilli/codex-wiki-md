<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a continuous boundary function $g(e^{i\theta})$, its [Poisson integral on the unit disk](../../../../../poisson-integral-on-the-unit-disk.md) is

$$
V(z)=\frac1{2\pi}\int_0^{2\pi}g(e^{i\theta})\frac{1-|z|^2}{|e^{i\theta}-z|^2}\,d\theta,\qquad |z|<1.
$$

The kernel is the real part of the [holomorphic function](../../../../../holomorphic-function.md) $(e^{i\theta}+z)/(e^{i\theta}-z)$, so differentiation under the integral on compact subsets shows that $V$ is harmonic. The kernel is positive and has integral $2\pi$: expand the holomorphic fraction as $1+2\sum_{n\geq1}z^ne^{-in\theta}$ and integrate. As $z$ approaches a boundary point, the mass outside any fixed arc around that point tends to zero. Uniform continuity of $g$ therefore shows that $V$ extends continuously with boundary values $g$.

Apply this with $g=u|_{\partial\mathbb D}$. The [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md) applied to the harmonic difference $u-V$, which vanishes on the boundary, gives

$$
\boxed{u(z)=\frac1{2\pi}\int_0^{2\pi}u(e^{i\theta})\frac{1-|z|^2}{|e^{i\theta}-z|^2}\,d\theta.}
$$

At boundary points the formula is understood through its continuous interior limit.

Now suppose a continuous function has the [mean value property](../../../../../mean-value-property-for-harmonic-functions.md) and has a local maximum $M=u(z)$ at $z$. Shrink the neighborhood so that $u\leq M$ there and all sufficiently small centered circles satisfy the [mean value property](../../../../../mean-value-property-for-harmonic-functions.md). On each such circle the average is $M$. If one value were smaller than $M$, continuity would make it smaller on an arc of positive length, contradicting this average. Thus every sufficiently small circle, and hence an entire neighborhood of $z$, has value $M$.

A [harmonic function](../../../../../harmonic-function.md) has the [mean value property](../../../../../mean-value-property-for-harmonic-functions.md). Indeed, if $m(r)$ is its average on a circle centered at $z$, the [divergence theorem](../../../../../divergence-theorem.md) gives

$$
m'(r)=\frac1{2\pi r}\int_{|w-z|<r}\Delta u(w)\,dA(w)=0.
$$

As $r\downarrow0$, $m(r)\to u(z)$, giving the asserted equality.

Conversely, suppose $u$ is continuous and has the [mean value property](../../../../../mean-value-property-for-harmonic-functions.md). On an arbitrary closed disk compactly contained in its domain, form the harmonic [Poisson integral](../../../../../poisson-integral.md) $V$ with boundary values $u$. The difference $w=u-V$ is continuous, has the [mean value property](../../../../../mean-value-property-for-harmonic-functions.md), and vanishes on the boundary. If its maximum were positive, it would be attained inside. The set attaining that maximum is relatively closed and, by the local argument already proved, relatively open. [Connectedness](../../../../../connected-space.md) of the disk makes $w$ constant, contradicting its boundary value. Thus $w\leq0$. Applying the same argument to $-w$ gives $w\geq0$. Therefore $u=V$ on every such disk, proving

$$
\boxed{u\text{ has the mean value property}\ \Longleftrightarrow\ u\text{ is harmonic}.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
