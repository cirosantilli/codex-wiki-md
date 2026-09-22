<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the finite [residue field](../../../../../../residue-field.md) as $k=\mathbb F_q$, with $q=p^f$ and residue characteristic $p$. Every $\bar a\in k$ satisfies $\bar a^q=\bar a$. The polynomial $F(X)=X^q-X$ has derivative $qX^{q-1}-1$, whose reduction is $-1$. Hence [Hensel lemma](../../../../../../hensel-s-lemma.md) gives a unique lift $[\bar a]\in\mathcal O_K$ such that

$$
[\bar a]\bmod\mathfrak m_K=\bar a,\qquad[\bar a]^q=[\bar a].
$$

This includes $[0]=0$ and $[1]=1$. If $\bar a\ne0$, its lift is a unit and satisfies $[\bar a]^{q-1}=1$.

The product $[\bar a][\bar b]$ also satisfies $X^q=X$ and has residue $\bar a\bar b$. Uniqueness therefore gives $[\bar a\bar b]=[\bar a][\bar b]$. Reduction is a left inverse of this map, so the map is injective. Restricting to nonzero residues proves the requested multiplicative [Teichmuller lift](../../../../../../teichmuller-representative.md):

$$
\boxed{k^\times\hookrightarrow\mathcal O_K^\times\subset K^\times,\qquad\bar a\longmapsto[\bar a].}
$$

Its image is the group of $(q-1)$st roots of unity in $K$. Indeed a root of unity of that order is a unit satisfying $X^q=X$, hence is the unique lift of its residue. The only finite-field fact used here is $a^q=a$; for $a\ne0$ it follows from Lagrange's theorem in the multiplicative group of order $q-1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
