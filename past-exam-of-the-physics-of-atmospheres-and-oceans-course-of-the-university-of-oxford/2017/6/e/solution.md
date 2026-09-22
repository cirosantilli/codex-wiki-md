<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

If one retains the [Euler approximation](../../../../euler-method.md) $A=I+J\delta t$, its exact [norm](../../../../norm.md) [matrix](../../../../matrix.md) is

$$
A^TA=I+(J+J^T)\delta t+J^TJ\delta t^2.
$$

The additional term can mix the instantaneous [symmetric-part](../../../../symmetric-matrix.md) [eigenvectors](../../../../eigenvector.md), so they no longer generally diagonalize finite-time error amplification. However, when $\delta t^2$ is material, a reliable physical [propagator](../../../../fundamental-matrix-of-a-linear-differential-equation.md) must itself be calculated beyond first-order Euler: a large [Euler-step](../../../../euler-method.md) amplification can be a numerical artifact. For constant $J$, the exact map is $\Phi=e^{J\Delta t}$; for a changing reference trajectory it solves $\dot\Phi=J(t)\Phi$, $\Phi(0)=I$.

Use its [singular value decomposition](../../../../singular-value-decomposition.md), $\Phi=U\Sigma V^T$. The initial orthonormal [right singular vectors](../../../../right-singular-vector.md) $\mathbf v_i$ diagonalize $\Phi^T\Phi$ and satisfy

$$
\boxed{\Phi\mathbf v_i=s_i\mathbf u_i,\qquad
\frac{\|\Phi\mathbf v_i\|^2}{\|\mathbf v_i\|^2}=s_i^2.}
$$

A [singular value](../../../../singular-value.md) $s_i>1$ gives finite-time [norm](../../../../norm.md) growth, $s_i<1$ decay, and the leading [right singular vector](../../../../right-singular-vector.md) is the initial perturbation with greatest amplification in the stated [norm](../../../../norm.md). The [left singular vector](../../../../left-singular-vector.md) describes the resulting final error pattern. [Non-normal](../../../../non-normal-matrix.md) dynamics can give transient growth even if every [Jacobian matrix](../../../../jacobian-matrix.md) [eigenvalue](../../../../eigenvalue.md) has negative real part, so selecting observations from those [eigenvalues](../../../../eigenvalue.md) alone is insufficient. Over a genuinely short interval, $s_i^2=1+\lambda_i\delta t+O(\delta t^2)$, recovering the [symmetric-part](../../../../symmetric-matrix.md) result. Initial observations should target the relevant growing right singular projections, with [prior covariance](../../../../covariance-matrix.md) and observational precision included when they are not isotropic.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
