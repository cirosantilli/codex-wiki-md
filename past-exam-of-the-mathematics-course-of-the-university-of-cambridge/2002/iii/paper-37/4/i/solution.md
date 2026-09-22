<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [CUSUM](../../../../../../cusum.md) threshold $h$, define the first signalling time

$$
\tau_h=\inf\{t\geq1:X_t\geq h\}.
$$

The [average run length](../../../../../../average-run-length.md) is $\mathbb E(\tau_h)$ under a specified distribution of the observations and specified initial state, here $X_0=0$. The in-control value $\operatorname{ARL}_0$ is computed under the [null hypothesis](../../../../../../null-hypothesis.md); a large value means false signals occur infrequently. The out-of-control value $\operatorname{ARL}_A$ is computed under a specified [alternative hypothesis](../../../../../../alternative-hypothesis.md); a small value means rapid detection when that alternative holds from monitoring's start. If a change occurs later, its detection delay depends also on the chart state at change time, so the zero-state alternative [average run length](../../../../../../average-run-length.md) is not every possible delay.

A fixed-horizon [statistical hypothesis test](../../../../../../statistical-hypothesis-test.md) is characterized by [Type I error](../../../../../../type-i-and-type-ii-errors.md) probability under its null and [Type II error](../../../../../../type-i-and-type-ii-errors.md) probability under a specified alternative. Continuous monitoring repeatedly offers opportunities to signal: over an indefinitely long run its probability of eventually signalling can be one even under the null. The [average run length](../../../../../../average-run-length.md) quantifies waiting time rather than that eventual probability. It replaces the single-test emphasis on a false-rejection probability with a false-signal timescale, and compares detection speed rather than only a fixed-horizon miss probability. However, a mean run length alone does not determine either finite-horizon error probability; those require the run-length distribution.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
