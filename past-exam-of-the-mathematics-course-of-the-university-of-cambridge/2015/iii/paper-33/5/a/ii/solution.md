<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a continuous positive [survival time](../../../../../../../survival-time.md), $S'(t)=-f(t)$ and the [hazard function](../../../../../../../hazard-function.md) is $h(t)=f(t)/S(t)$ wherever $S(t)>0$. Therefore

$$
\frac{d}{dt}\log S(t)=-h(t).
$$

Since $S(0)=1$, integrating gives the [cumulative hazard function](../../../../../../../cumulative-hazard-function.md) identity

$$
\boxed{S(t)=\exp\{-H(t)\},\qquad H(t)=\int_0^t h(u)\,du.}
$$

At an endpoint where survival reaches zero, the corresponding cumulative hazard is interpreted as $+\infty$ and the exponential as zero.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 33](../../../../paper-33-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
