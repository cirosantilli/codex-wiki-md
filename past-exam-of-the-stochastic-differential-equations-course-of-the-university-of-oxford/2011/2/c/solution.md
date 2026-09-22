<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Work modulo [indistinguishability of stochastic processes](../../../../indistinguishability-of-stochastic-processes.md), with norm $\|M\|=(\mathbb E|M_t|^2)^{1/2}$. It is a genuine norm: zero terminal value implies $M_s=\mathbb E[M_t\mid\mathcal F_s]=0$ at every fixed time, and continuity extends equality from countably many rational times to all times simultaneously.

Let $M^j$ be a Cauchy sequence in this norm. Choose a subsequence with $\|M^{j_{n+1}}-M^{j_n}\|<2^{-n}$. Part (b) applies to these difference martingales, so their telescoping series converges uniformly almost surely. Its limit has continuous paths. At each time $s$, conditional-expectation contractivity gives

$$
\|M^j_s-M^k_s\|_2\leq\|M^j_t-M^k_t\|_2,
$$

so the fixed-time limit also exists in $L^2$ and agrees with the pathwise limit. It has an adapted version obtained by taking the finite pointwise subsequence limit when it exists, and zero otherwise. Each such definition is measurable at its own time, and the almost surely uniform limit gives continuous paths. Passing to the $L^2$ limit in $\mathbb E[M^j_v\mid\mathcal F_s]=M^j_s$ shows that the limit is a martingale. The original Cauchy sequence converges to it in terminal norm. Thus **the space is complete**.

Part (b) supplies what fixed-time $L^2$ completeness alone does not: a single full-probability set on which a subsequence converges uniformly in time, preserving path continuity. This is [completeness of continuous square-integrable martingales](../../../../completeness-of-continuous-square-integrable-martingales.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the stochastic differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic differential equations course of the University of Oxford](../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
