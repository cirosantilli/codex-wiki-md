<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [spherical Abel deprojection](../../../../../../spherical-abel-deprojection.md), put $A_r=r^2+b^2$ and $s=(R^2+b^2)/A_r$. Then $dR^2=A_r\,ds$ and $\sqrt{R^2-r^2}=A_r^{1/2}\sqrt{s-1}$. Consequently the integral appearing in the reconstruction of $n$ is

$$
J_n(r)=N_0b^5 A_r^{-2}I_{5/2},\qquad
I_\alpha=\int_1^\infty s^{-\alpha}(s-1)^{-1/2}\,ds.
$$

Differentiate before substituting the numerical value of $I_{5/2}$:

$$
n(r)=-\frac{J_n'(r)}{2\pi r}=\frac{2N_0b^5}{\pi A_r^3}I_{5/2}
=\boxed{\frac{8N_0b^5}{3\pi(r^2+b^2)^3}.}
$$

For the projected second [stellar velocity moment](../../../../../../stellar-velocity-moment.md), $N\sigma^2=N_0\sigma_0^2b^6(R^2+b^2)^{-3}$. The identical substitution in [isotropic stellar pressure deprojection](../../../../../../isotropic-stellar-pressure-deprojection.md) gives

$$
J_p=N_0\sigma_0^2b^6A_r^{-5/2}I_3,\qquad
p(r)=\frac{5N_0\sigma_0^2b^6}{2\pi A_r^{7/2}}I_3
=\boxed{\frac{15N_0\sigma_0^2b^6}{16(r^2+b^2)^{7/2}}.}
$$

For completeness, setting $t=1/s$ yields $I_\alpha=B(1/2,\alpha-1/2)$, where $B$ is the [Euler beta function](../../../../../../beta-function.md). The [Gamma function recurrence](../../../../../../gamma-function-recurrence.md) gives $I_{5/2}=4/3$ and $I_3=3\pi/8$. This also checks the normalization of the [power-law spherical projection kernel](../../../../../../power-law-spherical-projection-kernel.md).

The radial [Jeans equation](../../../../../../jeans-equation.md) is $p'=n\psi'$. Since $p'=-105N_0\sigma_0^2b^6r/(16A_r^{9/2})$, division by the tracer [number density](../../../../../../number-density.md) gives

$$
\psi'(r)=-\frac{315\pi}{128}\frac{\sigma_0^2br}{(r^2+b^2)^{3/2}}.
$$

Writing $A=315\pi\sigma_0^2b/128$, the total [gravitational acceleration](../../../../../../gravitational-acceleration.md) is therefore

$$
\boxed{\nabla\psi=-\frac{A\mathbf r}{(r^2+b^2)^{3/2}}.}
$$

To find all gravitating [mass density](../../../../../../density.md), apply the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md), with the same sign convention:

$$
\rho_{\rm tot}(r)=-\frac1{4\pi G r^2}\frac d{dr}(r^2\psi')
=\frac{3Ab^2}{4\pi G(r^2+b^2)^{5/2}}
=\boxed{\frac{945\sigma_0^2b^3}{512G(r^2+b^2)^{5/2}}.}
$$

Equivalently, the enclosed [mass](../../../../../../mass.md) is $M(r)=Ar^3/[G(r^2+b^2)^{3/2}]$, and $\rho_{\rm tot}=M'/(4\pi r^2)$. The inferred total [mass](../../../../../../mass.md) is $A/G$ and its [relative potential](../../../../../../relative-potential.md) is $A/\sqrt{r^2+b^2}$, a [Plummer model](../../../../../../plummer-model.md). The tracer [number density](../../../../../../number-density.md) has a different radial exponent from this total [mass density](../../../../../../density.md). One must not multiply $n$ by an arbitrary stellar mass and identify it with all matter: the inferred field can include unobserved [stars](../../../../../../star.md), gas, and [dark matter](../../../../../../dark-matter.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
