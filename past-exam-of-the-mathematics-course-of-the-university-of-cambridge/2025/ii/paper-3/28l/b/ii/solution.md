<h1 id="28l/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\delta'$ be any decision rule. For every $j$,

$$
\sup_{\theta\in\Theta}R(\theta,\delta')
\geq
\int_\Theta R(\theta,\delta')\,\pi_j(d\theta)
\geq r_j,
$$

because $r_j$ is the infimum of the integrated risk under $\pi_j$. Taking the lower limit gives

$$
\sup_\theta R(\theta,\delta')\geq
\lim_{j\to\infty}r_j=r.
$$

The given rule $\delta$ has constant risk $r$, and hence worst-case risk exactly $r$. It attains this universal lower bound and is therefore minimax. This is the [constant-risk limit-of-Bayes-risk criterion](../../../../../../../constant-risk-limit-of-bayes-risk-criterion.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [28L](../../../28l.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
