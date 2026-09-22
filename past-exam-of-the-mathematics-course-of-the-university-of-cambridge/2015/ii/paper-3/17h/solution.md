<h1 id="17h/solution">Solution</h1>

↑ **Parent:** [17H](../17h.md)

A [simplicial approximation](../../../../../simplicial-approximation.md) to $f:|K|\to|L|$ is a simplicial map $g:K\to L$ satisfying the open-star condition

$$
f(\operatorname{st}_K(v))\subseteq\operatorname{st}_L(g(v))
$$

for every vertex $v$. Equivalently, whenever $f(x)$ lies in the interior of a simplex of $L$, $|g|(x)$ lies in that simplex. In particular $f$ and $|g|$ are joined by the simplexwise straight-line [homotopy](../../../../../homotopy.md).

The [Simplicial approximation theorem](../../../../../simplicial-approximation-theorem.md) says that, for finite $K$, every continuous $f$ has such an approximation after sufficiently many [barycentric subdivisions](../../../../../barycentric-subdivision.md) of $K$. For general complexes one uses a subdivision adapted to the open-star cover; a single uniform number of barycentric subdivisions is the compact-domain version.

Given triangulations $X\cong|K|$, $Y\cong|L|$, choose a simplicial approximation $g$ on a suitable subdivision $K'$. Its [chain map](../../../../../chain-map.md) sends an oriented simplex $[v_0,\ldots,v_r]$ to $[g(v_0),\ldots,g(v_r)]$, with repeated-vertex simplices sent to zero. It commutes with the boundary operator and induces $g_*$. Compose this with the subdivision isomorphism $H_r(K)\to H_r(K')$ and the triangulation identifications to define $f_*:H_r(X)\to H_r(Y)$.

For $z\mapsto z^n$, a positively oriented fundamental loop winds $n$ times around the target circle. With integer coefficients,

$$
\boxed{h_*:H_0(S^1)\to H_0(S^1)\ \hbox{is the identity},\qquad h_*:H_1(S^1)\to H_1(S^1)\ \hbox{is multiplication by }n.}
$$

All higher homology groups vanish. The $H_1$ result can also be read from a subdivision into $n$ copies of a target fundamental cycle.

## ↑ Ancestors (10)

1. [17H](../17h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
