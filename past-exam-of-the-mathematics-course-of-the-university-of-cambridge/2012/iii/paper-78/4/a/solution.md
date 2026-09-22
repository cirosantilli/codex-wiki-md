<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [inner product](../../../../../../inner-product.md) convention linear in its first argument. A [singular value system](../../../../../../singular-system-of-a-compact-operator.md) consists of positive [singular values](../../../../../../singular-value.md) $\sigma_n$ and [orthonormal bases](../../../../../../orthonormal-basis.md) $u_n$ of $(\ker A)^\perp\subset X$ and $v_n$ of $\overline{\operatorname{ran}A}\subset Y$, with

$$
Au_n=\sigma_n v_n,\qquad A^*v_n=\sigma_nu_n.
$$

For an infinite-rank [compact operator](../../../../../../compact-operator-split.md), $\sigma_n\to0$; a finite-rank operator has a finite system. Applying the [spectral theorem for compact self-adjoint operators](../../../../../../spectral-theorem-for-compact-hermitian-operators.md) to $A^*A$ constructs $u_n$, with eigenvalues $\sigma_n^2$, and then $v_n=Au_n/\sigma_n$. This solution uses the input/output naming of this problem, which is the reverse of another common singular-vector convention.

The [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md) is

$$
\boxed{x^\dagger=A^\dagger y=\sum_n\frac{\langle y,v_n\rangle}{\sigma_n}u_n.}
$$

Its domain is $\operatorname{ran}A\oplus(\operatorname{ran}A)^\perp$, equivalently the data satisfying the [Picard criterion](../../../../../../picard-criterion.md)

$$
\sum_n\frac{|\langle y,v_n\rangle|^2}{\sigma_n^2}<\infty.
$$

It ignores the component in $\ker A^*$ and lies in $(\ker A)^\perp$. The series then converges in $X$ by orthonormality and is the [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md). If $y\in\operatorname{ran}A$, it is an exact solution; all other exact solutions are $x^\dagger+z$ with $z\in\ker A$. Compactness does not make the inverse bounded when there are infinitely many positive singular values.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
