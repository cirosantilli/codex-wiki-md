<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [regular category](../../../../../regular-category.md) has finite limits, regular-epimorphism--monomorphism image factorizations, and regular epimorphisms stable under pullback. A relation $A\rightsquigarrow B$ in $\mathbf{Rel}(\mathcal C)$ is a subobject of $A\times B$; composition forms the pullback over the middle object and then takes its image.

Suppose $R:A\rightsquigarrow B$ has a right adjoint relation $S$, so $1_A\leq SR$ and $RS\leq1_B$. In the internal regular logic, the first inequality says that for every $a$ there is a $b$ with $R(a,b)$ and $S(b,a)$. If also $R(a,b')$, the second inequality forces $b=b'$. Thus $R$ is total and single-valued. Categorically, if $R\hookrightarrow A\times B$ has projections $p:R\to A$ and $q:R\to B$, totality makes $p$ a regular epimorphism and single-valuedness makes it a monomorphism. Hence $p$ is an isomorphism and $R$ is the [graph of a morphism as a relation](../../../../../graph-of-a-morphism-as-a-relation.md) $qp^{-1}:A\to B$. Conversely, the graph of any morphism is left adjoint to its converse relation, as the two required inequalities follow directly from equality. This proves the characterization.

Let $L$ be a [frame](../../../../../complete-heyting-algebra.md). Composition in the [category of matrices valued in a frame](../../../../../category-of-matrices-valued-in-a-frame.md) is

$$
(gf)(a,c)=\bigvee_{b\in B}f(a,b)\wedge g(b,c).
$$

If $f\dashv g$, the diagonal part of $1_A\leq gf$ implies

$$
1=\bigvee_b f(a,b)\wedge g(b,a)\leq\bigvee_bf(a,b),
$$

so every row of $f$ joins to $1$. For $b\ne b'$, distribute $f(a,b)\wedge f(a,b')$ over the displayed join. Every term vanishes by $fg\leq1_B$, first using the factor with column $b$ and then the one with column $b'$. Hence

$$
f(a,b)\wedge f(a,b')=0.
$$

Conversely, if the rows of $f$ join to $1$ and have pairwise disjoint entries, define $g(b,a)=f(a,b)$. Then

$$
(gf)(a,a)=\bigvee_bf(a,b)=1,
$$

while $(fg)(b,b')=0$ for $b\ne b'$. Thus $1_A\leq gf$ and $fg\leq1_B$, proving the stated criterion.

Finally take $L=\Omega(X)$ for a connected [topological space](../../../../../topological-space.md) $X$. For fixed $a$, the opens $f(a,b)$ are pairwise disjoint and cover $X$. Connectedness forces exactly one of them to be $X$ and all the others to be empty. Hence a left adjoint matrix determines a unique function $\varphi:A\to B$ by $f(a,\varphi(a))=X$. Conversely every function gives this matrix, and matrix composition agrees with function composition. The left adjoints in $\mathbf{Mat}(\Omega(X))$ therefore form a category isomorphic to $\mathbf{Set}$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
