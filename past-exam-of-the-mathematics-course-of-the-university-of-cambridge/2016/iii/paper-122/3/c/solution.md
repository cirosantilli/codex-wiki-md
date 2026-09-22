<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The algebra must be finite-dimensional, and there is no universal bound on its dimension.** Let $e=\varepsilon m$ and write its [coevaluation morphism](../../../../../../coevaluation-morphism.md) as a finite sum

$$
n(1)=\sum_{i=1}^r a_i\otimes b_i.
$$

For any $v\in A$, one [snake identity](../../../../../../snake-identity.md) gives

$$
v=\sum_{i=1}^r e(v,a_i)b_i.
$$

Thus the finitely many $b_i$ span $A$, making it a [finite-dimensional vector space](../../../../../../finite-dimensional-vector-space.md). The other [snake identity](../../../../../../snake-identity.md) shows that $e$ is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) in the other variable as well, so the maps to the [dual space](../../../../../../dual-space.md) determined by this pairing are isomorphisms. In the standard algebraic terminology this is a [Frobenius algebra](../../../../../../frobenius-algebra.md).

Every positive finite [dimension of a vector space](../../../../../../dimension-vector-space.md) occurs: take $A=k^d$ with coordinatewise multiplication and $\varepsilon(a_1,\ldots,a_d)=\sum_i a_i$. The coordinate idempotents $e_i$ give $e(e_i,e_j)=\delta_{ij}$ and $n(1)=\sum_i e_i\otimes e_i$. If zero unital algebras are allowed, the zero object gives dimension zero too.

The pairing need not make $A$ a [semisimple algebra](../../../../../../semisimple-algebra.md). For example, the [dual numbers](../../../../../../dual-number.md) $k[t]/(t^2)$ with $\varepsilon(a+bt)=b$ have pairing matrix

$$
\begin{pmatrix}0&1\\1&0\end{pmatrix}
$$

and [coevaluation morphism](../../../../../../coevaluation-morphism.md) $1\mapsto1\otimes t+t\otimes1$. This pairing is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md) over every [field](../../../../../../field.md), despite the [nilpotent ideal](../../../../../../nilpotent-ideal.md) $(t)$. **Finite-dimensionality is the dimension conclusion; separability is not part of the given definition.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
