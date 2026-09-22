<h1 id="4/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a fixed point $g_f$, put $g=g_f+\delta g$. Linearizing the [renormalization-group flow](../../../../../../../renormalization-group-flow.md) gives

$$
\frac{d\delta g}{d\ell}=\mathcal B'(g_f)\delta g+O(\delta g^2),\qquad
\mathcal B'(g_f)=-\epsilon+2(n-2)A_Dg_f.
$$

Because $g$ is proportional to temperature at fixed microscopic stiffness, this derivative is the thermal eigenvalue. The [thermal eigenvalues of the spherical nonlinear sigma model](../../../../../../../thermal-eigenvalues-of-the-spherical-nonlinear-sigma-model.md) are

$$
\boxed{y_T(0)=-\epsilon,\qquad y_T(g_*)=\epsilon\quad(n>2,\ \epsilon>0).}
$$

The first value describes the stable zero-temperature ordered fixed point. At the nonzero critical point the thermal perturbation grows as $e^{\epsilon\ell}$, so the stopping scale gives $\xi\propto|g-g_*|^{-1/\epsilon}$ and $\nu=1/\epsilon$ to leading order in the expansion. Higher-loop terms change this to $y_T=\epsilon+O(\epsilon^2)$.

At $\epsilon=0$ the linear eigenvalue is zero, so its sign alone does not decide the flow. For $n>2$ the first nonlinear term is positive. Integrating it gives

$$
\frac1{g(\ell)}=\frac1{g(0)}-\frac{n-2}{2\pi}\ell.
$$

The flow reaches order-one coupling at a length logarithm of order $2\pi/[(n-2)g(0)]$, explaining the [exponentially large correlation length in a two-dimensional spherical sigma model](../../../../../../../exponentially-large-correlation-length-in-a-two-dimensional-spherical-sigma-model.md) rather than a finite-temperature power-law critical point in this smooth-field regime. For $n=2$, $\epsilon=0$, the linear eigenvalue is zero everywhere on the perturbative line and vortex effects require an additional coupling. For $n=2$, $\epsilon>0$, the sole zero-coupling fixed point has $y_T=-\epsilon$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [4](../../../4.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
