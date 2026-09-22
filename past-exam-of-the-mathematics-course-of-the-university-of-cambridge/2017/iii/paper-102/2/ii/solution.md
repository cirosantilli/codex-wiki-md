<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [classification of finite-dimensional sl2 representations](../../../../../../classification-of-finite-dimensional-sl2-representations.md). In the irreducible representation $V(m)$, choose $v_j=f^jv_0$, $0\leq j\leq m$, so

$$
hv_j=(m-2j)v_j,\qquad fv_j=v_{j+1},\qquad
ev_j=j(m-j+1)v_{j-1},
$$

with vectors beyond the endpoints interpreted as zero. The [invariant form on an irreducible sl2 module](../../../../../../invariant-form-on-an-irreducible-sl2-module.md) is

$$
\boxed{B(v_j,v_k)=\begin{cases}(-1)^j,&j+k=m,\\0,&j+k\ne m.\end{cases}}
$$

Its anti-diagonal entries are nonzero, so it is [nondegenerate](../../../../../../nondegenerate-bilinear-form.md). [Lie-invariant bilinear form](../../../../../../lie-invariant-bilinear-form.md) invariance under $h$ follows from the sum of the two weights. For $f$, the two potentially nonzero terms are $(-1)^{j+1}$ and $(-1)^j$. For $e$, their coefficients coincide when $j+k=m+1$, and their signs are opposite. These checks prove invariance under the generators of the [sl2 Lie algebra](../../../../../../sl2-lie-algebra.md).

Interchanging $j,k$ multiplies the form by $(-1)^m$, giving

$$
\boxed{B\text{ is symmetric for even }m,\quad\text{alternating for odd }m.}
$$

Equivalently it is a [symmetric bilinear form](../../../../../../symmetric-bilinear-form.md) in [odd integer](../../../../../../odd-integer.md) [dimension](../../../../../../dimension-vector-space.md) and an [alternating bilinear form](../../../../../../alternating-bilinear-form.md) in [even number](../../../../../../even-number.md) [dimension](../../../../../../dimension-vector-space.md). The [Weyl complete reducibility theorem](../../../../../../weyl-complete-reducibility-theorem.md) expresses any finite-dimensional representation as a [direct sum](../../../../../../direct-sum.md) of these irreducibles. Give each summand the displayed form and make different summands orthogonal. The resulting form is invariant and nondegenerate. On a reducible representation with both parities, this orthogonal sum need not itself be symmetric or alternating; the dichotomy in the preceding part required irreducibility.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
