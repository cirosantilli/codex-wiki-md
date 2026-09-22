<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [uniformly integrable martingale convergence theorem](../../../../../uniformly-integrable-martingale-convergence-theorem.md) states that a [uniformly integrable](../../../../../uniform-integrability.md) [martingale](../../../../../martingale-split.md) $(U_n)$ has an [integrable](../../../../../integrability.md) terminal [random variable](../../../../../random-variable-split.md) $U_\infty$ such that $U_n\to U_\infty$ [almost surely](../../../../../almost-sure-convergence.md) and in the [L1 norm](../../../../../l1-norm.md), and

$$
U_n=\mathbb E[U_\infty\mid\mathcal F_n].
$$

The last identity follows by passing to the [limit of a sequence](../../../../../limit-of-a-sequence.md) in $\mathbb E[U_m\mathbf1_A]=\mathbb E[U_n\mathbf1_A]$ for $A\in\mathcal F_n$ and $m\geq n$, using [convergence in L1](../../../../../convergence-in-l1.md).

Part (b)(iii) verifies [uniform integrability](../../../../../uniform-integrability.md) for $(Z_n)$, so

$$
\boxed{Z_n\longrightarrow Z_\infty\quad\text{almost surely and in }L^1,\qquad
Z_n=\mathbb E[Z_\infty\mid\mathcal F_n].}
$$

Moreover $|Z_\infty|\leq L$ [almost surely](../../../../../almost-sure-convergence.md). In this particular problem the common bound also yields [convergence in Lp](../../../../../convergence-in-lp.md) for every finite $p\geq1$, including [convergence in L2](../../../../../convergence-in-l2.md): the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) applies to $|Z_n-Z_\infty|^p\leq(2L)^p$. General [uniform integrability](../../../../../uniform-integrability.md) alone does not assert these higher-power conclusions.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
