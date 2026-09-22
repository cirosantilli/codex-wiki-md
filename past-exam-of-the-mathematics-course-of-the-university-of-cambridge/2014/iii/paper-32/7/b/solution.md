<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Aalen–Johansen estimator](../../../../../../aalen-johansen-estimator.md) of the [cumulative incidence function](../../../../../../cumulative-incidence-function.md), updating the overall [Kaplan–Meier estimator](../../../../../../kaplan-meier-estimator.md) for either event:

$$
\Delta\widehat F_B(t)=\widehat S(t-)\frac{d_B(t)}{Y(t)},\qquad \widehat S(t)=\widehat S(t-)\left[1-\frac{d_A(t)+d_B(t)}{Y(t)}\right].
$$

[Right censoring](../../../../../../right-censoring.md) changes subsequent [risk sets](../../../../../../risk-set.md), not the [survival function](../../../../../../survival-function.md) by itself. Starting with the given estimates at $a_k$, the complete calculation is

$$
\begin{array}{c|c|c|c|c|c}
\text{event time}&Y(t)&\widehat S(t-)&\Delta\widehat F_B(t)&\widehat F_B(t)&\widehat S(t)\\\hline
a_{k+1}&10&0.40&0.40/10=0.04&0.34&0.36\\
a_{k+2}&9&0.36&0&0.34&0.32\\
a_{k+3}&8&0.32&0.32/8=0.04&0.38&0.28
\end{array}
$$

The middle event is of the competing type: it decreases overall survival while leaving the disease [cumulative incidence function](../../../../../../cumulative-incidence-function.md) unchanged at that instant. The event-free intervals leave every estimate and [risk set](../../../../../../risk-set.md) unchanged.

At the final time, both the event subject and the subject censored at that time are in the just-before [risk set](../../../../../../risk-set.md), so its denominator is eight. This is the usual event-before-censoring convention for recorded ties. After the event and [right censoring](../../../../../../right-censoring.md), six subjects remain at risk. Consequently

$$
\boxed{\widehat F_B(a_{k+3})=0.30+0.04+0.04=0.38.}
$$

The nine numbered source items are the inputs to this single calculation, not nine further questions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
