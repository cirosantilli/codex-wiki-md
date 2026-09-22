<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\langle\cdot\rangle$ denote $(2\pi)^{-2}\int d^2\theta$. Average the [Collisionless Boltzmann equation](../../../../collisionless-boltzmann-equation.md) to second order. All first-order angle derivatives average to zero, leaving

$$
\partial_tf_0=-\langle\{\delta f,\delta\Phi\}\rangle.
$$

An angle [integration by parts](../../../../integration-by-parts.md) shows that

$$
\begin{aligned}
\langle\{\delta f,\delta\Phi\}\rangle
&=\left\langle\partial_{\theta_i}\delta f\,\partial_{J_i}\delta\Phi-\partial_{J_i}\delta f\,\partial_{\theta_i}\delta\Phi\right\rangle\\
&=-\partial_{J_i}\langle\delta f\,\partial_{\theta_i}\delta\Phi\rangle.
\end{aligned}
$$

Thus the angle-averaged [galactic distribution function](../../../../galactic-distribution-function.md) obeys an action-space [continuity equation](../../../../continuity-equation.md),

$$
\partial_tf_0=-\partial_{J_i}q_i,\qquad q_i=-\langle\delta f\,\partial_{\theta_i}\delta\Phi\rangle.
$$

This sign also follows from [Hamilton's equations](../../../../hamilton-s-equations.md), $\dot J_i=-\partial_{\theta_i}\delta\Phi$: the flux is $\langle\delta f\,\dot J_i\rangle$.

Reality gives $\delta\phi_{-\mathbf k}=\delta\phi_{\mathbf k}^*$ and $\delta f_{-\mathbf k}=\delta f_{\mathbf k}^*$. Orthogonality of the [Fourier series](../../../../fourier-series-split.md) implies

$$
\langle\delta f\,\partial_{\theta_i}\delta\Phi\rangle=-i\sum_{\mathbf k}k_i\delta f_{\mathbf k}\delta\phi_{\mathbf k}^*.
$$

Insert [b](../b.md) to obtain

$$
q_i=-\sum_{\mathbf k}k_i\int_0^t dt'\,\mathbf k\cdot\partial_{\mathbf J}f_0(\mathbf J,t')\,e^{-i\mathbf k\cdot\boldsymbol\Omega(t-t')}\delta\phi_{\mathbf k}(\mathbf J,t')\delta\phi_{\mathbf k}^*(\mathbf J,t).
$$

Although individual terms are complex, pairing $\mathbf k$ with $-\mathbf k$ makes the flux real.

Now take the [marginalization](../../../../marginalization.md) specified by $F_0=2\pi\int_0^\infty f_0\,dJ_R$. Assume vanishing radial-action flux at $J_R=0$ and $J_R\to\infty$: the first boundary does not permit negative [radial action](../../../../radial-action.md), and the second has no escaping flux in this calculation. Then

$$
\partial_tF_0=-2\pi\partial_{J_\varphi}\int_0^\infty q_\varphi\,dJ_R-2\pi[q_R]_0^\infty=-\partial_{J_\varphi}Q_0,
$$

with

$$
\boxed{\begin{aligned}
Q_0={}&-2\pi\sum_{\mathbf k}k_\varphi\int_0^\infty dJ_R\int_0^t dt'\,\mathbf k\cdot\frac{\partial f_0(\mathbf J,t')}{\partial\mathbf J}\\
&\quad\times e^{-i\mathbf k\cdot\boldsymbol\Omega(t-t')}\delta\phi_{\mathbf k}(\mathbf J,t')\delta\phi_{\mathbf k}^*(\mathbf J,t).
\end{aligned}}
$$

If radial-action boundary flux were present, its explicit boundary term would have to be retained.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
