<h1 id="section-c/c13/solution">Solution</h1>

↑ **Parent:** [C13](../c13.md)

**Constitutive law and Poisson ratio.** Use positive [stress](../../../../../stress.md) for tension. In an isotropic linearly elastic medium, [Hooke's law](../../../../../hooke-s-law.md) gives

$$
\boxed{e_1=\frac{\tau_1-\sigma(\tau_2+\tau_3)}E.}
$$

The analogous equations follow by cyclic permutation. Under uniaxial tension in direction 1, $e_1=\tau_1/E$ and $e_2=e_3=-\sigma\tau_1/E$. Thus [Poisson's ratio](../../../../../poisson-s-ratio.md) $\sigma=-e_2/e_1$ measures transverse contraction relative to longitudinal extension when the transverse stresses are zero. It is dimensionless; it is not the ratio of transverse [stress](../../../../../stress.md) to longitudinal [stress](../../../../../stress.md).

**Radial and hoop strains.** Let a material point originally at radius $r$ move to $r+R(r)$, with small axisymmetric displacement. Two neighbouring radii separated by $dr$ move apart by $dr+dR$, so the radial fractional extension is $dR/dr$. A circle's circumference changes from $2\pi r$ to $2\pi(r+R)$, so its fractional extension is $R/r$. Consequently

$$
\boxed{e_r=R'(r),\qquad e_\phi=\frac{R(r)}r.}
$$

The absence of longitudinal [stress](../../../../../stress.md) is a [plane stress](../../../../../plane-stress.md) condition, not a claim of zero longitudinal [strain](../../../../../strain.md).

**Equilibrium of an annular wedge.** Consider a slice of unit axial length, radial thickness $dr$ and small angular width $d\phi$. The difference of the outward and inward radial face forces is $(r\tau_r)'dr\,d\phi$ to leading order. The two tangential face tensions have inward radial resultant $\tau_\phi dr\,d\phi$: each contributes $\tau_\phi dr\sin(d\phi/2)$. With no body [force](../../../../../force-split.md), their balance gives the [radial equilibrium of a thick elastic cylinder](../../../../../radial-equilibrium-of-a-thick-elastic-cylinder.md),

$$
\boxed{\tau_\phi=\frac d{dr}(r\tau_r)
=\tau_r+r\tau_r'.}
$$

This hoop contribution is why the radial [stress](../../../../../stress.md) need not be spatially constant in a thick wall.

**Displacement equation.** With $\tau_z=0$, the two [Hooke's law](../../../../../hooke-s-law.md) equations read

$$
R'=\frac{\tau_r-\sigma\tau_\phi}E,\qquad
\frac Rr=\frac{\tau_\phi-\sigma\tau_r}E.
$$

Invert them:

$$
\tau_r=\frac E{1-\sigma^2}\left(R'+\sigma\frac Rr\right),\qquad
\tau_\phi=\frac E{1-\sigma^2}\left(\frac Rr+\sigma R'\right).
$$

Substitute in $\tau_\phi=(r\tau_r)'$. After cancelling the common factor, the right-hand side is $rR''+(1+\sigma)R'$, so

$$
\frac Rr+\sigma R'=rR''+(1+\sigma)R',
\qquad
\boxed{r^2R''+rR'-R=0.}
$$

The cancellation explains why this displacement equation does not depend on the value of [Poisson's ratio](../../../../../poisson-s-ratio.md).

**Power laws and wall pressure.** Try $R\propto r^n$. The indicial equation is $n(n-1)+n-1=n^2-1=0$, so

$$
R=c_1r+\frac{c_2}r.
$$

The resulting [Lamé stress distribution in a pressurized cylindrical wall](../../../../../lame-stress-distribution-in-a-pressurized-cylindrical-wall.md) can be written

$$
\tau_r=P-\frac Q{r^2},\qquad
\tau_\phi=P+\frac Q{r^2},
\quad P=\frac{Ec_1}{1-\sigma},\quad Q=\frac{Ec_2}{1+\sigma}.
$$

The [pressure](../../../../../pressure-split.md) boundary tractions are $\tau_r(a)=-p_1$ and $\tau_r(b)=-p_0$. Solving them yields

$$
P=\frac{p_1a^2-p_0b^2}{b^2-a^2},\qquad
Q=\frac{(p_1-p_0)a^2b^2}{b^2-a^2}.
$$

Hence the positive compressive radial [pressure](../../../../../pressure-split.md) in the wall is

$$
\boxed{p(r)=-\tau_r(r)=
\frac{p_0b^2-p_1a^2+(p_1-p_0)a^2b^2/r^2}{b^2-a^2},
\qquad a\leq r\leq b.}
$$

It equals $p_1$ at $a$ and $p_0$ at $b$. This directional radial [pressure](../../../../../pressure-split.md) is not an isotropic fluid [pressure](../../../../../pressure-split.md): radial and tangential stresses differ. The associated displacement is $R=[(1-\sigma)Pr+(1+\sigma)Q/r]/E$. Also $e_z=-\sigma(\tau_r+\tau_\phi)/E=-2\sigma P/E$, generally nonzero even though $\tau_z=0$.

**Maximum absolute tangential stress.** For $p_1>p_0$, $Q>0$ and $\tau_\phi'= -2Q/r^3<0$. Therefore the maximum of its absolute value must be at one of the two surfaces. Keeping the specified external [pressure](../../../../../pressure-split.md) gives the fully general answer

$$
\boxed{\max_{a\leq r\leq b}|\tau_\phi(r)|
=\frac1{b^2-a^2}\max\left\{
\left|p_1(a^2+b^2)-2p_0b^2\right|,
\left|2p_1a^2-p_0(a^2+b^2)\right|
\right\}.}
$$

For the usual high internal [pressure](../../../../../pressure-split.md) with negligible external [pressure](../../../../../pressure-split.md), the largest magnitude is the tensile [stress](../../../../../stress.md) on the inner wall:

$$
\boxed{\tau_{\phi,\max}\simeq\tau_\phi(a)
=\frac{p_1(a^2+b^2)}{b^2-a^2}\quad(p_0\simeq0).}
$$

For finite $p_0$, the inner-wall expression is $[p_1(a^2+b^2)-2p_0b^2]/(b^2-a^2)$, but its absolute value is not always the larger endpoint value. For example, nearly equal internal and external pressures can leave the outer surface more compressive. With $p_1=p_0=p$, both stresses correctly reduce to $-p$ everywhere. These results use a homogeneous linear elastic wall without axial loading; a closed-ended pipe would require a different longitudinal-[stress](../../../../../stress.md) condition.

## ↑ Ancestors (14)

1. [C13](../c13.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
