<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

Fix $R>|z|$. The [Cauchy integral formula](../../../../../cauchy-integral-formula.md) and the uniformly convergent geometric series on $|\zeta|=R$ give

$$
f(z)=\frac1{2\pi i}\int_{|\zeta|=R}\frac{f(\zeta)}{\zeta-z}\,d\zeta
=\sum_{n=0}^{\infty}z^n\frac1{2\pi i}\int_{|\zeta|=R}\frac{f(\zeta)}{\zeta^{n+1}}\,d\zeta.
$$

Defining

$$
c_j=\frac1{2\pi i}\int_{|\zeta|=R}\frac{f(\zeta)}{\zeta^{j+1}}\,d\zeta,
$$

the remainder after degree $N$ has modulus at most $M_R(|z|/R)^{N+1}/(1-|z|/R)$, which tends to zero uniformly on each smaller disk. Differentiating the integral formula at zero identifies $c_j=f^{(j)}(0)/j!$, independently of $R$. Since $f$ is an [entire function](../../../../../entire-function.md), $R$ can be chosen larger than any given $|z|$, proving the global [Taylor series](../../../../../taylor-series.md).

For the requested radius $r$, the same coefficient integral gives the [Cauchy estimate](../../../../../cauchy-estimate.md)

$$
\boxed{|c_n|\le\frac{M_r}{r^n}.}
$$

To characterize [equality in the Cauchy coefficient estimate](../../../../../equality-in-the-cauchy-coefficient-estimate.md), parametrize its circle:

$$
r^nc_n=\frac1{2\pi}\int_0^{2\pi}f(re^{i\theta})e^{-in\theta}\,d\theta.
$$

If $M_r=0$, the [identity theorem](../../../../../identity-theorem.md) gives $f=0$. Otherwise equality in the modulus bound requires the continuous integrand to have both constant modulus $M_r$ and constant complex argument. To see this directly, rotate its average to the positive real axis: its real part is bounded above by $M_r$, and equality of its average with $M_r$ forces that real part to equal $M_r$ everywhere. Thus $f(re^{i\theta})=c_nr^ne^{in\theta}$ on the circle. The [identity theorem](../../../../../identity-theorem.md) extends that equality to the plane. Conversely every such monomial attains the bound. Therefore

$$
\boxed{\text{equality holds exactly for }f(z)=cz^n,\quad c\in\mathbb C,}
$$

including the zero function and, when $n=0$, arbitrary constant functions.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
