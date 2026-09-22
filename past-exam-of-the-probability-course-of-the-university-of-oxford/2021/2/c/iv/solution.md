<h1 id="2/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

It suffices that the [moment-generating function](../../../../../moment-generating-function.md) be finite on some open [interval](../../../../../interval-mathematics.md) containing zero:

$$
\boxed{M_Y(t)<\infty\text{ for every }|t|<\delta\text{, for some }\delta>0.}
$$

Equivalently, some two-sided [exponential moment](../../../../../exponential-moment.md) exists: $\mathbb E e^{r|Y|}<\infty$ for some $r>0$. For the forward implication, choose $0<r<\delta$ and use $e^{r|Y|}\leq e^{rY}+e^{-rY}$; the converse follows from $e^{tY}\leq e^{r|Y|}$ for $|t|\leq r$.

Under this weaker hypothesis, all [moments](../../../../../moment.md) exist. For $|t|<r$, [dominated convergence](../../../../../dominated-convergence-theorem.md) justifies the [Taylor series](../../../../../taylor-series.md) argument in (i). Vanishing odd [moments](../../../../../moment.md) gives $M_Y(t)=M_{-Y}(t)$ near zero, and the local [uniqueness theorem for moment-generating functions](../../../../../uniqueness-theorem-for-moment-generating-functions.md) gives the [symmetric distribution](../../../../../symmetric-distribution.md). The reverse implication follows directly from equality of the two [probability distributions](../../../../../probability-distribution-split.md).

More generally, it suffices that all [moments](../../../../../moment.md) exist and the [probability distribution](../../../../../probability-distribution-split.md) have [moment determinacy](../../../../../moment-determinacy.md): $Y$ and $-Y$ then have identical [moments](../../../../../moment.md) and hence identical [probability distributions](../../../../../probability-distribution-split.md). Existence of all [moments](../../../../../moment.md) by itself does not provide that uniqueness.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
