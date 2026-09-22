<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [clique count in a binomial random graph](../../../../../../clique-count-in-a-binomial-random-graph.md), write

$$
\mu_r=\mathbb EX_r=\binom nr2^{-\binom r2},\qquad L=\log_2n.
$$

Fix $0<\varepsilon<1$. At $r_- =\lfloor(2-\varepsilon)L\rfloor$, the estimates $\binom nr\geq(n/r)^r$ and $r=O(L)$ give

$$
\log_2\mu_{r_-}\geq r_-L-\frac{r_-(r_--1)}2-r_-\log_2r_-
=\left(\varepsilon-\frac{\varepsilon^2}{2}\right)L^2-O(L\log L).
$$

This eventually exceeds $(9/5)L$. At $r_+=\lceil(2+\varepsilon)L\rceil$, the upper bound $\binom nr\leq n^r$ instead gives

$$
\log_2\mu_{r_+}\leq-\left(\varepsilon+\frac{\varepsilon^2}{2}\right)L^2+O(L),
$$

so $\mu_{r_+}<n^{9/5}$. Moreover

$$
\frac{\mu_{r+1}}{\mu_r}=\frac{n-r}{r+1}\,2^{-r}<1\qquad(r\geq r_+),
$$

so no later [clique](../../../../../../clique-graph-theory.md) size can regain the threshold. The maximum defining $r_0$ exists for sufficiently large $n$, since $\mu_2=\binom n2/2\geq n^{9/5}$ then. We have $r_-\leq r_0<r_+$. Letting $\varepsilon$ decrease to zero proves **the asymptotic size**:

$$
\boxed{r_0=(2+o(1))\log_2n.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
