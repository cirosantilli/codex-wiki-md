<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**Yes.** The preceding calculation established $\mathbb E L_\tau=-2ab/(b-a)<\infty$. For every $n$, the stopped [martingale](../../../../../martingale-split.md) satisfies

$$
|M_{n\wedge\tau}|
\leq |S_{n\wedge\tau}|+L_{n\wedge\tau}
\leq C+L_\tau=:H,
\qquad C=\max\{-a,b\}.
$$

Here $H$ is a single nonnegative [integrable random variable](../../../../../integrable-random-variable.md) that bounds the whole family. Thus, for any $K>0$,

$$
\sup_n\mathbb E\!\left[|M_{n\wedge\tau}|\mathbf1_{\{|M_{n\wedge\tau}|>K\}}\right]
\leq\mathbb E[H\mathbf1_{\{H>K\}}]\longrightarrow0.
$$

The last limit follows from the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md). This is precisely [uniform integrability](../../../../../uniform-integrability.md). It also gives $M_{n\wedge\tau}\to M_\tau=|S_\tau|-L_\tau$ with [convergence in L1](../../../../../convergence-in-l1.md), and therefore $\mathbb EM_\tau=0$, consistently with the preceding answer. A common bound on the individual [expected values](../../../../../expected-value-split.md) alone would not have sufficed; the [integrable](../../../../../integrability.md) dominating [random variable](../../../../../random-variable-split.md) is what supplies control of every tail.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
