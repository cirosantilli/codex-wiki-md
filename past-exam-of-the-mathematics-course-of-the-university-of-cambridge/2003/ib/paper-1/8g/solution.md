<h1 id="8g/solution">Solution</h1>

↑ **Parent:** [8G](../8g.md)

Nondegeneracy of $b$ means both radicals are zero: if $b(x,y)=0$ for every $y$, then $x=0$, and the analogous implication holds in the other variable. Define [linear maps](../../../../../linear-map.md) $B_U:U\to V^*$ and $B_V:V\to U^*$ by $B_U(x)(y)=b(x,y)$ and $B_V(y)(x)=b(x,y)$. Both are injective. Finite dimensionality gives $\dim U\leq\dim V$ and $\dim V\leq\dim U$, so they are [isomorphisms](../../../../../isomorphism.md).

Similarly define $C_U(x)(y)=c(x,y)$ and $C_V(y)(x)=c(x,y)$, which are linear by bilinearity. Set

$$
\boxed{S=B_U^{-1}C_U,\qquad T=B_V^{-1}C_V.}
$$

Then $S$ and $T$ are [linear endomorphisms](../../../../../linear-endomorphism.md) of $U$ and $V$, respectively, and their definitions give $b(Sx,y)=c(x,y)=b(x,Ty)$ for every pair. These [dual isomorphisms induced by a nondegenerate pairing](../../../../../dual-isomorphisms-induced-by-a-nondegenerate-pairing.md) also prove uniqueness. No symmetry of $b$, and no identification of the two vector spaces, is required.

## ↑ Ancestors (10)

1. [8G](../8g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
