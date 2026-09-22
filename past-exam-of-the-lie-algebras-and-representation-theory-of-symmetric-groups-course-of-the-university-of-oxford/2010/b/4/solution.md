<h1 id="b/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a [Young diagram](../../../../young-diagram.md) cell $(i,j)$, its [hook length](../../../../hook-length.md) is one plus the number of cells to its right and below. The [hook-length formula](../../../../hook-length-formula.md) is

$$
f^\lambda=\frac{n!}{\prod_{(i,j)\in\lambda}h_{ij}}.
$$

Applying it to the two shapes gives

$$
\boxed{f^{(n-2,1,1)}=\frac{(n-1)(n-2)}2,\qquad
f^{(n-2,2)}=\frac{n(n-3)}2.}
$$

The shapes here require $n\ge4$.

A hook [tabloid](../../../../tabloid.md) remembers its first-row set and the ordered singleton entries below it. The proposed map keeps that first-row set and merges the remaining entries into one unordered row. Thus it is well-defined on tabloids. Permuting entries before merging gives the same [tabloid](../../../../tabloid.md) as merging before permuting, so it is a [module](../../../../module-mathematics.md) homomorphism. Every target [tabloid](../../../../tabloid.md) is reached by putting its second-row entries, in any order, into the singleton rows. Therefore it is surjective.

For $r=2$, the strictly dominating partitions of $\lambda=(n-2,1,1)$ are exactly $(n),(n-1,1),(n-2,2)$. Indeed dominance forces the first part to be at least $n-2$, and the possibilities for the remaining sum give precisely those shapes or $\lambda$ itself.

In [characteristic zero](../../../../characteristic-zero.md), [Maschke's theorem](../../../../maschke-s-theorem.md) makes the [permutation module](../../../../permutation-module.md) semisimple, and [Young's rule](../../../../young-s-rule.md) gives one copy of $S^\lambda$ and only strictly dominating additional shapes. The trivial multiplicity is one, since a transitive [permutation module](../../../../permutation-module.md) has a one-dimensional invariant space. For the standard [representation](../../../../group-representation.md) $S^{(n-1,1)}$, [Frobenius reciprocity](../../../../frobenius-reciprocity.md) identifies its multiplicity with the [dimension](../../../../dimension-vector-space.md) of fixed vectors under the row stabilizer $S_{n-2}$. In its realization $\{(z_1,\ldots,z_n):\sum z_i=0\}$, those fixed vectors have the form $(c,\ldots,c,a,b)$ with $(n-2)c+a+b=0$, a two-dimensional space. Thus its multiplicity is two.

Finally $\dim M^\lambda=n(n-1)$. Subtracting the dimensions of one $S^\lambda$, one trivial [module](../../../../module-mathematics.md) and two standard modules leaves $n(n-3)/2$, exactly one $S^{(n-2,2)}$. Therefore

$$
\boxed{M^{(n-2,1,1)}\cong
S^{(n-2,1,1)}\oplus S^{(n)}\oplus2S^{(n-1,1)}\oplus S^{(n-2,2)}.}
$$

The additional multiplicities are $1,2,1$ respectively. If the printed weak summation index is read literally alongside its separate $S^\lambda$, then $m_{\lambda,\lambda}=0$; the total multiplicity of $S^\lambda$ is one.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../split.md)
5. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
