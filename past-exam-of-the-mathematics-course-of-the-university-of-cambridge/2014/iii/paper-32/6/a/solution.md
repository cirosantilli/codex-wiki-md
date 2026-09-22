<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Conditional on an event and the immediately preceding history, [probabilities](../../../../../../probability.md) are proportional to the three instantaneous hazards. Put $w=e^{\beta_0}$. The two zero-covariate subjects each have weight one, and the one-covariate subject has weight $w$. The common [baseline hazard](../../../../../../baseline-hazard.md) cancels. Thus

$$
\boxed{P(z_{\mathrm{event}}=0\mid\text{event, history})=\frac2{2+w},\qquad P(z_{\mathrm{event}}=1\mid\text{event, history})=\frac w{2+w}.}
$$

Each individual with zero covariate has [probability](../../../../../../probability.md) $1/(2+w)$; the first boxed [probability](../../../../../../probability.md) is their combined [probability](../../../../../../probability.md). Conditioning on an event at a specified continuous time can be understood by the limiting conditional event [probabilities](../../../../../../probability.md) in a short interval.

The hazard-weighted covariate mean is $w/(2+w)$, so the [Schoenfeld function](../../../../../../schoenfeld-function.md) at the true coefficient is

$$
s(\beta_0)=\begin{cases}-w/(2+w),&z_{\mathrm{event}}=0,\\2/(2+w),&z_{\mathrm{event}}=1.\end{cases}
$$

Multiplying by the two [conditional probabilities](../../../../../../conditional-probability.md) gives

$$
\boxed{E\{s(\beta_0)\mid\text{event, history}\}=\frac2{2+w}\frac{-w}{2+w}+\frac w{2+w}\frac2{2+w}=0.}
$$

This verifies the score-centering property directly for this [risk set](../../../../../../risk-set.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
