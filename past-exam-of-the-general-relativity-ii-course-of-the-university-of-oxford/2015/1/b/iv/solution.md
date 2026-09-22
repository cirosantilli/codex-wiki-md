<h1 id="1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write the [affine function](../../../../../affine-function.md) obtained in part (iii) as $\lambda=c+2b_\mu x^\mu$, with constant $c$ and $b_\mu$. A [Conformal Killing vector field](../../../../../conformal-killing-vector-field.md) with precisely this [conformal Killing factor](../../../../../conformal-killing-factor.md) is

$$
X_{\mathrm{part}}^\mu=cx^\mu+2(b\cdot x)x^\mu-x^2b^\mu,
\qquad x^2=\eta_{\alpha\beta}x^\alpha x^\beta.
$$

Direct [partial differentiation](../../../../../partial-derivative.md) verifies its [Conformal Killing equation](../../../../../conformal-killing-equation.md). Subtracting it from any other solution leaves a [Killing vector field](../../../../../killing-vector-field-split.md) $Y$. The formula in part (iii), now with $\lambda=0$, says $\partial_\mu\partial_\nu Y_\rho=0$. Therefore $Y$ is affine, and the [Killing equation](../../../../../killing-equation.md) makes its linear coefficient antisymmetric after lowering an index. Every solution is consequently

$$
\boxed{X^\mu=a^\mu+\omega^\mu{}_{\nu}x^\nu+cx^\mu+2(b\cdot x)x^\mu-x^2b^\mu,
\qquad \omega_{\mu\nu}=-\omega_{\nu\mu}.}
$$

The four constant $a^\mu$ generate [translations](../../../../../translation-geometry.md), the six independent $\omega_{\mu\nu}$ generate [Lorentz transformations](../../../../../lorentz-transformation.md), $c$ generates a [dilation](../../../../../uniform-dilation.md), and the four $b^\mu$ generate [special conformal transformations](../../../../../special-conformal-transformation.md). Their constant, linear and quadratic terms are independent; within the linear terms, the antisymmetric coefficient cannot equal a nonzero multiple of the identity. Hence the [conformal Killing algebra of Minkowski spacetime](../../../../../conformal-killing-algebra-of-minkowski-spacetime.md) has

$$
\boxed{\dim\mathfrak{conf}(\mathbb R^{1,3})=4+6+1+4=15.}
$$

For $\lambda=1$, the canonical choice is the [dilation](../../../../../uniform-dilation.md) generator $D=x^\mu\partial_\mu$. Its [flow of a vector field](../../../../../flow-of-a-vector-field.md) solves $dx^\mu/ds=x^\mu$, giving

$$
\boxed{\Phi_s(x)=e^s x,\qquad \Phi_s^*\eta=e^{2s}\eta,\qquad \Phi_s\circ\Phi_t=\Phi_{s+t}.}
$$

One may add any [Killing vector field](../../../../../killing-vector-field-split.md) without changing $\lambda=1$, so this choice is not unique. The displayed [dilation](../../../../../uniform-dilation.md) gives a global [one-parameter group](../../../../../one-parameter-subgroup.md) of [diffeomorphisms](../../../../../diffeomorphism.md). The count of fifteen concerns independent [Conformal Killing vector fields](../../../../../conformal-killing-vector-field.md); some [special conformal transformations](../../../../../special-conformal-transformation.md) have only local flows on all of affine [Minkowski spacetime](../../../../../minkowski-spacetime.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the general relativity II course of the University of Oxford](../../../../split.md)
6. [General relativity II course of the University of Oxford](../../../../../general-relativity-ii-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
