<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [Bayes' theorem](../../../../../../bayes-theorem.md) with the individual [survivor function](../../../../../../survival-function.md). Writing $z=\theta t^2/2$, the [frailty distribution among survivors](../../../../../../frailty-distribution-among-survivors.md) has density

$$
g(u\mid T>t)=\frac{e^{-uz}e^{-u}}{\overline S(t)}=(1+z)e^{-(1+z)u}\quad(u\geq0).
$$

Hence

$$
\boxed{U\mid T>t\sim\operatorname{Exp}(1+\theta t^2/2),\qquad \mathbb E[U\mid T>t]=\frac1{1+\theta t^2/2}.}
$$

The [conditional expectation](../../../../../../conditional-expectation.md) starts at one and declines toward zero when $\theta>0$. Survival favors the less frail individuals, precisely explaining why the [population hazard under exponential frailty](../../../../../../population-hazard-under-exponential-frailty.md) equals $h_0(t)$ times a decreasing multiplier. The original PDF asks for conditioning on the event $T>t$; the TeX's misplaced inequality is a transcription error, not conditioning on an observed exact event time.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
