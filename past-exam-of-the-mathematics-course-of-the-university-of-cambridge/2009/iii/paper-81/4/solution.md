<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $\ell_g$ for the dimensional offset of the [centre of mass](../../../../../center-of-mass.md), reserving $h$ below for the dimensionless swimming parameter. The weight $-mg\mathbf k$ acts at $-\ell_g\mathbf p$, so its [torque](../../../../../torque.md) about the geometric centre is $mg\ell_g\mathbf p\times\mathbf k$. Buoyancy acts through the geometric centre and has no such [torque](../../../../../torque.md). For a spherical cell, the ambient angular [velocity](../../../../../velocity.md) is $\boldsymbol\omega/2$ and the rotational resistance is $\zeta_r=\rho\nu\alpha_\perp v$. Neglecting angular inertia, [torque](../../../../../torque.md) balance gives

$$
\boldsymbol\Omega_{\mathrm{cell}}=\frac12\boldsymbol\omega+\frac1B\mathbf p\times\mathbf k,\qquad B=\frac{\rho\nu\alpha_\perp v}{mg\ell_g}.
$$

Since $\dot{\mathbf p}=\boldsymbol\Omega_{\mathrm{cell}}\times\mathbf p$, the [bottom-heavy spherical-cell orientation dynamics](../../../../../bottom-heavy-spherical-cell-orientation-dynamics.md) is

$$
\boxed{\dot{\mathbf p}=\frac1B[\mathbf k-(\mathbf k\cdot\mathbf p)\mathbf p]+\frac12\boldsymbol\omega\times\mathbf p.}
$$

Thus a steady orientation satisfies

$$
\boxed{\frac1B[\mathbf k-(\mathbf k\cdot\mathbf p)\mathbf p]=-\frac12\boldsymbol\omega\times\mathbf p.}
$$

**The printed algebraic equation has the opposite sign on its right side**, if [vorticity](../../../../../vorticity.md) means the usual $\nabla\times\mathbf u$. Its later concentration equation is consistent with the corrected sign. In particular, linearizing the corrected equation about $\mathbf p=\mathbf k$ gives $\mathbf p_\perp=(B/2)(\boldsymbol\omega\times\mathbf k)_\perp$, whereas the printed sign would reverse that response. Merely changing the definition of [vorticity](../../../../../vorticity.md) would also require changing the ensuing fluid and orientation calculations.

The [gyrotactic reorientation time](../../../../../gyrotactic-reorientation-time.md) $B$ measures gravitational restoration against rotational viscous resistance. In still fluid a tilt angle obeys $\dot\theta=-\sin\theta/B$, so

$$
\tan\frac{\theta(t)}2=\tan\frac{\theta(0)}2e^{-t/B}.
$$

For small tilt it is precisely the exponential relaxation time. Applying the algebraic orientation balance to a time-dependent disturbance additionally assumes that this relaxation is fast enough to neglect orientation lag. Keeping the full dynamic orientation equation would introduce an additional relaxation factor into the perturbation problem.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 81](../../paper-81-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
