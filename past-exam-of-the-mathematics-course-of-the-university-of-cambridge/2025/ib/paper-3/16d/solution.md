<h1 id="16d/solution">Solution</h1>

↑ **Parent:** [16D](../16d.md)

The initially irrotational inviscid flow remains irrotational, so $u=\nabla\phi$; incompressibility gives $\nabla^2\phi=0$. At the plates, normal [velocity](../../../../../velocity.md) matches their motion:

$$
\frac1r\phi_\theta(r,\alpha)=-\Omega r,\qquad
\frac1r\phi_\theta(r,-\alpha)=\Omega r.
$$

With $\phi=r^2f(\theta)$, Laplace's equation gives $f''+4f=0$. The symmetric solution is

$$
\phi=\frac{\Omega r^2\cos2\theta}{2\sin2\alpha}.
$$

Hence

$$
u_r=\frac{\Omega r\cos2\theta}{\sin2\alpha},\qquad
u_\theta=-\frac{\Omega r\sin2\theta}{\sin2\alpha}.
$$

A streamfunction is

$$
\psi=\frac{\Omega r^2\sin2\theta}{2\sin2\alpha},
$$

so [streamlines](../../../../../streamline.md) are $r^2\sin2\theta=\text{constant}$ and fluid is expelled radially as the plates close. The outward flux through $r=R$ is

$$
\boxed{\int_{-\alpha}^{\alpha}u_rR\,d\theta=\Omega R^2.}
$$

## ↑ Ancestors (10)

1. [16D](../16d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
