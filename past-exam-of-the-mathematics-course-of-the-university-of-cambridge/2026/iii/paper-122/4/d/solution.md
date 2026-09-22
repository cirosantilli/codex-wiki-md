<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $N=C(\log k)2^k$ and red-blue colour $K_N$. Across an equal bipartition, one colour has density at least $1/2$. Repeated [common-neighbourhood sampling](../../../../../../common-neighbourhood-sampling-bound.md), with

$$
t=k-C_0\log k,
$$

finds distinct vertices $x_1,\ldots,x_t$ whose common neighbourhood in one colour has size at least

$$
c2^{-t}N
=cC(\log k)2^{k-t},
$$

which is a sufficiently large polynomial in $k$ when $C_0$ is fixed and large.

Apply the [complete-bipartite Ramsey completion lemma](../../../../../../complete-bipartite-ramsey-completion-lemma.md) to this polynomial-size common neighbourhood. The lemma iterates the same averaging argument for the remaining $C_0\log k$ vertices: either they extend $x_1,\ldots,x_t$ to one side of a $K_{k,k}$ in the first colour, or their failed extensions have enough edges in the other colour to form a $K_{k,k}$ there. Taking $C_0$ and then $C$ sufficiently large therefore forces a monochromatic $K_{k,k}$. Consequently

$$
\boxed{R(K_{k,k})=O((\log k)2^k).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
