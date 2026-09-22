<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand the [vector field](../../../../vector-field.md) about the reference trajectory:

$$
\dot{\delta\mathbf x}=\mathbf f(\mathbf x+\delta\mathbf x)-\mathbf f(\mathbf x)
=J(t)\delta\mathbf x+O(\|\delta\mathbf x\|^2),\qquad
J_{ij}=\frac{\partial f_i}{\partial x_j}.
$$

Over a sufficiently short interval, the [tangent-linear](../../../../linearization.md) [propagator](../../../../fundamental-matrix-of-a-linear-differential-equation.md) is

$$
\boxed{\delta\mathbf x(t+\delta t)=A\delta\mathbf x(t),\qquad
A=I+J\delta t+O(\delta t^2).}
$$

Consequently

$$
A^TA=I+(J+J^T)\delta t+O(\delta t^2).
$$

If $S=J+J^T$ has $S\mathbf e=\lambda\mathbf e$ and the perturbation is initially parallel to $\mathbf e$, its squared [Euclidean norm](../../../../euclidean-norm.md) obeys

$$
\boxed{\|\delta\mathbf x(t+\delta t)\|^2
=(1+\lambda\delta t)\|\delta\mathbf x(t)\|^2+O(\delta t^2\|\delta\mathbf x(t)\|^2).}
$$

Positive $\lambda$ means instantaneous norm-squared growth, negative $\lambda$ decay, and zero $\lambda$ no first-order change. The corresponding [norm](../../../../norm.md) growth rate is $\lambda/2$, not $\lambda$. These are [eigenvalues](../../../../eigenvalue.md) of the [symmetric part](../../../../symmetric-matrix.md) governing the chosen error metric, not generally the [eigenvalues](../../../../eigenvalue.md) of the nonsymmetric [Jacobian matrix](../../../../jacobian-matrix.md) or the long-time [Lyapunov exponents](../../../../lyapunov-exponent.md). The direction and the reference [Jacobian matrix](../../../../jacobian-matrix.md) evolve during a finite forecast.

## ↑ Ancestors (12)

1. [B](../b.md)
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
