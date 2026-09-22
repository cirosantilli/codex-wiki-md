<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taking traces of the [constitutive equation](../../../../constitutive-equation.md) gives

$$
\lambda\operatorname{tr}e_\lambda=\frac13\left(\operatorname{tr}S_\lambda-2\mu\operatorname{tr}e_\lambda\right).
$$

The assumed finite limits of [stress](../../../../stress.md) and [strain](../../../../strain.md) make the right side bounded. Therefore $\operatorname{tr}e_\lambda=O(\lambda^{-1})$, and the limiting [strain](../../../../strain.md) satisfies $\operatorname{tr}e=0$. The permitted interchange of [derivatives](../../../../derivative.md) and limits gives $\operatorname{tr}e=\operatorname{div}u$. Define

$$
q=\lim_{\lambda\to\infty}\lambda\operatorname{tr}e_\lambda=\tfrac13\operatorname{tr}S,\qquad p=-q.
$$

Then the limit [stress](../../../../stress.md) is $S=-pI+2\mu e$. Passing to the limit in [force](../../../../force-split.md) balance and using $2\operatorname{Div}e=\Delta u+\nabla\operatorname{div}u$ gives

$$
\boxed{-\mu\Delta u+\nabla p=f,\qquad\operatorname{div}u=0\quad\text{in }\Omega,\qquad u=0\text{ on }\partial\Omega.}
$$

The [pressure](../../../../pressure-split.md) acts as the [Lagrange multiplier](../../../../lagrange-multiplier.md) enforcing the [volume](../../../../volume.md) constraint. The [differential equations](../../../../differential-equation-split.md) determine it up to an additive constant, while a specified absolute limit [stress](../../../../stress.md) can fix that constant.

Nonlinear [elastic incompressibility](../../../../elastic-incompressibility.md) is $\det Dy=1$. Expanding the [determinant](../../../../determinant.md) for $Dy=I+Du$ gives $\det(I+Du)=1+\operatorname{div}u+O(|Du|^2)$, so its first-order form is precisely $\operatorname{div}u=0$. The volumetric energy term $\lambda(\operatorname{div}u)^2/2$ becomes increasingly expensive as $\lambda$ grows, while the fixed positive $\mu$ leaves [shear strain](../../../../shear-strain.md) possible. Thus **the infinite-bulk-stiffness limit is the [incompressible limit of isotropic linear elasticity](../../../../incompressible-limit-of-isotropic-linear-elasticity.md)**, with the same equilibrium operator as the steady [Stokes equations](../../../../stokes-equation.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
