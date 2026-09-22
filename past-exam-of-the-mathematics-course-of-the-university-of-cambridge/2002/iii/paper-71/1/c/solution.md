<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For radial null propagation, $dr/\sqrt{1-kr^2}=|dt|/a$. Since $dz/dt=-(1+z)H(z)$ and $a=a_0/(1+z)$, its present-distance integral is

$$
\boxed{d_S=a_0\int_{t_e}^{t_0}\frac{dt}{a(t)}=\int_0^z\frac{dz'}{H(z')}}.
$$

Thus the printed extra $a_0$ before the [redshift](../../../../../../redshift.md) integral is inappropriate when $H$ is the physical [Hubble parameter](../../../../../../hubble-parameter.md); it disappears only if $a_0$ has been set to one.

Dust conservation and the [curvature](../../../../../../curvature.md) relation give

$$
H^2(z)=H_0^2[\Omega_0(1+z)^3+(1-\Omega_0)(1+z)^2],\qquad d_S=\frac1{H_0}\int_0^z\frac{dz'}{(1+z')\sqrt{1+\Omega_0z'}}.
$$

To evaluate it, put $s=\sqrt{1-\Omega_0}$ and $v=\sqrt{1+\Omega_0z}$. The dimensionless integral $I=H_0d_S$ is

$$
I=2\int_1^v\frac{dv'}{v'^2-s^2}=\frac1s\log\left[\frac{v-s}{v+s}\frac{1+s}{1-s}\right].
$$

Inverting the proper-distance expression in part b gives $r=\sinh(sI)/(a_0H_0s)$. Substituting the logarithm, writing the [hyperbolic sine](../../../../../../hyperbolic-sine.md) as half the difference of its exponential and inverse, and using $v^2-s^2=\Omega_0(1+z)$ yields

$$
\boxed{r(z)=\frac2{a_0H_0}\frac{\Omega_0z+(2-\Omega_0)[1-\sqrt{1+\Omega_0z}]}{\Omega_0^2(1+z)}}.
$$

This is the [open dust distance-redshift relation](../../../../../../open-dust-distance-redshift-relation.md). The printed square root lacks the factor $z$; its literal form would give a negative, nonzero coordinate at $z=0$. The corrected expression has $r\sim z/(a_0H_0)$ near zero. At fixed positive $\Omega_0$ and $z\gg\Omega_0^{-1}$, the term linear in $z$ dominates, giving

$$
\boxed{r\longrightarrow\frac2{a_0H_0\Omega_0}}.
$$

The zero-density limit is nonuniform: a pure Milne model has no such finite limiting radial coordinate.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
