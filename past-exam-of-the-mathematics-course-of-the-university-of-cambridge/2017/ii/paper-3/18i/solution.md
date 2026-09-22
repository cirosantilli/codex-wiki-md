<h1 id="18i/solution">Solution</h1>

↑ **Parent:** [18I](../18i.md)

Use [singular homology](../../../../../singular-homology.md) with [integer](../../../../../integer.md) coefficients. The [Künneth theorem](../../../../../kunneth-theorem.md) for triangulable spaces gives a split short exact [sequence](../../../../../sequence.md) with tensor terms $\bigoplus_{i+j=k}H_i(X)\otimes H_j(Y)$ and torsion terms $\bigoplus_{i+j=k-1}\operatorname{Tor}_1(H_i(X),H_j(Y))$. When one factor's [homology groups](../../../../../homology-group.md) are free abelian, the torsion terms vanish and the tensor map is an [isomorphism](../../../../../isomorphism.md).

The [circle](../../../../../circle.md) has $H_0(S^1)=H_1(S^1)=\mathbb Z$ and all other [groups](../../../../../group-split.md) zero. Inductively, the [homology groups](../../../../../homology-group.md) of a [torus](../../../../../torus.md) are free, and

$$
 H_k(T^{n-1}\times S^1)\cong H_k(T^{n-1})\oplus H_{k-1}(T^{n-1}).
$$

Pascal's identity gives

$$
\boxed{H_k(T^n;\mathbb Z)\cong\mathbb Z^{\binom nk}\quad(0\leq k\leq n),\qquad H_k=0\quad(k>n).}
$$

Geometrically the generators correspond to choosing $k$ of the $n$ [circle](../../../../../circle.md) factors and taking their product, consistent with the cellular model having one $k$-cell for each such [subset](../../../../../subset.md) and cancelling opposite boundary faces.

## ↑ Ancestors (10)

1. [18I](../18i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
