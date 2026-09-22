<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $M=\sup|f|$ and $F_T(z)=\int_0^T f(t)e^{-tz}dt$. Each $F_T$ is an [entire function](../../../../../../entire-function.md): on any compact set of $z$, differentiation under this finite-interval integral is justified by a bounded integrable majorant. We prove $\boxed{F_T(0)\to F(0)}$, which gives ordinary convergence of the improper integral, not just an Abel limit.

Fix $R>0$. Since $\Omega$ contains the imaginary segment from $-iR$ to $iR$ and is open, choose $0<\delta<R$ so small that its closed left strip of width $\delta$ belongs to $\Omega$. Let $C_+$ be the right semicircle $|z|=R$ oriented from $-iR$ to $iR$, and let $\Gamma$ be the left half-ellipse $z=\delta\cos\theta+iR\sin\theta$, $\pi/2\le\theta\le3\pi/2$, oriented back to $-iR$. The enclosed right half-disk and thin left region lie in $\Omega$. The [residue theorem](../../../../../../residue-theorem.md), applied to the analytic difference with its simple pole at zero, gives

$$
F_T(0)-F(0)=\frac1{2\pi i}\int_{C_+\cup\Gamma}(F_T(z)-F(z))e^{Tz}\left(1+\frac{z^2}{R^2}\right)\frac{dz}{z}.
$$

For $x=\operatorname{Re}z>0$,

$$
|F_T(z)-F(z)|\le\int_T^\infty M e^{-tx}dt=\frac{M e^{-Tx}}x.
$$

On the right circle, $|1+z^2/R^2|=2x/R$ and $|z|=R$. The exponential cancels the displayed damping, so the absolute integrand per unit arc length is at most $2M/R^2$. The right-arc contribution is therefore at most $M/R$ after the factor $1/(2\pi)$.

For the $F_T$ term on $\Gamma$, deform that left path to the left semicircle $C_-$ of radius $R$. The [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) allows this because $F_T$ is an [entire function](../../../../../../entire-function.md) and the region between the paths excludes the pole at zero. On $C_-$, $x<0$ and

$$
|e^{Tz}F_T(z)|=\left|\int_0^T f(t)e^{(T-t)z}dt\right|\le\frac{M}{-x}.
$$

The same factor $|1+z^2/R^2|=2|x|/R$ bounds this contribution by $M/R$. The arc endpoints can be omitted from the estimates, since they have zero arc length and the integrands are continuous there.

Finally, the $F$ term on the original $\Gamma$ tends to zero as $T\to\infty$. This compact path stays away from zero, so $F(z)(1+z^2/R^2)/z$ is bounded there. Its interior has $\operatorname{Re}z<0$, hence $e^{Tz}\to0$, and $|e^{Tz}|\le1$. [Dominated convergence](../../../../../../dominated-convergence-theorem.md) on the finite-length path gives the claim. Combining the three pieces yields

$$
\limsup_{T\to\infty}|F_T(0)-F(0)|\le\frac{2M}{R}.
$$

Since $R$ is arbitrary, the difference tends to zero. This proves the [Newman Tauberian theorem](../../../../../../newman-tauberian-theorem.md) in the required setting; the proof crucially uses analytic continuation across every finite segment of the imaginary axis.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
