<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The terminal bracket value printed as zero is incompatible with a strictly increasing bracket starting at zero. If the intended value is infinity, [solution](../a/solution.md) applies directly. In fact the substantive conclusion holds for every deterministic continuous bracket $a(t)=[M]_t$, whether its terminal value is finite or infinite, and without strict increase.

For $u\in\mathbb R$, the [Itô formula](../../../../../../ito-s-lemma.md) makes

$$
Z_t=\exp\bigl(iuM_t+\tfrac12u^2a(t)\bigr)
$$

a complex [local martingale](../../../../../../local-martingale.md). Its modulus is the deterministic value $e^{u^2a(t)/2}$, bounded on every finite horizon, so its real and imaginary parts are true [martingales](../../../../../../martingale-split.md) there. Conditioning between $s$ and $t$ gives

$$
\boxed{\mathbb E[e^{iu(M_t-M_s)}\mid\mathcal F_s]
=\exp\bigl(-\tfrac12u^2(a(t)-a(s))\bigr)}.
$$

This deterministic [conditional characteristic function](../../../../../../conditional-characteristic-function.md) shows that the increment is independent of $\mathcal F_s$ and is normal with mean zero and variance $a(t)-a(s)$. Induction over ordered times gives independent Gaussian increments and hence jointly Gaussian coordinate vectors. Since $a(t)$ is finite at every finite time, the [integrable terminal bracket criterion](../../../../../../integrable-terminal-bracket-criterion.md) applied on each fixed horizon also upgrades $M$ to a true square-integrable [martingale](../../../../../../martingale-split.md). This proves the [deterministic quadratic variation characterizes a Gaussian continuous local martingale](../../../../../../deterministic-quadratic-variation-characterizes-a-gaussian-continuous-local-martingale.md) result in a form covering the corrected question.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
