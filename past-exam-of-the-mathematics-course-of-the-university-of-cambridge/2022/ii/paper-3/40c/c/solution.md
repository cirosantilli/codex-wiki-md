<h1 id="40c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix a shift $s$ that is not an [eigenvalue](../../../../../../eigenvalue.md) of $A$. [Inverse iteration](../../../../../../inverse-iteration.md) computes

$$
(A-sI)\mathbf y_{k+1}=\mathbf x_k,
\qquad
\mathbf x_{k+1}
=\frac{\mathbf y_{k+1}}{\|\mathbf y_{k+1}\|},
$$

and may use $r(\mathbf x_k)$ as the eigenvalue estimate.

For a real symmetric matrix, suppose that one eigenvalue $\lambda_*$ is uniquely closest to $s$ and that $\mathbf x_0$ has a nonzero component in its eigenspace. Since the iteration is the [power method](../../../../../../power-method.md) applied to $(A-sI)^{-1}$, the normalized vectors converge, up to sign, to an eigenvector for $\lambda_*$. If $\lambda_{\rm next}$ is the second-closest eigenvalue to the shift, the asymptotic direction-error ratio is

$$
\boxed{
\frac{|\lambda_*-s|}
{|\lambda_{\rm next}-s|}
}.
$$

Thus a shift close to the desired eigenvalue gives rapid convergence. The Rayleigh quotients converge to $\lambda_*$ and, for a simple eigenvalue, their errors are of second order in the vector error. This is [convergence of fixed-shift inverse iteration](../../../../../../convergence-of-fixed-shift-inverse-iteration.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [40C](../../40c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
