<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Write $G=G^{(0)}(\tau-\tau')$ and $g_0=G^{(0)}(0)$. With two identical degree-$n$ [vertices](../../../../vertex-graph-theory.md), let $r$ lines join them. The remaining $n-r$ half-edges on each [vertex](../../../../vertex-graph-theory.md) form self-loops. Both $n$ and $r$ are even. The number of [Wick contractions](../../../../wick-contraction.md) is

$$
N_{n,r}=\binom nr^2r!\bigl[(n-r-1)!!\bigr]^2,
$$

since one chooses and matches the joining half-edges and then pairs the rest independently. Dividing by the expansion denominator $2!(n!)^2$ gives every [symmetry factor](../../../../feynman-diagram-symmetry-factor.md) weight without guessing graph multiplicities.

For two quartic [vertices](../../../../vertex-graph-theory.md), $r=0,2,4$ gives

$$
\boxed{\left.\frac Z{Z_0}\right|_{\lambda^2}
=\lambda^2\int_0^\beta d\tau\,d\tau'\left[\frac{g_0^4}{128}+\frac{g_0^2G^2}{16}+\frac{G^4}{48}\right].}
$$

The graphs are respectively the product of two first-order two-loop graphs; two [vertices](../../../../vertex-graph-theory.md) joined by two lines with one self-loop on each; and two [vertices](../../../../vertex-graph-theory.md) joined by four lines with no self-loops.

For two sextic [vertices](../../../../vertex-graph-theory.md), $r=0,2,4,6$ gives

$$
\boxed{\left.\frac Z{Z_0}\right|_{\mu^2}
=\mu^2\int_0^\beta d\tau\,d\tau'\left[\frac{g_0^6}{4608}+\frac{g_0^4G^2}{256}
+\frac{g_0^2G^4}{192}+\frac{G^6}{1440}\right].}
$$

The corresponding numbers of self-loops on each [vertex](../../../../vertex-graph-theory.md) are $3,2,1,0$. All seven second-order graphs are drawn in [solution](../e/solution.md); in each series the $r=0$ graph is disconnected and the others are connected.

For completeness, a mixed quartic-sextic pair, not needed for the two pure second-order coefficients, contributes

$$
\left.\frac Z{Z_0}\right|_{\lambda\mu}=\lambda\mu\int_0^\beta d\tau\,d\tau'
\left[\frac{g_0^5}{384}+\frac{g_0^3G^2}{32}+\frac{g_0G^4}{48}\right].
$$

Taking $\log Z$ removes the products of first-order graphs, that is, the $r=0$ terms. The requested [partition function](../../../../canonical-partition-function.md) retains them.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../e/solution.md)
