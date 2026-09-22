<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\rho_i=\rho_n=\rho$ and $\mu=\mu_{in}=\mu_{ni}$. Use [normal modes](../../../../../../normal-mode.md) proportional to $e^{i\mathbf k\cdot\mathbf x-i\omega t}$, so $\operatorname{Im}\omega<0$ means damping. The linear [displacements](../../../../../../displacement.md) satisfy

$$
\mathbf u_i=\partial_t\boldsymbol\xi_i=-i\omega\boldsymbol\xi_i,\qquad\mathbf u_n=\partial_t\boldsymbol\xi_n=-i\omega\boldsymbol\xi_n,\qquad\mathbf k\cdot\boldsymbol\xi_i=\mathbf k\cdot\boldsymbol\xi_n=0.
$$

For a nonzero-frequency perturbation, linearizing the [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) gives

$$
\partial_t\delta\mathbf B=B_0\partial_z\partial_t\boldsymbol\xi_i,\qquad\delta\mathbf B=B_0\partial_z\boldsymbol\xi_i=ik_\parallel B_0\boldsymbol\xi_i.
$$

Project both momentum equations with $\mathsf P=I-\mathbf k\mathbf k^T/k^2$. This removes the [pressure gradients](../../../../../../pressure-gradient.md). The [magnetic tension](../../../../../../magnetic-tension.md) is already transverse to $\mathbf k$, and, with $a=k_\parallel v_A$, the projected equations are

$$
\ddot{\boldsymbol\xi}_i=-a^2\boldsymbol\xi_i-\mu(\dot{\boldsymbol\xi}_i-\dot{\boldsymbol\xi}_n),\qquad\ddot{\boldsymbol\xi}_n=-\mu(\dot{\boldsymbol\xi}_n-\dot{\boldsymbol\xi}_i).
$$

Here $v_A=B_0/\sqrt{4\pi\rho}$ uses the [ion](../../../../../../ion.md) [density](../../../../../../density.md), as stipulated. For either of the two independent transverse polarizations, the [equal-density ion-neutral Alfvén dispersion relation](../../../../../../equal-density-ion-neutral-alfven-dispersion-relation.md) follows from

$$
\begin{pmatrix}\omega^2-a^2+i\mu\omega&-i\mu\omega\\-i\mu\omega&\omega^2+i\mu\omega\end{pmatrix}\begin{pmatrix}\xi_i\\\xi_n\end{pmatrix}=0.
$$

Its determinant is $\omega[\omega^3+2i\mu\omega^2-a^2\omega-i\mu a^2]$. Removing the static neutral-displacement factor gives

$$
\boxed{\omega^3+2i\mu\omega^2-a^2\omega-i\mu a^2=0.}
$$

The removed factor is a time-independent neutral [displacement](../../../../../../displacement.md) with no [velocity](../../../../../../velocity.md) or magnetic perturbation, a relabeling of the homogeneous neutral fluid rather than a fourth physical [wave](../../../../../../wave.md). Direct elimination in the first-order system for $(u_i,u_n,\delta B)$ gives exactly the same cubic. This also handles the zero-frequency limits without introducing a displacement-label mode.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
