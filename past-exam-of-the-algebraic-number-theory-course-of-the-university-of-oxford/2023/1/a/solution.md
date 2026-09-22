<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [number field](../../../../number-field.md) $K$ of [degree of a field extension](../../../../degree-of-a-field-extension.md) $n$, an [integral basis](../../../../integral-basis.md) is a [basis](../../../../basis.md) $\omega_1,\ldots,\omega_n$ over $\mathbb Q$ such that

$$
\mathcal O_K=\mathbb Z\omega_1\oplus\cdots\oplus\mathbb Z\omega_n.
$$

Thus every [algebraic integer](../../../../algebraic-integer.md) in $K$ has a unique expression with [integer](../../../../integer-split.md) coefficients in this [basis](../../../../basis.md). Merely requiring its entries to be [algebraic integers](../../../../algebraic-integer.md) would not suffice: for example, $1,2\sqrt2$ is a rational [basis](../../../../basis.md) of $\mathbb Q(\sqrt2)$ but misses the [algebraic integer](../../../../algebraic-integer.md) $\sqrt2$ in its integer span.

Here is a proof of the [existence of an integral basis](../../../../existence-of-an-integral-basis.md). Start with any rational [basis](../../../../basis.md) $v_1,\ldots,v_n$. Each $v_j$ has a nonzero [integer](../../../../integer-split.md) multiple $\alpha_j$ that is an [algebraic integer](../../../../algebraic-integer.md). Indeed, if

$$
v^m+c_{m-1}v^{m-1}+\cdots+c_0=0,\qquad c_i\in\mathbb Q,
$$

choose a positive [integer](../../../../integer-split.md) $q$ clearing all the denominators. Then $qv$ satisfies the [monic polynomial](../../../../monic-polynomial.md)

$$
X^m+qc_{m-1}X^{m-1}+q^2c_{m-2}X^{m-2}+\cdots+q^mc_0\in\mathbb Z[X].
$$

The $\alpha_j$ are still a rational [basis](../../../../basis.md). Put $M=\sum_j\mathbb Z\alpha_j$ and form the [matrix](../../../../matrix.md)

$$
T=(\operatorname{Tr}_{K/\mathbb Q}(\alpha_i\alpha_j))_{i,j},\qquad D=\det T.
$$

Its entries are [integers](../../../../integer-split.md), because products and sums of [algebraic integers](../../../../algebraic-integer.md) are [algebraic integers](../../../../algebraic-integer.md) and a rational [algebraic integer](../../../../algebraic-integer.md) is an [integer](../../../../integer-split.md). The [nondegeneracy of the trace form of a number field](../../../../nondegeneracy-of-the-trace-form-of-a-number-field.md) gives $D\ne0$: if $x\ne0$, then $\operatorname{Tr}(xx^{-1})=n\ne0$.

For $x=\sum_j x_j\alpha_j\in\mathcal O_K$, each $\operatorname{Tr}(x\alpha_i)$ is an [integer](../../../../integer-split.md), so

$$
T(x_1,\ldots,x_n)^T\in\mathbb Z^n.
$$

The [adjugate matrix](../../../../adjugate-matrix.md) formula for $T^{-1}$ gives $Dx_j\in\mathbb Z$. Consequently

$$
M\subseteq\mathcal O_K\subseteq D^{-1}M.
$$

The [submodule theorem for free modules over a principal ideal domain](../../../../submodule-theorem-for-free-modules-over-a-principal-ideal-domain.md) says that every subgroup of the finite-rank [free abelian group](../../../../free-abelian-group.md) $D^{-1}M$ is again a [free abelian group](../../../../free-abelian-group.md) of rank at most $n$. Since $\mathcal O_K$ contains $M$, its rank is exactly $n$. A [basis](../../../../basis.md) of this [free abelian group](../../../../free-abelian-group.md) is the required [integral basis](../../../../integral-basis.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic number theory course of the University of Oxford](../../../split.md)
5. [Algebraic number theory course of the University of Oxford](../../../../algebraic-number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
