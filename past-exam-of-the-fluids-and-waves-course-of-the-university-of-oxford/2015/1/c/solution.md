<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $s=a^2/r$ and define the image term $G(r,\theta)=(r/a)\Psi(s,\theta)$. The key step is to verify that inversion preserves the [Stokes streamfunction equation for irrotational flow](../../../../stokes-streamfunction-equation-for-irrotational-flow.md). Direct differentiation gives

$$
G_r=\frac1a(\Psi-s\Psi_s),\qquad
G_{rr}=\frac{s^2}{ar}\Psi_{ss},\qquad
G_{\theta\theta}-\cot\theta\,G_\theta
=\frac r a(\Psi_{\theta\theta}-\cot\theta\,\Psi_\theta),
$$

where the quantities on the right are evaluated at $(s,\theta)$. Hence

$$
\mathcal L_rG=\frac r a\left[s^2\Psi_{ss}+\Psi_{\theta\theta}-\cot\theta\,\Psi_\theta\right]
=\frac r a\mathcal L_s\Psi=0.
$$

By [linearity](../../../../linearity.md), $\widetilde\Psi=\Psi-G$ obeys the same equation and describes an [incompressible flow](../../../../incompressible-flow.md) and an [irrotational flow](../../../../irrotational-flow.md) wherever the original exterior flow is regular.

On the [sphere](../../../../sphere.md), $s=a$ and the two terms cancel identically:

$$
\widetilde\Psi(a,\theta)=0,\qquad
\boxed{\widetilde u_r(a,\theta)=\frac{\partial_\theta\widetilde\Psi(a,\theta)}{a^2\sin\theta}=0.}
$$

Thus the [sphere](../../../../sphere.md) is a stream surface and satisfies the [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md). Tangential slip is allowed in this [potential flow](../../../../potential-flow.md) model. For every finite $r>a$, the image argument satisfies $0<s<a$, where $\Psi$ has no singularities. The prefactor $r/a$ is regular there. Therefore the construction creates **no new finite exterior singularities**; any original exterior singularities remain those of the prescribed incident flow. This is the [sphere theorem for a Stokes streamfunction](../../../../sphere-theorem-for-a-stokes-streamfunction.md).

For the far-field claim, the stated bound gives

$$
|G(r,\theta)|\leq\frac r a c\frac{a^2}r=ca
\qquad(r\text{ sufficiently large}).
$$

One must compare [velocities](../../../../velocity.md), rather than require the correction to the [Stokes streamfunction](../../../../stokes-streamfunction.md) to tend to zero. Smoothness at the original origin, together with $\Psi(0,\theta)=0$, gives $\Psi_s=O(1)$ and $\Psi_\theta=O(s)$ there. Thus $G_r=O(r^{-1})$ and $G_\theta=O(1)$, and the correction has

$$
\delta u_r=-\frac{G_\theta}{r^2\sin\theta}=O(r^{-2}),\qquad
\delta u_\theta=\frac{G_r}{r\sin\theta}=O(r^{-2}).
$$

These estimates hold away from the coordinate poles, with the regular-axis limits supplied by the original smooth physical flow. Consequently

$$
\boxed{\widetilde{\mathbf u}-\mathbf u\longrightarrow\mathbf0\quad(r\to\infty).}
$$

The far-field [velocity field](../../../../velocity-field.md) is unchanged. For a fully smooth incident [velocity field](../../../../velocity-field.md) at the origin, the usual regular expansion is stronger and makes the sphere disturbance decay as $r^{-3}$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
