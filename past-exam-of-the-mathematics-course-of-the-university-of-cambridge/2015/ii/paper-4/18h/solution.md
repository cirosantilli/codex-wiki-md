<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

The [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md) for $K=M\cup N$ is the [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md)

$$
\cdots\to H_n(M\cap N)\xrightarrow{(i_*,-j_*)}H_n(M)\oplus H_n(N)\xrightarrow{k_*+l_*}H_n(K)\xrightarrow{\partial_n}H_{n-1}(M\cap N)\to\cdots.
$$

We use integer coefficients. A [simplicial cycle](../../../../../simplicial-cycle.md) $c$ in $K$ can be written $c=m+n$ with chains in $M,N$. Since $\partial m=-\partial n$, this chain lies in $M\cap N$ and is a cycle. Define $\partial_n[c]=[\partial m]$; changing the splitting or the cycle representative changes this by a boundary, giving a well-defined [connecting homomorphism](../../../../../connecting-homomorphism.md).

First consider two acyclic subcomplexes. Their intersection is either empty or acyclic. If empty, positive-degree [homology](../../../../../homology-split.md) of their disjoint union vanishes. If nonempty, the reduced [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md) implies the same conclusion, including degree one since the intersection has zero reduced $H_0$. This proves the claim for two subcomplexes.

Inductively let $U=M_1\cup\cdots\cup M_{n-1}$, $V=M_n$, and $W=U\cap V=\bigcup_{i<n}(M_i\cap M_n)$. Discard empty members as necessary. Both $U$ and $W$ satisfy the same intersection hypothesis with at most $n-1$ members, so their homology vanishes in degrees at least $n-2$. The exact segment $H_i(U)\oplus H_i(V)\to H_i(K)\to H_{i-1}(W)$ then gives $\boxed{H_i(K)=0\text{ for }i\geq n-1}$. For $n\geq3$ these degrees are positive and the induction applies directly; empty $W$ again means a disjoint union.

For sharpness, take the boundary of an $(n-1)$-simplex, covered by its $n$ facets. Every nonempty proper intersection of facets is a simplex and thus has the [homology of a point](../../../../../acyclic-space.md); the intersection of all facets is empty. The union is a [sphere](../../../../../sphere.md) $S^{n-2}$ and $H_{n-2}$ is nonzero. For $n=2$ it is two isolated vertices and $H_0\cong\mathbb Z^2$; for $n\geq3$, $H_{n-2}\cong\mathbb Z$. **The degree bound cannot be lowered.**

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
