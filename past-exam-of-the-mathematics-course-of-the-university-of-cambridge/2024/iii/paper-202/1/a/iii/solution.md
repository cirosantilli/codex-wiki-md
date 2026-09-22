<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

They are not independent. The [Itô formula](../../../../../../../ito-s-lemma.md) gives $\beta_t^2=t+2\int_0^t\beta_s\,d\beta_s$, and the bilinear [Itô isometry](../../../../../../../ito-isometry.md) therefore gives

$$
\mathbb E[B_t\beta_t^2]=2\int_0^t\mathbb E[\operatorname{sign}(\beta_s)\beta_s]ds=2\int_0^t\mathbb E|\beta_s|ds=\frac43\sqrt{\frac2\pi}\,t^{3/2}>0.
$$

If $B_t$ and $\beta_t$ were [independent random variables](../../../../../../../independent-random-variables.md), then $B_t$ would also be independent of the [measurable function](../../../../../../../measurable-function.md) $\beta_t^2$, and centeredness would instead give $\mathbb E[B_t\beta_t^2]=\mathbb E[B_t]\mathbb E[\beta_t^2]=0$. This contradiction disproves independence.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
