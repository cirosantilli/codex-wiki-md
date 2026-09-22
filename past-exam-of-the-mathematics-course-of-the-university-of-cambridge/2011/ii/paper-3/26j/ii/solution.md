<h1 id="26j/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

To derive the distribution from the infinitesimal characterization, let $p_j(t)=\mathbb P(N(t)=j)$. Independent increments give the forward equations

$$
p_0'=-\lambda(t)p_0,\qquad p_j'=\lambda(t)(p_{j-1}-p_j)\quad(j\geq1).
$$

With $L(t)=\int_0^t\lambda(u)\,du$ and $p_0(0)=1$, $p_j(0)=0$ for $j>0$, these have solution

$$
\boxed{p_j(t)=e^{-L(t)}\frac{L(t)^j}{j!},\qquad N(t)\sim\operatorname{Poisson}(L(t)).}
$$

Substitution verifies each equation, and the probabilities sum to one. Alternatively the [probability generating function](../../../../../../probability-generating-function.md) solves $\partial_tG=\lambda(t)(z-1)G$, $G(z,0)=1$, giving $G=e^{(z-1)L(t)}$. For a general locally integrable rate, time-changing a unit-rate [Poisson process](../../../../../../poisson-process.md) by $L(t)$ gives the same formula.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [26J](../../26j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
