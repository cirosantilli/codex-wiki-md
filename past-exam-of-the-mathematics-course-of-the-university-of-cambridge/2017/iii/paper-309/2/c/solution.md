<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) convention

$$
R^\alpha{}_{\beta\mu\nu}=\partial_\mu\Gamma^\alpha{}_{\nu\beta}-\partial_\nu\Gamma^\alpha{}_{\mu\beta}+\Gamma^\alpha{}_{\mu\lambda}\Gamma^\lambda{}_{\nu\beta}-\Gamma^\alpha{}_{\nu\lambda}\Gamma^\lambda{}_{\mu\beta},\qquad R_{\beta\nu}=R^\alpha{}_{\beta\alpha\nu}.
$$

For the limiting [affine connection](../../../../../../affine-connection.md), every product of two nonzero connection coefficients is zero, because its only nonzero coefficients have spatial upper index and both lower indices $t$. Its only possibly nonzero [curvature](../../../../../../curvature.md) components, apart from antisymmetry in the last two indices, are

$$
R^i{}_{tjt}=\partial_j\partial_i\phi.
$$

The [Ricci tensor](../../../../../../ricci-tensor.md) is therefore

$$
\boxed{\operatorname{Ric}(\nabla^{(\infty)})=(\Delta\phi)\,dt\otimes dt.}
$$

All other components vanish, so the limiting connection is a connection with vanishing [Ricci tensor](../../../../../../ricci-tensor.md) exactly when $\phi$ satisfies the [Laplace equation](../../../../../../laplace-equation.md) on spatial [Euclidean space](../../../../../../euclidean-norm.md). This is Ricci-flatness, not necessarily vanishing curvature: $\phi=x^2-y^2$ is a [harmonic function](../../../../../../harmonic-function.md) but has nonzero [Hessian matrix](../../../../../../hessian-matrix.md) and hence a nonflat limiting connection. Reversing the curvature sign convention reverses the displayed Ricci sign but leaves the equivalence unchanged.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
