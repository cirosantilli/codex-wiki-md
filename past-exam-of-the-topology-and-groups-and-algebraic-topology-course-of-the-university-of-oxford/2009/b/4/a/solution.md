<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $n\geq1$, the integral [singular homology](../../../../../singular-homology.md) of the [sphere](../../../../../sphere.md) is $H_0(S^n)=\mathbb Z$, $H_n(S^n)=\mathbb Z$, and zero in other degrees. For $S^0$ there are two components, so $H_0(S^0)=\mathbb Z^2$. Choose an [orientation](../../../../../orientation-of-a-simplex.md) generator $[S^n]$ for positive dimension. The [degree of a map](../../../../../degree-of-a-continuous-mapping.md) is the integer satisfying

$$
\boxed{f_*[S^n]=\deg(f)[S^n]}.
$$

To define a [local degree of a continuous map](../../../../../local-degree-of-a-continuous-map.md) at $x$ over $y=f(x)$, require $x$ to be isolated in that fibre. A small neighbourhood $U$ contains no other preimage of $y$, so $f$ maps $(U,U\setminus\{x\})$ to $(S^n,S^n\setminus\{y\})$. By [excision](../../../../../excision-theorem.md) their local top homology groups are both $\mathbb Z$, with generators fixed by the orientations. Multiplication by an integer in this induced map defines $\deg_xf$. Without fibre isolation, this particular local-degree definition is not in general available.

If $f^{-1}(y)=\{x_1,\ldots,x_r\}$ is finite, the local-degree formula is

$$
\boxed{\deg(f)=\sum_{j=1}^r\deg_{x_j}f}.
$$

Indeed [excision](../../../../../excision-theorem.md) identifies $H_n(S^n,S^n\setminus f^{-1}(y))$ with the direct sum of the local groups at the $x_j$. The global [fundamental class](../../../../../fundamental-class.md) maps to the vector of their local [orientation](../../../../../orientation-of-a-simplex.md) generators, namely $(1,\ldots,1)$. Naturality of the map of pairs sends that vector to $\sum_j\deg_{x_j}f$ in the local group at $y$. The other route through the naturality diagram sends the global class by $f_*$ first and therefore gives $\deg(f)$. The map from the target [sphere](../../../../../sphere.md)'s top homology to its [local homology](../../../../../local-homology.md) is an [isomorphism](../../../../../isomorphism.md), so the two integers agree. Empty fibres give degree zero by the same argument. Standard approximation by a homotopic smooth map permits the formula to be used with regular values when an original continuous map has no convenient finite fibre.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the topology and Groups and Algebraic Topology course of the University of Oxford](../../../../split.md)
6. [Topology and Groups and Algebraic Topology course of the University of Oxford](../../../../../topology-and-groups-and-algebraic-topology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
