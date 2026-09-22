<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Within each constant-conductivity region the [temperature](../../../../../../temperature.md) is [harmonic](../../../../../../harmonic-function.md). For $u=v(r)\cos\theta$, the spherical Laplacian gives

$$
\Delta u=\left(v''+\frac2rv'-\frac2{r^2}v\right)\cos\theta.
$$

Trying $v=r^s$ yields $s(s-1)+2s-2=(s-1)(s+2)=0$. Thus $v=Cr+Dr^{-2}$. Boundedness at the origin removes the interior $r^{-2}$ term, while the prescribed far [gradient](../../../../../../gradient.md) fixes the exterior growing term:

$$
u_{\mathrm{in}}=C_{\mathrm{in}}r\cos\theta,\qquad
u_{\mathrm{out}}=(r+Br^{-2})\cos\theta.
$$

Continuity of [temperature](../../../../../../temperature.md) and normal flux at $r=r_1$ give

$$
C_{\mathrm{in}}=1+\frac{B}{r_1^3},\qquad
a_1C_{\mathrm{in}}=a_0\left(1-\frac{2B}{r_1^3}\right).
$$

Solving these two equations yields $B=-r_1^3(a_1-a_0)/(a_1+2a_0)$ and $C_{\mathrm{in}}=3a_0/(a_1+2a_0)$. Consequently

$$
\boxed{
u_{\mathrm{out}}=x_3-\frac{r_1^3(a_1-a_0)}{a_1+2a_0}\frac{x_3}{|x|^3},
\qquad
u_{\mathrm{in}}=\frac{3a_0}{a_1+2a_0}x_3.
}
$$

Positive conductivities make the denominator nonzero. The matched solution is unique in the usual finite-energy decaying-perturbation class: the difference of two solutions has zero far data and interface jumps, and an energy integration gives zero [gradient](../../../../../../gradient.md).

For the [polarization field of a conductivity inclusion](../../../../../../polarization-field-of-a-conductivity-inclusion.md), use the sign convention consistent with the perturbation equation:

$$
P=(a-a_0I)\nabla u,\qquad
\beta=\frac{3a_0(a_1-a_0)}{a_1+2a_0}.
$$

Thus

$$
\boxed{P(x)=\beta\,\chi_B(x)e_3.}
$$

For a general incident constant [gradient](../../../../../../gradient.md) $E$, rotational [symmetry](../../../../../../symmetry-physics.md) and [linearity](../../../../../../linearity.md) replace $e_3$ by $E$. The polarization vanishes outside the [sphere](../../../../../../sphere.md) because its local conductivity equals the reference value. The [temperature](../../../../../../temperature.md) perturbation outside is dipolar; this is the [spherical conductivity inclusion](../../../../../../spherical-conductivity-inclusion.md) response used in the remaining parts.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
