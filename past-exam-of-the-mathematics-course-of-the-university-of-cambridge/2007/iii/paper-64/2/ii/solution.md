<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $w=c_s^2$ be constant and small, and write $\theta=i\mathbf k\cdot\mathbf v$. The supplied [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md) equations imply

$$
\delta'=-(1+w)(\theta+h'/2),\qquad
\theta'+(1-3w)\mathcal H\theta-\frac{w}{1+w}k^2\delta=0.
$$

Differentiating the first and eliminating $\theta$ gives

$$
\delta''+(1-3w)\mathcal H\delta'+wk^2\delta
=-\frac{1+w}2\left[h''+(1-3w)\mathcal Hh'\right].
$$

For the dominant single component, the Einstein equation gives $h''+\mathcal Hh'=-3\mathcal H^2(1+3w)\delta$. Therefore the exact algebraic intermediate relation is

$$
\delta''+(1-3w)\mathcal H\delta'
+\left[wk^2-\frac32(1+w)(1+3w)\mathcal H^2\right]\delta
=\frac32w(1+w)\mathcal Hh'.
$$

The requested [nonrelativistic density equation in synchronous gauge](../../../../../../nonrelativistic-density-equation-in-synchronous-gauge.md) follows to leading nonrelativistic order: discard [pressure](../../../../../../pressure.md) corrections to the background, Hubble damping, and [metric tensor](../../../../../../metric-tensor.md) terms while retaining $c_s^2k^2\delta$, which can be comparable to gravity at the [Jeans wavenumber](../../../../../../jeans-wavenumber.md). Since $w\ll1$, that scale lies well inside the [Hubble radius](../../../../../../hubble-radius.md), so keeping its enhanced gradient term is consistent. The resulting equation is

$$
\delta''+\mathcal H\delta'+(c_s^2k^2-4\pi Ga^2\bar\rho_m)\delta=0,
$$

where the [Friedmann equation](../../../../../../friedmann-equations.md) gave $3\mathcal H^2/2=4\pi Ga^2\bar\rho_m$. Now $\delta'=a\dot\delta$ and $\delta''=a^2(\ddot\delta+H\dot\delta)$, so

$$
\boxed{\ddot\delta+2H\dot\delta-
\left(4\pi G\bar\rho_m-\frac{c_s^2k^2}{a^2}\right)\delta=0.}
$$

This is the specified approximation, not an exact finite-$w$ relativistic identity. The pressure-gradient term stabilizes short wavelengths, while gravity drives the long-wavelength [Jeans instability](../../../../../../jeans-instability.md).

Now apply the stipulated equation to $P=K\rho^{4/3}$ with $K>0$. In the pressure-negligible matter background,

$$
a\propto t^{2/3},\qquad \bar\rho_m=\frac1{6\pi Gt^2},\qquad
c_s^2=\frac43K\bar\rho_m^{1/3}\propto t^{-2/3}\propto a^{-1}.
$$

Thus $c_s^2k^2/a^2$ is proportional to $t^{-2}$, exactly like the gravitational term. Define

$$
k_J^2=\frac{4\pi G\bar\rho_m a^2}{c_s^2},\qquad
q=\frac{k^2}{k_J^2}.
$$

The comoving [Jeans wavenumber](../../../../../../jeans-wavenumber.md) and $q$ are constant in this era. The equation becomes the [Euler-Cauchy equation](../../../../../../euler-cauchy-equation.md)

$$
\ddot\delta+\frac4{3t}\dot\delta+\frac{2(q-1)}{3t^2}\delta=0.
$$

Setting $\delta\propto t^p$ gives $p^2+p/3+2(q-1)/3=0$. For distinct real roots the full pair of modes is

$$
\boxed{\delta(t)=A\left(\frac t{t_*}\right)^{p_+}
+B\left(\frac t{t_*}\right)^{p_-},\qquad
p_\pm=\frac{-1\pm\sqrt{25-24q}}6.}
$$

These are the [Jeans modes of a four-thirds polytropic cosmological fluid](../../../../../../jeans-modes-of-a-four-thirds-polytropic-cosmological-fluid.md). The physical [Jeans length](../../../../../../jeans-length.md) is

$$
\boxed{\lambda_J=\frac{2\pi a}{k_J}
=c_s\sqrt{\frac\pi{G\bar\rho_m}},\qquad
q=\left(\frac{\lambda_J}{\lambda}\right)^2,
\quad\lambda=\frac{2\pi a}{k}.}
$$

Here $\lambda_J\propto a$, so its comoving value is constant. For $\lambda>\lambda_J$, $q<1$ and $p_+>0$, giving genuine growth; the other solution decays. In the long-wavelength pressure-free limit, $p_+=2/3$ and $p_-=-1$, the familiar matter-era modes. At $\lambda=\lambda_J$, the two powers are $0$ and $-1/3$, so the leading mode is constant rather than growing.

For $1<q<25/24$ both powers are negative: [pressure](../../../../../../pressure.md) prevents growth, although the modes still decay without oscillation. At $q=25/24$ they coincide and the complete solution is

$$
\delta=t^{-1/6}\left[A+B\ln(t/t_*)\right].
$$

For $q>25/24$ they become a complex-conjugate pair; a real basis is

$$
\boxed{\delta=t^{-1/6}\left[A\cos\bigl(\omega\ln(t/t_*)\bigr)
+B\sin\bigl(\omega\ln(t/t_*)\bigr)\right],\qquad
\omega=\frac{\sqrt{24q-25}}6.}
$$

These short-wavelength acoustic oscillations have a decaying envelope. The onset of instability is $q=1$, while the threshold for oscillatory time dependence is slightly larger, $q=25/24$; expansion damping explains why these two thresholds are not identical.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
