# Gaussian binomial coefficient counts finite-field subspaces

↑ **Parent:** [Gaussian binomial coefficient](gaussian-binomial-coefficient.md)

For a [prime power](prime-power.md) $q$ and $0\leq k\leq n$, count ordered lists of $k$ [linearly independent vectors](linear-independence.md) in $\mathbb F_q^n$. The first has $q^n-1$ choices. After $i$ independent choices, their [linear span](linear-span.md) contains $q^i$ [vectors](vector.md), so the next has $q^n-q^i$ choices. Every $k$-dimensional [vector subspace](vector-subspace.md) has exactly $\prod_{i=0}^{k-1}(q^k-q^i)$ [ordered bases](ordered-basis.md). Dividing the list count by this common multiplicity gives

$$
\#\operatorname{Gr}(k,\mathbb F_q^n)=\frac{\prod_{i=0}^{k-1}(q^n-q^i)}{\prod_{i=0}^{k-1}(q^k-q^i)}=G_{n,k}(q).
$$

The notation $\operatorname{Gr}$ refers to the [Grassmannian](grassmannian.md), here considered simply as the finite collection of these [vector subspaces](vector-subspace.md).[§1.7, Proposition 1.7.2, pp. 63–64](enumerative-combinatorics-volume-1-second-edition-draft-by-richard-stanley.md)

For $n=4,k=2,q=2$, there are $15\cdot14=210$ ordered independent pairs. Each two-dimensional [vector subspace](vector-subspace.md) has $3\cdot2=6$ [ordered bases](ordered-basis.md), leaving $210/6=35$ [vector subspaces](vector-subspace.md). There are only $\binom42=6$ coordinate-selected [vector subspaces](vector-subspace.md); most of the 35 also contain [vectors](vector.md) combining coordinates.

A unique [reduced row echelon form](reduced-row-echelon-form.md) gives another count. Its six possible pivot-column patterns have $4,3,2,2,1,0$ freely chosen entries. Each free entry lies in $\mathbb F_2$, giving $16,8,4,4,2,1$ [vector subspaces](vector-subspace.md), respectively. The diagram fixes the zero entries required to make each pivot the first nonzero entry in its row and the only nonzero entry in its column. Different choices describe different [row spaces](row-space.md).

<a id="image-the-six-reduced-row-echelon-form-pivot-patterns-give-35-two-dimensional-vector-subspaces-of-mathbb-f-2-4"></a>
![](gaussian-binomial-finite-field-subspaces.png)

**[Figure 19](#image-the-six-reduced-row-echelon-form-pivot-patterns-give-35-two-dimensional-vector-subspaces-of-mathbb-f-2-4). The six reduced row echelon form pivot patterns give 35 two-dimensional vector subspaces of $\mathbb F_2^4$**. Original exact matrix-pattern enumeration. A star is a freely chosen [finite field](finite-field.md) entry, while every displayed zero or one is fixed. Pivot columns are numbered from one in this image.

## ↑ Ancestors (6)

1. [Gaussian binomial coefficient](gaussian-binomial-coefficient.md)
2. [Binomial coefficient](binomial-coefficient.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Gaussian binomial coefficient](gaussian-binomial-coefficient.md)
