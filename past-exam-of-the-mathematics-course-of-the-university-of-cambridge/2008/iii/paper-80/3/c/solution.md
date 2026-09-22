<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [fourth-order two-stage Gauss collocation method](../../../../../../fourth-order-two-stage-gauss-collocation-method.md), $b_1=b_2=1/2$, $a_{11}=a_{22}=1/4$, $a_{12}=1/4-\sqrt3/6$ and $a_{21}=1/4+\sqrt3/6$. The weights are positive. For the matrix defining [algebraic stability](../../../../../../algebraic-stability-of-a-runge-kutta-method.md),

$$
m_{11}=m_{22}=2(1/2)(1/4)-(1/2)^2=0,
$$

and

$$
m_{12}=m_{21}=\frac12\left(\frac14-\frac{\sqrt3}6\right)
+\frac12\left(\frac14+\frac{\sqrt3}6\right)-\frac14=0.
$$

Hence **$M=0$ is positive semidefinite, so the method is algebraically stable**. Its two-stage contractivity estimate follows from part (b). The PDF has $a_{22}=1/4$; the extra $\sqrt3/6$ attached to that entry in the converted TeX is a transcription error.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
