<h1 id="5j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual [normal linear model](../../../../../../normal-linear-model.md) $Y=X\beta+\varepsilon$, with fixed full-column-rank design $X\in\mathbb R^{n\times p}$, $n>p$, and $\varepsilon\sim N(0,\sigma^2I_n)$. These [Gaussian distribution](../../../../../../normal-distribution.md) and constant-[variance](../../../../../../variance-split.md) hypotheses are necessary for an exact finite-sample [Student's t-test](../../../../../../student-s-t-test.md). Put $V=(X^TX)^{-1}$ and $\nu=n-p$. The vector of [ordinary least squares estimators](../../../../../../ordinary-least-squares-estimators.md) satisfies

$$
\widehat\beta=(X^TX)^{-1}X^TY,\qquad\boxed{\widehat\beta_0\sim N(\beta_0,\sigma^2V_{00}).}
$$

With $s^2=\|Y-X\widehat\beta\|^2/\nu$, the [test statistic](../../../../../../test-statistic.md) is

$$
\boxed{T=\frac{\widehat\beta_0}{s\sqrt{V_{00}}}.}
$$

Under the [null hypothesis](../../../../../../null-hypothesis.md), $T$ has [Student's t-distribution](../../../../../../student-s-t-distribution.md) with $\nu$ [degrees of freedom](../../../../../../degree-of-freedom.md). A two-sided level-$5\%$ [Student's t-test](../../../../../../student-s-t-test.md) rejects when $|T|>t_{\nu,0.975}$. If the intended test is one-sided against $\beta_0>0$, it rejects when $T>t_{\nu,0.95}$; the [statistical power](../../../../../../statistical-power.md) conclusion below holds for either convention.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5J](../../5j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
