<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take the [stopping times](../../../../../../stopping-time.md)

$$
\boxed{S_n=\inf\{t\geq0:|M_t|\geq n\},\qquad\inf\varnothing=\infty.}
$$

Continuity gives $|M_{t\wedge S_n}|\leq n$, with no overshoot at the first crossing. Stopping preserves the [local martingale](../../../../../../local-martingale.md) property, and the bounded case proved in question 4(i) makes each $M^{S_n}$ a continuous true [martingale](../../../../../../martingale-split.md).

Every continuous path is bounded on each compact time interval, so $S_n\uparrow\infty$ [almost surely](../../../../../../almost-sure-convergence.md). Hence this is also a [localizing sequence](../../../../../../localizing-sequence.md) consisting of bounded stopped [martingales](../../../../../../martingale-split.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
