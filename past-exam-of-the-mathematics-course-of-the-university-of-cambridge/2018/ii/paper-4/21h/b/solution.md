<h1 id="21h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Represent a class in $H_k(K)$ by a [chain cycle](../../../../../../chain-cycle.md) $z\in Z_k(K)$. Since every simplex of $K=M\cup N$ belongs to at least one of the two [simplicial subcomplexes](../../../../../../simplicial-subcomplex.md), split the chain in the [simplicial chain complex](../../../../../../simplicial-chain-complex.md) as

$$
z=m+n,
\qquad m\in C_k(M),\quad n\in C_k(N).
$$

Because $\partial z=0$, we have

$$
\partial m=-\partial n.
$$

The left side lies in $C_{k-1}(M)$ and the right side in $C_{k-1}(N)$, so this common chain is supported in $L=M\cap N$. It is a cycle because $\partial^2=0$. The [connecting homomorphism](../../../../../../connecting-homomorphism.md) is therefore

$$
\boxed{\partial_*[z]=[\partial m]=[-\partial n]\in H_{k-1}(L)}.
$$

Changing the decomposition or the representative changes $\partial m$ only by a boundary in $L$, which is why the construction descends to [homology classes](../../../../../../homology-class.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [21H](../../21h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
