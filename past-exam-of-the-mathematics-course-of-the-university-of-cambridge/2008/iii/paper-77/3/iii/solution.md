<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use unit knot spacing and the centered [Cardinal cubic B-spline](../../../../../../cardinal-cubic-b-spline.md) convention $C(t)=\sum_iP_iM_3(t-i)$, where $M_3$ is supported on $[-2,2]$. On the span $[i,i+1]$, with $s=t-i$, the active control points are $P_{i-1},P_i,P_{i+1},P_{i+2}$, and their [B-spline](../../../../../../b-spline.md) weights are

$$
(b_0,b_1,b_2,b_3)=\frac16\big((1-s)^3,\;3s^3-6s^2+4,\;-3s^3+3s^2+3s+1,\;s^3\big).
$$

For $t=11/4$, take $i=2$, $s=3/4$. The weights and their [derivatives](../../../../../../derivative.md) are

$$
(b_0,b_1,b_2,b_3)=\frac1{384}(1,121,235,27),\qquad (b'_0,b'_1,b'_2,b'_3)=\frac1{32}(-1,-21,13,9).
$$

The PDF has $P_3=(0,0,0)$ and $P_4=(0,1,0)$, so the point and [tangent vector](../../../../../../tangent-vector.md) are

$$
C(11/4)=\frac{P_1+121P_2+235P_3+27P_4}{384},\qquad C'(11/4)=\frac{-P_1-21P_2+13P_3+9P_4}{32}.
$$

Thus, under this centered convention,

$$
\boxed{C(11/4)=\left(\frac{61}{192},\frac7{96},\frac{61}{192}\right),\qquad C'(11/4)=\left(-\frac{11}{16},\frac14,-\frac{11}{16}\right).}
$$

The original PDF specifies neither the knot origin nor its indexing relative to $P_i$. If instead the convention associates span $[i,i+1]$ with $P_i,P_{i+1},P_{i+2},P_{i+3}$, the identical local weights multiply $P_2,P_3,P_4,P_5$ at the requested parameter, giving

$$
\boxed{C(11/4)=\left(-\frac{13}{192},\frac{131}{192},\frac7{96}\right),\qquad C'(11/4)=\left(-\frac5{16},\frac{11}{16},\frac14\right).}
$$

These are parameter translations of the same uniform construction, rather than contradictory evaluations with the same knots. A specified knot convention is necessary to select the numerical pair uniquely; changing the knot spacing would also rescale the [derivative](../../../../../../derivative.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
