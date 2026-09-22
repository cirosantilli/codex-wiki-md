<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The transverse row sequence in the [extrusion invariance of Loop subdivision](../../../../../../extrusion-invariance-of-loop-subdivision.md) obeys

$$
\boxed{g'_{2j}=\frac{g_{j-1}+6g_j+g_{j+1}}8,\qquad g'_{2j+1}=\frac{g_j+g_{j+1}}2.}
$$

In the convention $g'_k=\sum_j a_{k-2j}g_j$, the centered univariate [subdivision mask](../../../../../../subdivision-mask.md) is

$$
\boxed{(a_{-2},a_{-1},a_0,a_1,a_2)=\frac18(1,4,6,4,1).}
$$

The even coefficients sum to one and the odd coefficients sum to one; the whole binary mask sums to two. Its generating expression is $a(z)=z^{-2}(1+z)^4/8$, identifying the [Cardinal cubic B-spline](../../../../../../cardinal-cubic-b-spline.md) refinement rule. Its limit is $G(y)=\sum_jg_jM_3(y-j)$ for the centered unit-grid cubic basis $M_3$. The curve across rows is this cubic [B-spline](../../../../../../b-spline.md); extrusion generates the whole limit surface. The along-extrusion direction itself has constant height, so its profile is a straight line rather than an additional nonconstant cubic curve.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
