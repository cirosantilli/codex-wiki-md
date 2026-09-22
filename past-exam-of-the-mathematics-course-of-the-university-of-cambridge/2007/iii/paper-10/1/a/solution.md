<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the complex [inner product](../../../../../../inner-product.md) convention linear in its first argument. Give the [exterior algebra](../../../../../../exterior-algebra.md) its induced [inner product](../../../../../../inner-product.md), with an [orthonormal](../../../../../../orthonormal-set.md) wedge basis. Exterior multiplication is **$e(v)\eta=v\wedge\eta$**. Its adjoint is contraction:

$$
e(b)^*(v_1\wedge\cdots\wedge v_r)
=\sum_{j=1}^r(-1)^{j-1}(v_j,b)\,v_1\wedge\cdots\widehat v_j\cdots\wedge v_r.
$$

Applying this formula to $a\wedge\eta$ separates its first term from the remaining terms, giving $e(b)^*e(a)\eta=(a,b)\eta-e(a)e(b)^*\eta$. Hence the [canonical anticommutation relations](../../../../../../canonical-anticommutation-relations.md) are

$$
\boxed{e(a)e(b)^*+e(b)^*e(a)=(a,b)I.}
$$

For irreducibility, choose an [orthonormal basis](../../../../../../orthonormal-basis.md) $u_1,\ldots,u_d$. The occupancy projections are $N_j=e(u_j)e(u_j)^*$, and $P_0=\prod_j(I-N_j)$ projects onto the vacuum $1\in\Lambda^0V$. For an increasing index set $J$, put $E_J=e(u_{j_1})\cdots e(u_{j_r})$. Then $E_IP_0E_J^*$ maps the wedge basis [vector](../../../../../../vector.md) $u_J$ to $u_I$ and kills every other wedge basis [vector](../../../../../../vector.md). Thus these products are all [matrix units](../../../../../../matrix-unit.md) and the generated star-algebra is **$\operatorname{End}(\Lambda V)$**. Any common [invariant subspace](../../../../../../invariant-subspace.md) for the [creation and annihilation operators](../../../../../../creation-and-annihilation-operators.md) is therefore either zero or all of $W$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
