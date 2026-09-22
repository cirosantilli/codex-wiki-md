<h1 id="12b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Taking the [Laplace transform](../../../../../../laplace-transform.md) of the differential equation and using

$$
\mathcal L\{y'\}(s)=sY(s)-y(0)
$$

gives

$$
sY-y_0=AY+G.
$$

Hence

$$
(sI-A)Y=y_0+G.
$$

Whenever $s$ is not an [eigenvalue](../../../../../../eigenvalue.md) of $A$, the matrix $sI-A$ is invertible, and thus

$$
\boxed{Y(s)=(sI-A)^{-1}(y_0+G(s))}.
$$

This is the [Laplace-transform solution of a constant-coefficient vector ODE](../../../../../../laplace-transform-solution-of-a-constant-coefficient-vector-ode.md).

Set $g=0$. The given homogeneous solution is $y(t)=e^{tA}y_0$, so the preceding formula says

$$
\mathcal L\{e^{tA}\}(s)y_0=(sI-A)^{-1}y_0
$$

for every initial vector $y_0$. Equality on every vector gives the matrix identity

$$
\boxed{\mathcal L\{e^{tA}\}(s)=(sI-A)^{-1}},
$$

on the common domain of convergence and in particular away from the eigenvalues of $A$. This is the [Laplace transform of a matrix exponential](../../../../../../laplace-transform-of-a-matrix-exponential.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12B](../../12b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
