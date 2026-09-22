<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $k=p^{3p}$. Parts ii and iii give a graph with neither a [clique](../../../../../../clique-graph-theory.md) nor an [independent set](../../../../../../independent-set-graph-theory.md) of size $k$. Its number of vertices satisfies the standard binomial lower bound

$$
\binom{p^3}{p^2}
\geq\left(\frac{p^3}{p^2}\right)^{p^2}
=p^{p^2}.
$$

Consequently the [modular-intersection graph Ramsey lower bound](../../../../../../modular-intersection-graph-ramsey-lower-bound.md) gives

$$
\boxed{R(k,k)\geq p^{p^2}}.
$$

For every fixed $C>0$,

$$
\log(p^{p^2})=p^2\log p,
\qquad
\log(k^C)=3Cp\log p.
$$

The first quantity exceeds the second when $p>3C$. Thus $p^{p^2}$ is eventually larger than $k^C$ for every fixed $C$, so this lower bound grows faster than every [polynomial](../../../../../../polynomial-split.md) in $k$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 161](../../../paper-161-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
