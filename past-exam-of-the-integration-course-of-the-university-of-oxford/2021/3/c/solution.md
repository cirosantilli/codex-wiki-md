<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The a.e. limit $f$ is nonnegative. For a fixed [measurable set](../../../../measurable-set.md) $A$, [Fatou's lemma](../../../../fatou-s-lemma.md) gives $\int_Af\leq\liminf_n\int_Af_n$. Apply the same lemma to $A^c$ and use convergence of the total integrals:

$$
\limsup_n\int_Af_n
=\int_{\mathbb R}f-\liminf_n\int_{A^c}f_n
\leq\int_{\mathbb R}f-\int_{A^c}f=\int_Af.
$$

The lower and upper bounds prove $\boxed{\int_Af_n\to\int_Af}$.

For the asserted [L1 convergence](../../../../convergence-in-l1.md), choose an [integer](../../../../integer-split.md) $k$ so large that $\int_{|x|>k}f<\varepsilon$, possible by [Lebesgue integrability](../../../../integrability.md). The first result applied to this fixed tail [set](../../../../set-split.md) makes $\int_{|x|>k}f_n<2\varepsilon$ eventually. The additional local hypothesis makes $\int_{-k}^k|f_n-f|<\varepsilon$ eventually. Therefore

$$
\int_{\mathbb R}|f_n-f|
\leq\int_{-k}^k|f_n-f|+\int_{|x|>k}f_n+\int_{|x|>k}f<4\varepsilon.
$$

Thus $\boxed{\|f_n-f\|_{L^1(\mathbb R)}\to0}$.

In fact the extra local hypothesis is unnecessary here. [Scheffé's lemma](../../../../scheffe-lemma.md) follows directly from $\min\{f_n,f\}\to f$ [almost everywhere](../../../../almost-everywhere.md) and domination by $f$:

$$
\|f_n-f\|_1=\int f_n+\int f-2\int\min\{f_n,f\}\longrightarrow0.
$$

This stronger argument uses precisely the already assumed nonnegativity, a.e. convergence, and convergence of total integrals.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
