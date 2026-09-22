<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At time $x_i$, the observed number of events is $v_i$ and the exposure to the common instantaneous hazard is the risk-set size $n-i+1$. The likelihood score for a hazard increment therefore equates observed and expected events:

$$
v_i=(n-i+1)\,d\widehat H(x_i).
$$

Thus the [Nelson–Aalen estimator](../../../../../../../nelson-aalen-estimator.md) is

$$
\widehat H(t)
=\sum_{i:x_i\leq t}\frac{v_i}{n-i+1}.
$$

It estimates the [cumulative hazard function](../../../../../../../cumulative-hazard-function.md) by adding event count divided by current exposure at every observed event time.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
