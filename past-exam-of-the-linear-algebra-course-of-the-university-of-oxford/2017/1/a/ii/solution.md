<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem-split.md) states

$$
\boxed{\chi_T(T)=0.}
$$

Let $d=\dim V$. Extend the [field](../../../../../field.md) to an [algebraically closed field](../../../../../algebraically-closed-field.md) and choose a [basis](../../../../../basis.md) in which the [matrix](../../../../../matrix.md) of $T$ is an [upper triangular matrix](../../../../../upper-triangular-matrix.md), as permitted. Write its diagonal entries as $\lambda_1,\ldots,\lambda_d$ and put $V_i=\operatorname{span}(e_1,\ldots,e_i)$. Each $V_i$ is an [invariant subspace](../../../../../invariant-subspace.md), and

$$
(T-\lambda_iI)V_i\subseteq V_{i-1}.
$$

Apply $T-\lambda_dI$ first, then $T-\lambda_{d-1}I$, and continue. The resulting product sends $V_d$ into $V_0=\{0\}$. These factors are [commuting operators](../../../../../commuting-operators.md), so

$$
\prod_{i=1}^d(T-\lambda_iI)=0.
$$

The [determinant](../../../../../determinant.md) of an [upper triangular matrix](../../../../../upper-triangular-matrix.md) gives $\chi_T(x)=(-1)^d\prod_i(x-\lambda_i)$. Thus $\chi_T(T)=0$ after the [field extension](../../../../../field-extension.md). Its entries were in the original [field](../../../../../field.md), whose embedding is injective, so they were already zero there. The zero-dimensional case is immediate as well.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
