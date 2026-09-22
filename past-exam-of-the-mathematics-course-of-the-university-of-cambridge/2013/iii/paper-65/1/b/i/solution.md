<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the nonrotating linear [Boussinesq approximation](../../../../../../../boussinesq-approximation.md) with reference density $\rho_0$ and $N^2=-(g/\rho_0)d\bar\rho/dz>0$:

$$
\partial_tu'=-\frac{\partial_xp'}{\rho_0},\quad
\partial_tv'=-\frac{\partial_yp'}{\rho_0},\quad
\partial_tw'=-\frac{\partial_zp'}{\rho_0}-\frac{g\rho'}{\rho_0},\quad
\partial_t\rho'+w'\bar\rho_z=0,\quad
\nabla\cdot\mathbf u'=0.
$$

Let $K_h^2=k^2+l^2>0$, $K^2=K_h^2+m^2$ and $E=e^{i(kx+ly+mz-\omega t)}$. The horizontal momentum equations give $u'=kp'/(\rho_0\omega)$ and $v'=lp'/(\rho_0\omega)$. Continuity requires $ku'+lv'+mw'=0$. Thus the [internal-wave polarization](../../../../../../../internal-wave-polarization.md) is

$$
\boxed{u'=-\frac{km}{K_h^2}w_0E,\qquad
v'=-\frac{lm}{K_h^2}w_0E,\qquad
p'=-\frac{\rho_0\omega m}{K_h^2}w_0E,\qquad
\rho'=i\frac{\rho_0N^2}{g\omega}w_0E.}
$$

Physical perturbations are the real parts. The density is in temporal quadrature with the vertical velocity, because buoyancy responds to the vertical [fluid displacement](../../../../../../../lagrangian-displacement-fluid-mechanics.md). Substitution into the vertical momentum equation determines the [internal gravity wave](../../../../../../../internal-wave.md) [dispersion relation](../../../../../../../dispersion-relation.md),

$$
\boxed{\omega^2=N^2\frac{K_h^2}{K^2}.}
$$

A nontrivial propagating wave requires a nonzero horizontal [wave vector](../../../../../../../wavevector.md) and a nonzero frequency. The formulas are not to be divided by $K_h^2=0$: incompressibility excludes a nonzero oscillatory vertical velocity for a purely vertical [wave vector](../../../../../../../wavevector.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 65](../../../../paper-65-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
