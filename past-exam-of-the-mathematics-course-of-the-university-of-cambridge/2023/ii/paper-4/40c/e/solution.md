<h1 id="40c/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let the computed [eigenpair residual](../../../../../../eigenpair-residual.md) be

$$
r=A\widetilde v-\widetilde\lambda\widetilde v,
\qquad \|r\|_2=\epsilon,
\qquad \|\widetilde v\|_2=1.
$$

Define the [rank-one matrix](../../../../../../rank-one-matrix.md)

$$
E=-r\widetilde v^T.
$$

Then

$$
(A+E)\widetilde v
=A\widetilde v-r(\widetilde v^T\widetilde v)
=\widetilde\lambda\widetilde v,
$$

so $(\widetilde\lambda,\widetilde v)$ is an exact eigenpair of the perturbed matrix $A+E$. Moreover,

$$
\|E\|_2=\|r\|_2\|\widetilde v\|_2=\epsilon,
$$

which is the [backward error of an approximate eigenpair](../../../../../../backward-error-of-an-approximate-eigenpair.md).

Follow the simple eigenvalue branch from $\lambda(0)=\lambda$ for $A(t)=A+tE$. The [first-order perturbation of a simple eigenvalue](../../../../../../first-order-perturbation-of-a-simple-eigenvalue.md) and part (b) give

$$
|\widetilde\lambda-\lambda|
=|\lambda(1)-\lambda(0)|
\approx|\lambda'(0)|
\leq\|E\|_2s(\lambda).
$$

Since the residual is at the [machine precision](../../../../../../machine-epsilon.md) scale, this proves

$$
\boxed{|\widetilde\lambda-\lambda|\lesssim\epsilon s(\lambda)}.
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [40C](../../40c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
