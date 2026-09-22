<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With constant permeability, the electric equation reduces to $(\partial_x^2+\partial_z^2+k^2(z))E_y=0$. Insert the oblique-wave dependence $E_y=e_y(z)e^{-ik_0\sin\theta_0x}$ and set $s=z-z_0$. The [inverse-square refractive-index profile](../../../../../../inverse-square-refractive-index-profile.md) gives

$$
e_y''+\left[\beta^2-\frac{\nu^2-1/4}{s^2}\right]e_y=0,
\qquad \beta^2=k_0^2(a^2-\sin^2\theta_0),
\qquad \nu^2=\frac14+k_0^2b^2.
$$

Substituting $e_y=\sqrt{|s|}\,w(\beta|s|)$ gives the [Bessel equation](../../../../../../bessel-differential-equation.md) of order $\nu$. On either side of the profile singularity, when $\beta^2>0$,

$$
\boxed{e_y(z)=\sqrt{|z-z_0|}\left[A J_\nu(\beta|z-z_0|)+B Y_\nu(\beta|z-z_0|)\right].}
$$

Equivalently use [Hankel functions](../../../../../../hankel-function.md) for an incoming/outgoing wave basis. If $\beta^2<0$, write $\gamma=\sqrt{-\beta^2}$ and replace $J_\nu,Y_\nu$ by [modified Bessel functions](../../../../../../modified-bessel-function.md) $I_\nu,K_\nu$ with argument $\gamma|s|$. For $\beta=0$, the solutions are $|s|^{1/2+\nu}$ and $|s|^{1/2-\nu}$, with a logarithmic second solution in the repeated-root case $\nu=0$. The constants on each side require incident-wave and boundary or matching data; the supplied singular profile alone does not choose them.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
