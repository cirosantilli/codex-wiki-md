<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose a [basis](../../../../../../basis.md) $x_1,x_2,x_3$ of the [Lie algebra](../../../../../../lie-algebra-split.md) and filter its [universal enveloping algebra](../../../../../../universal-enveloping-algebra.md) by word length: $F_0R=\mathbb C$ and $F_dR$ is spanned by products of at most $d$ [basis](../../../../../../basis.md) elements. The relations $x_jx_i-x_ix_j=[x_j,x_i]$ replace a degree-two [commutator](../../../../../../commutator.md) by degree one, so the degree-one symbols commute.

The [Poincaré-Birkhoff-Witt theorem](../../../../../../poincare-birkhoff-witt-theorem.md) says the ordered [monomials](../../../../../../monomial.md) $x_1^{a_1}x_2^{a_2}x_3^{a_3}$ are a [basis](../../../../../../basis.md). Its relevant proof can be seen by reordering an inverted neighboring pair using the displayed relation. Reordering terminates because same-length terms have fewer inversions and bracket terms have smaller word length. Disjoint swaps commute; the only overlapping three-letter reorderings differ by $[x_i,[x_j,x_k]]+[x_j,[x_k,x_i]]+[x_k,[x_i,x_j]]=0$. The [Jacobi identity](../../../../../../jacobi-identity.md) therefore makes the reduced ordered expression independent of the reordering path. Ordered [monomials](../../../../../../monomial.md) have no remaining relations and form the [basis](../../../../../../basis.md). Their degree-$d$ symbols give

$$
\boxed{\operatorname{gr}R\cong\operatorname{Sym}(\mathfrak g)\cong\mathbb C[X_1,X_2,X_3]},\qquad\dim F_dR=\binom{d+3}{3}.
$$

For generators $m_1,\ldots,m_q$ of the [finitely generated module](../../../../../../finitely-generated-module.md) $M$, put $M_d=\sum_jF_dRm_j$. This is a [good filtration](../../../../../../good-filtration-of-a-module.md), and $\operatorname{gr}M$ is finite over the three-variable [polynomial ring](../../../../../../polynomial-ring.md). Define the [dimension of a filtered module](../../../../../../dimension-of-a-filtered-module.md) as the [Krull dimension](../../../../../../krull-dimension.md) of its [associated graded module](../../../../../../associated-graded-module.md), equivalently the degree of the eventual cumulative [polynomial](../../../../../../polynomial-split.md) $\dim_{\mathbb C}M_d$, or the [Gelfand–Kirillov dimension of a module](../../../../../../gelfand-kirillov-dimension-of-a-module.md). Two [good filtrations](../../../../../../good-filtration-of-a-module.md) have bounded shifts, so the growth degree is independent of the generators. Since

$$
\dim M_d\le q\binom{d+3}{3},
$$

its [polynomial](../../../../../../polynomial-split.md) degree is at most three. Therefore **every nonzero finitely generated $R$-module has dimension at most $3$**. The zero [module](../../../../../../module-mathematics.md) may be assigned the usual separate empty-support convention. This bound also follows immediately from its [support of a module](../../../../../../support-of-a-module.md) inside affine three-space.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
