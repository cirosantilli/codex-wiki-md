<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The paper uses $F$ for the [survivor function](../../../../../../survival-function.md), rather than for the [cumulative distribution function](../../../../../../cumulative-distribution-function.md). For a nonnegative [survival time](../../../../../../survival-time.md) $T$ with an absolutely continuous [probability distribution](../../../../../../probability-distribution.md), define

$$
F(t)=\Pr(T>t),\qquad f(t)=-F'(t).
$$

Where $F(t)>0$, the [hazard function](../../../../../../hazard-function.md) is the instantaneous event rate conditional on survival:

$$
h(t)=\lim_{\Delta\downarrow0}\frac{\Pr(t<T\leq t+\Delta\mid T>t)}{\Delta}
=\frac{f(t)}{F(t)}.
$$

The [integrated hazard](../../../../../../cumulative-hazard-function.md) is $H(t)=\int_0^t h(u)\,du$. Since $h=-F'/F$, integration gives $H(t)=\log F(0)-\log F(t)$. With the usual time origin and no event at zero, $F(0)=1$, so

$$
\boxed{H(t)=-\log F(t),\qquad F(t)=e^{-H(t)},\qquad f(t)=h(t)e^{-H(t)}.}
$$

Conversely, differentiating $F=e^{-H}$ gives $F'=-hF$, so these relationships determine each of the [survivor function](../../../../../../survival-function.md), [hazard function](../../../../../../hazard-function.md) and [integrated hazard](../../../../../../cumulative-hazard-function.md) from either of the others. A positive limiting [survivor function](../../../../../../survival-function.md) is possible if the [integrated hazard](../../../../../../cumulative-hazard-function.md) remains finite; a proper finite event time instead has $F(t)\to0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
