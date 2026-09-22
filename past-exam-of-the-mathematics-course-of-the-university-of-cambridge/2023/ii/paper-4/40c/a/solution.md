<h1 id="40c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonzero real vector $x$, the [Rayleigh quotient](../../../../../../rayleigh-quotient.md) of the [matrix](../../../../../../matrix.md) $A$ is

$$
\boxed{R_A(x)=\frac{x^TAx}{x^Tx}}.
$$

The [Rayleigh quotient iteration](../../../../../../rayleigh-quotient-iteration.md) starts from a unit vector $v_0$. Given $v_k$, compute the shift

$$
\mu_k=R_A(v_k),
$$

solve the [linear system](../../../../../../system-of-linear-equations.md)

$$
(A-\mu_kI)w_k=v_k,
$$

and normalize in the [Euclidean norm](../../../../../../euclidean-norm.md):

$$
v_{k+1}=\frac{w_k}{\|w_k\|_2}.
$$

The next eigenvalue estimate is $\mu_{k+1}=R_A(v_{k+1})$. The process stops when the [eigenpair residual](../../../../../../eigenpair-residual.md) is sufficiently small.

## ↑ Ancestors (11)

1. [A](../a.md)
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
