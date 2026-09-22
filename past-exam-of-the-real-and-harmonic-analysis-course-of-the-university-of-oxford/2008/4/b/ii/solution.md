<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [first-crossing maximal inequality for refining partitions](../../../../../first-crossing-maximal-inequality-for-refining-partitions.md) follows from countable disjointness and the strict average bound:

$$
\mu(\{\widetilde Mf>t\})=\sum_{M\in\mathcal S_t}\mu(M)\leq\frac1t\sum_{M\in\mathcal S_t}\int_M|f|\,d\mu\leq\frac{\|f\|_1}t.
$$

Thus **this partition maximal operator has weak-type constant one**.

The conclusion of [differentiation along refining metric partitions](../../../../../differentiation-along-refining-metric-partitions.md) is

$$
\boxed{\lim_{k\to\infty}\frac1{\mu(M_k(x))}\int_{M_k(x)}|f(y)-f(x)|d\mu(y)=0\quad\text{for }\mu\text{-almost every }x.}
$$

The crucial geometric property is **shrinking [diameter](../../../../../diameter.md)**, not merely refinement: since $x\in M_k(x)$ and $\operatorname{diam}M_k(x)<1/k$, continuity makes the corresponding oscillation tend to zero for every continuous test function. Continuous $L^1$ approximation and the maximal inequality then transfer this to $f$, exactly as before: the exceptional-set bound is $2\|f-g\|_1/\varepsilon$ for an oscillation threshold $2\varepsilon$. Countability makes the maximal function measurable, and positive cell [measure](../../../../../measure-split.md) makes every average defined. Refinement supplied the disjoint first-crossing argument; shrinking [diameter](../../../../../diameter.md) supplies differentiation.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../../split.md)
6. [Real and harmonic analysis course of the University of Oxford](../../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
