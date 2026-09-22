<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

All edges in the [Type E(p,q,k) Coxeter graph](../../../../../../type-e-p-q-k-coxeter-graph.md) are unlabelled, so the factor $a^2$ in part c is one. Separate the arm of length $p$ from the central vertex. The remaining two arms form a type $A_{q+k+1}$ chain, while deleting the central vertex leaves the disjoint type $A_q$ and type $A_k$ chains. Using $\det G(A_r)=r+1$ in the formula from part c yields

$$
\begin{aligned}
\det G(E(p,q,k))
&=(p+1)(q+k+2)-p(q+1)(k+1)\\
&=(p+1)(q+1)(k+1)
\left(\frac1{p+1}+\frac1{q+1}+\frac1{k+1}-1\right).
\end{aligned}
$$

The associated [bilinear form](../../../../../../bilinear-form.md) is degenerate exactly when

$$
\frac1{p+1}+\frac1{q+1}+\frac1{k+1}=1.
$$

The positive-integer solutions of $1/a+1/b+1/c=1$, up to permutation, are $(3,3,3)$, $(2,4,4)$, and $(2,3,6)$. Consequently the degenerate arm-length triples are the permutations of

$$
(2,2,2),\qquad(1,3,3),\qquad(1,2,5).
$$

For every other allowed $(p,q,k)$ the determinant is nonzero, so the form is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
