<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use $\mathbb N=\{1,2,\ldots\}$. First recall the [Ramsey theorem for r-sets](../../../../../../ramsey-s-theorem.md) in its infinite form: every finite colouring of the $r$-element subsets of an infinite countable set has an infinite homogeneous subset. Here is a proof, so the combinatorial input is explicit.

For $r=1$, this is the [infinite pigeonhole principle](../../../../../../infinite-pigeonhole-principle.md). Suppose it holds for $r$. Given a colouring of $(r+1)$-sets, choose a first point $a_1$. Colour the $r$-sets in the remaining tail by adjoining $a_1$, and use the induction hypothesis to obtain an infinite tail on which that colouring is constant, with colour $d_1$. Choose $a_2$ from that tail and repeat, always thinning the unused tail. This produces increasing $a_i$, nested infinite reservoirs containing all later selected points, and colours $d_i$ such that every $(r+1)$-set of selected points whose least point is $a_i$ has colour $d_i$. Infinitely many $d_i$ are equal. Keeping the corresponding points gives an infinite homogeneous subset. This is a [successive thinning proof of the infinite Ramsey theorem](../../../../../../successive-thinning-proof-of-the-infinite-ramsey-theorem.md).

Now let $\chi$ be the given finite colouring of positive integers. Colour each unordered pair $\{a,b\}$, with $a<b$, by $\chi(a+2b)$. Apply the proved theorem with $r=2$, and enumerate its homogeneous set increasingly as $x_1<x_2<\cdots$. Then

$$
\boxed{\chi(x_i+2x_j)=\gamma\quad\text{for all }i<j}
$$

for one fixed colour $\gamma$. This proves the requested monochromatic pattern without requiring the $x_i$ themselves to have that colour.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
