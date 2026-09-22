<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $x\in Z(A\otimes_kB)$ uniquely as $x=\sum_j a_j\otimes b_j$ using part (i). For each $a\in A$, the equality $(a\otimes1)x=x(a\otimes1)$ becomes

$$
\sum_j(aa_j-a_ja)\otimes b_j=0.
$$

The coefficient uniqueness from part (i) gives $aa_j=a_ja$ for every $a$, so each $a_j$ belongs to the [center of an associative algebra](../../../../../center-of-an-associative-algebra.md) $Z(A)$. Consequently $x\in Z(A)\otimes_kB$.

Choose a [basis](../../../../../basis.md) $z_1,\ldots,z_t$ of the [vector space](../../../../../vector-space-split.md) $Z(A)$ and rewrite $x=\sum_{i=1}^t z_i\otimes d_i$. For $b\in B$, commuting with $1\otimes b$ gives

$$
\sum_i z_i\otimes(bd_i-d_ib)=0.
$$

Extend the [linearly independent](../../../../../linear-independence.md) family $z_i$ to a [basis](../../../../../basis.md) of $A$ and apply its [dual basis](../../../../../dual-basis.md) to the first factor. It follows that $bd_i=d_ib$ for every $b$, hence $d_i\in Z(B)$. This proves $Z(A\otimes_kB)\subseteq Z(A)\otimes_k Z(B)$.

Conversely, if $z\in Z(A)$ and $w\in Z(B)$, then

$$
(z\otimes w)(a\otimes b)=za\otimes wb=az\otimes bw=(a\otimes b)(z\otimes w).
$$

The [pure tensors](../../../../../pure-tensor.md) $a\otimes b$ span the [tensor product](../../../../../tensor-product.md), so $z\otimes w$ is central, as is every sum of such [pure tensors](../../../../../pure-tensor.md). Therefore the [center of a tensor product of associative algebras](../../../../../center-of-a-tensor-product-of-associative-algebras.md) is

$$
\boxed{Z(A\otimes_kB)=Z(A)\otimes_k Z(B).}
$$

These [tensor products](../../../../../tensor-product.md) are identified with their natural [vector subspaces](../../../../../vector-subspace.md) of $A\otimes_kB$; extending [bases](../../../../../basis.md) justifies these embeddings over the [field](../../../../../field.md) $k$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the introduction to representation theory course of the University of Oxford](../../../../split.md)
6. [Introduction to representation theory course of the University of Oxford](../../../../../introduction-to-representation-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
