<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a static equilibrium, [linearization](../../../../linearization.md) of magnetic induction gives

$$
\delta\mathbf B=\nabla\times(\boldsymbol\xi\times\mathbf B_0)
=(\mathbf B_0\cdot\nabla)\boldsymbol\xi-(\boldsymbol\xi\cdot\nabla)\mathbf B_0-\mathbf B_0\nabla\cdot\boldsymbol\xi.
$$

The rotating local basis must be differentiated. In particular, $\partial_\parallel\hat{\mathbf x}=\mathbf b_0/R$ and $\partial_\parallel\mathbf b_0=-\hat{\mathbf x}/R$. Their contributions proportional to $\xi_\parallel$ cancel in the radial component, yielding

$$
\boxed{\delta b_x=ik_\parallel\xi_x,\qquad\delta b_y=ik_\parallel\xi_y.}
$$

Writing $h=\delta B/B_0$, the magnitude component is

$$
h=ik_\parallel\xi_\parallel+\frac{\xi_x}{R}+\frac{\xi_x}{L_B}-\nabla\cdot\boldsymbol\xi
=\frac{\xi_x}{L_B}-ik_y\xi_y,
$$

where $\nabla\cdot\boldsymbol\xi=\xi_x/R+ik_y\xi_y+ik_\parallel\xi_\parallel$ when $\partial_x\xi_x=0$.

Set $M=B_0^2/(4\pi)=\rho_0v_A^2$ and $\delta\Pi=\delta p_\perp+Mh$. The transverse $y$ component of the linear [kinetic magnetohydrodynamic momentum equation](../../../../kinetic-magnetohydrodynamic-momentum-equation.md) is

$$
\rho_0(\omega^2-k_\parallel^2v_A^2)\xi_y=ik_y\delta\Pi.
$$

Since $k_y\gg k_\parallel\sim\omega/v_A$, perpendicular [magnetic pressure](../../../../magnetic-pressure.md) enforces the leading [pressure-balanced plasma perturbation](../../../../pressure-balanced-plasma-perturbation.md) condition $\delta\Pi=0$, giving

$$
\boxed{h=-\frac{4\pi\delta p_\perp}{B_0^2}=-\frac\beta2\frac{\delta p_\perp}{p_0}.}
$$

In the radial component, the curvature part of the perturbed magnetic force is $-2Mh/R$: one contribution comes from $(\mathbf B_0\cdot\nabla)\delta\mathbf B$ and one from $(\delta\mathbf B\cdot\nabla)\mathbf B_0$. The perturbed [pressure anisotropy](../../../../pressure-anisotropy.md) contributes $-(\delta p_\perp-\delta p_\parallel)/R$. After the leading total-[pressure](../../../../pressure-split.md) constraint has removed $\partial_x\delta\Pi$, the radial equation is

$$
-\rho_0\omega^2\xi_x=-Mk_\parallel^2\xi_x-\frac{2Mh}{R}-\frac{\delta p_\perp-\delta p_\parallel}{R}.
$$

Substituting $Mh=-\delta p_\perp$ gives

$$
\boxed{(\omega^2-k_\parallel^2v_A^2)\xi_x=-\frac{\delta p_\perp+\delta p_\parallel}{\rho_0R}.}
$$

Although $h$ is small at low [plasma beta](../../../../plasma-beta.md), its contribution $Mh$ to the [force balance](../../../../force-balance.md) is of the same order as $\delta p_\perp$ and must be kept.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the collisionless plasma physics course of the University of Oxford](../../../split.md)
5. [Collisionless plasma physics course of the University of Oxford](../../../../collisionless-plasma-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
