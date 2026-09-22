<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let

$$
v=p_1(1-p_1)+p_0(1-p_0),
\qquad I_j=\frac{m_j}{v},
$$

where $m_j$ is the cumulative sample size per arm. The [canonical joint distribution for group sequential test statistics](../../../../../../canonical-joint-distribution-for-group-sequential-test-statistics.md) is

$$
\begin{pmatrix}Z_1\\Z_2\end{pmatrix}
\dot\sim N_2\!\left[
\begin{pmatrix}\delta\sqrt{I_1}\\\delta\sqrt{I_2}\end{pmatrix},
\begin{pmatrix}
1&\sqrt{I_1/I_2}\\
\sqrt{I_1/I_2}&1
\end{pmatrix}
\right].
$$

**Thus $\operatorname{Corr}(Z_1,Z_2)=\sqrt{m_1/m_2}$. This correlation arises because the second statistic reuses all first-stage observations.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
