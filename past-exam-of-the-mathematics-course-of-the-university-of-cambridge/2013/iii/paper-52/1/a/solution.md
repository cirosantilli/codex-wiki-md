<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\mathbf u=\partial_t\boldsymbol\xi$. In the uniform equilibrium, the [linearized ideal magnetohydrodynamic equations](../../../../../../linearized-ideal-magnetohydrodynamic-equations.md) reduce to

$$
\partial_t\delta\rho=-\rho\nabla\cdot\partial_t\boldsymbol\xi,\qquad
\partial_t\delta p=-\gamma p\nabla\cdot\partial_t\boldsymbol\xi,\qquad
\partial_t\delta\mathbf B=\nabla\times(\partial_t\boldsymbol\xi\times\mathbf B).
$$

Integrating from the undisplaced reference state, and using the uniform background [magnetic field](../../../../../../magnetic-field.md), gives

$$
\boxed{\delta\rho=-\rho\nabla\cdot\boldsymbol\xi,\quad
\delta p=-\gamma p\nabla\cdot\boldsymbol\xi,\quad
\delta\mathbf B=(\mathbf B\cdot\nabla)\boldsymbol\xi-\mathbf B\nabla\cdot\boldsymbol\xi.}
$$

These are the perturbations induced by the [fluid displacement](../../../../../../lagrangian-displacement-fluid-mechanics.md); independent time-independent changes to the reference state are excluded. The linear [Lorentz force density](../../../../../../lorentz-force-density.md) is $(\nabla\times\delta\mathbf B)\times\mathbf B/\mu_0$. Its [magnetic pressure](../../../../../../magnetic-pressure.md) and [magnetic tension](../../../../../../magnetic-tension.md) parts give

$$
\boxed{\rho\partial_t^2\boldsymbol\xi=-\nabla\left(\delta p+\frac{\mathbf B\cdot\delta\mathbf B}{\mu_0}\right)+\frac{(\mathbf B\cdot\nabla)\delta\mathbf B}{\mu_0}.}
$$

For a [Fourier mode](../../../../../../fourier-mode.md), put $s=\mathbf k\cdot\boldsymbol\xi$, $q=\mathbf B\cdot\boldsymbol\xi$ and $K=\mathbf k\cdot\mathbf B$. Then $\delta p=-i\gamma p s$ and $\delta\mathbf B=i(K\boldsymbol\xi-\mathbf B s)$. Substitution gives

$$
\boxed{\rho\omega^2\boldsymbol\xi=\mathbf k\left[\left(\gamma p+\frac{B^2}{\mu_0}\right)s-\frac{Kq}{\mu_0}\right]+\frac{K}{\mu_0}(K\boldsymbol\xi-\mathbf B s).}
$$

If $s=q=0$, the [fluid displacement](../../../../../../lagrangian-displacement-fluid-mechanics.md) is perpendicular to both the [wave vector](../../../../../../wavevector.md) and the [magnetic field](../../../../../../magnetic-field.md). Only [magnetic tension](../../../../../../magnetic-tension.md) restores it, and

$$
\boxed{\omega^2=(\mathbf k\cdot\mathbf v_a)^2,\qquad \mathbf v_a=\frac{\mathbf B}{\sqrt{\mu_0\rho}}.}
$$

This is the [Alfvén wave](../../../../../../alfven-wave.md). The [Alfvén velocity](../../../../../../alfven-velocity.md) is the field-directed propagation vector: $\omega=\pm\mathbf k\cdot\mathbf v_a$. The signed [phase velocity](../../../../../../phase-velocity.md) normal to the wavefront is $\pm v_a\cos\theta\,\widehat{\mathbf k}$; the [group velocity](../../../../../../group-velocity.md) is $\pm\mathbf v_a$. The distinction matters for oblique propagation. For generic directions the [Alfvén wave](../../../../../../alfven-wave.md) has one transverse polarization, with $\delta\rho=\delta p=0$.

To obtain the other [magnetohydrodynamic waves](../../../../../../magnetohydrodynamic-wave.md), take the scalar products with $\mathbf k$ and $\mathbf B$:

$$
\rho\omega^2s=k^2\left[\left(\gamma p+\frac{B^2}{\mu_0}\right)s-\frac{Kq}{\mu_0}\right],\qquad
\rho\omega^2q=\gamma p K s.
$$

The [determinant](../../../../../../determinant.md) condition for a nonzero pair $(s,q)$ is

$$
\omega^4-k^2(c_s^2+v_a^2)\omega^2+k^4c_s^2v_a^2\cos^2\theta=0,\qquad c_s^2=\frac{\gamma p}{\rho}.
$$

Thus the [fast magnetosonic wave](../../../../../../fast-magnetosonic-wave.md) and [slow magnetosonic wave](../../../../../../slow-magnetosonic-wave.md) have

$$
\boxed{v_{\mathrm f,\mathrm{sl}}^2=\frac{c_s^2+v_a^2}{2}\pm\sqrt{\frac{(c_s^2+v_a^2)^2}{4}-c_s^2v_a^2\cos^2\theta}.}
$$

Their [fluid displacements](../../../../../../lagrangian-displacement-fluid-mechanics.md) lie in the plane of $\mathbf k$ and $\mathbf B$ and are generally compressive. In the [fast magnetosonic wave](../../../../../../fast-magnetosonic-wave.md), gas and [magnetic pressure](../../../../../../magnetic-pressure.md) provide the stronger restoring combination; in the [slow magnetosonic wave](../../../../../../slow-magnetosonic-wave.md), their perturbations oppose one another. The [phase speeds](../../../../../../phase-speed.md) depend on direction. They satisfy $v_{\mathrm{sl}}\leq\min(c_s,v_a)$ and $v_{\mathrm f}\geq\max(c_s,v_a)$. For parallel propagation the two speeds are $c_s$ and $v_a$, with a degeneracy between a transverse branch and the [Alfvén wave](../../../../../../alfven-wave.md). For perpendicular propagation $v_{\mathrm f}^2=c_s^2+v_a^2$ and $v_{\mathrm{sl}}=0$; the latter is a nonpropagating limiting disturbance. These special directions require interpreting the polarizations by continuity rather than assuming three distinct nonzero frequencies.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
