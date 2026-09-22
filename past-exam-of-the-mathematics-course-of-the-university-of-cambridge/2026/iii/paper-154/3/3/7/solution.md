<h1 id="3/3/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Change variables $x=\lambda_ny$ and use the profiles from part 5:

$$
\int_{\mathbb R^2}|u(t_n,x)|^2\phi(x),dx
=\int_{\mathbb R^2}|v_n(y)|^2\phi(\lambda_ny),dy.
$$

Since $v_n\to Qe^{i\gamma}$ in $L^2$, the difference made by replacing $|v_n|^2$ with $|Q|^2$ tends to zero against the bounded function $\phi(\lambda_n\cdot)$. For each fixed $y$, continuity gives $\phi(\lambda_ny)\to\phi(0)$, and [dominated convergence](../../../../../../../dominated-convergence-theorem.md) then gives

$$
\int|Q(y)|^2\phi(\lambda_ny),dy
\longrightarrow\phi(0)\|Q\|_2^2.
$$

**Thus the mass measures $|u(t_n,x)|^2dx$ converge weakly to the [Dirac delta function](../../../../../../../dirac-delta-function.md) $\|Q\|_2^2\delta_0$.**

## ↑ Ancestors (12)

1. [7](../7.md)
2. [3](../../3.md)
3. [3](../../../3.md)
4. [Paper 154](../../../../paper-154-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
