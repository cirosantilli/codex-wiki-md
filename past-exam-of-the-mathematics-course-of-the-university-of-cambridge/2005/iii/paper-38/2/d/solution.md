<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the [integrable terminal bracket criterion](../../../../../../integrable-terminal-bracket-criterion.md), assume $M_0=0$, or more generally $M_0\in L^2$. This initial-value assumption is necessary if it is not already part of the notation: an integrable but non-square-integrable random constant process has zero [quadratic variation](../../../../../../quadratic-variation.md) and still fails square-integrability.

For the zero-starting case, choose a [localizing sequence](../../../../../../localizing-sequence.md) $\tau_n$ bounding both $|M|$ and its [quadratic variation](../../../../../../quadratic-variation.md). The stopped processes are true square-integrable [martingales](../../../../../../martingale-split.md), and the [Itô isometry](../../../../../../ito-isometry.md) gives

$$
\mathbb E[M_{t\wedge\tau_n}^2]=\mathbb E[M]_{t\wedge\tau_n}\le C:=\mathbb E[M]_\infty<\infty.
$$

For each fixed time these variables are [uniformly integrable](../../../../../../uniform-integrability.md) by their bounded second moments. Almost sure convergence as $n\to\infty$ is therefore convergence in $L^1$. Passing to the limit in the stopped conditional-expectation identity gives $\mathbb E[M_t\mid\mathcal F_s]=M_s$: the [local martingale](../../../../../../local-martingale.md) is a true [martingale](../../../../../../martingale-split.md). The [Fatou lemma](../../../../../../fatou-s-lemma.md) also gives

$$
\boxed{\sup_{t\ge0}\mathbb EM_t^2\le\mathbb E[M]_\infty<\infty},
$$

so $M$ belongs to the global $\mathcal M_c^2$ space. For general square-integrable $M_0$, apply this argument to $M-M_0$ and use $|M_t|^2\le2|M_0|^2+2|M_t-M_0|^2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
