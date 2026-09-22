<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

The [Cauchy integral formula](../../../../../cauchy-integral-formula.md) says that if $f$ is [holomorphic](../../../../../holomorphic-function.md) on a neighbourhood of the closed disc $\overline{D(z_0;R)}$, then for $z\in D(z_0;R)$,

$$
f(z)=\frac1{2\pi i}\int_{|\zeta-z_0|=R}\frac{f(\zeta)}{\zeta-z}\,d\zeta.
$$

In particular, at the centre,

$$
f(z_0)=\frac1{2\pi}\int_0^{2\pi}f(z_0+re^{i\theta})\,d\theta
$$

for every $0<r<R$.

If $f(z_0)=0$, the assumed bound gives $|f(z)|\leq0$, so $f=0$. Otherwise define $g=f/f(z_0)$. Then $g(z_0)=1$ and $|g|\leq1$. Applying the centre formula and taking [real parts](../../../../../real-part.md) gives

$$
1=\frac1{2\pi}\int_0^{2\pi}\operatorname{Re}g(z_0+re^{i\theta})\,d\theta,
\qquad \operatorname{Re}g\leq|g|\leq1.
$$

The continuous nonnegative function $1-\operatorname{Re}g$ has integral zero, so it vanishes around the circle. Equality $\operatorname{Re}g=1$ together with $|g|\leq1$ forces $g=1$. This holds for every $r<R$, hence $f(z)=f(z_0)$ throughout the disc. This is the equality case underlying the [maximum modulus principle](../../../../../maximum-modulus-principle.md).

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
