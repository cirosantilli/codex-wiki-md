<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $t\in\mathbb R$. The [mean value theorem](../../../../../mean-value-theorem.md) for the exponential gives

$$
|e^{tx}-1|\leq |t|x e^{|t|},\qquad0<x<1.
$$

Consequently

$$
|u(x,t)|\leq\frac{|t|e^{|t|}}{\sqrt{1-x}},\qquad
\int_0^1\frac{|t|e^{|t|}}{\sqrt{1-x}}\,dx=2|t|e^{|t|}<\infty.
$$

The function is continuous on $(0,1)$ and hence measurable, so **$u(\cdot,t)$ is [Lebesgue integrable](../../../../../lebesgue-integrable-function.md) for every real $t$**. In particular, the numerator cancels the apparent $1/x$ singularity at zero: $u(x,t)\to t$ as $x\downarrow0$. Only the integrable square-root singularity at one remains. At $t=0$ the function is identically zero.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
