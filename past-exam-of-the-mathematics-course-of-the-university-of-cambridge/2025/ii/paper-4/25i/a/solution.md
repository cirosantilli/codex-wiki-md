<h1 id="25i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $v$ in a sufficiently small neighbourhood of $0\in T_pS$, let $\gamma_v$ be the geodesic satisfying $\gamma_v(0)=p$ and $\dot\gamma_v(0)=v$. The [exponential map](../../../../../../exponential-map-riemannian-geometry.md) at $p$ is

$$
\exp_p(v)=\gamma_v(1).
$$

Choose an oriented orthonormal basis of $T_pS$, write $e(\theta)=(\cos\theta,\sin\theta)$, and define [geodesic polar coordinates](../../../../../../geodesic-polar-coordinates.md) by

$$
\phi(r,\theta)=\exp_p\bigl(r e(\theta)\bigr).
$$

The [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) says that radial and angular coordinate curves are orthogonal. Since $r\mapsto\phi(r,\theta)$ is a unit-speed geodesic,

$$
|\phi_r|=1.
$$

Moreover, torsion-freeness of the surface connection gives $D_r\phi_\theta=D_\theta\phi_r$, and therefore

$$
\begin{aligned}
\frac{\partial}{\partial r}\langle\phi_r,\phi_\theta\rangle
&=\langle D_r\phi_r,\phi_\theta\rangle
  +\langle\phi_r,D_r\phi_\theta\rangle\\
&=0+\langle\phi_r,D_\theta\phi_r\rangle
=\frac12\frac{\partial}{\partial\theta}|\phi_r|^2=0.
\end{aligned}
$$

At $r=0$, $\phi_\theta=0$, so $\langle\phi_r,\phi_\theta\rangle=0$ for every sufficiently small $r$. Thus the [first fundamental form](../../../../../../first-fundamental-form.md) is

$$
\boxed{I=dr^2+G(r,\theta)\,d\theta^2},
\qquad G(r,\theta)=|\phi_\theta|^2,
$$

and $\sqrt G/r\to1$ as $r\downarrow0$ because $d(\exp_p)_0$ is the identity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [25I](../../25i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
