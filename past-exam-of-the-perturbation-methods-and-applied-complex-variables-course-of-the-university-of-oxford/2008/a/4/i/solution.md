<h1 id="a/4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Treat $t,T$ as independent variables, with $T=\epsilon^2t$. The [chain rule](../../../../../chain-rule.md) gives

$$
\frac d{dt}=\partial_t+\epsilon^2\partial_T,\qquad
\frac{d^2}{dt^2}=\partial_t^2+
2\epsilon^2\partial_t\partial_T+\epsilon^4\partial_T^2.
$$

Therefore the [method of multiple scales](../../../../../method-of-multiple-scales.md) is

$$
\boxed{y_{tt}+y+\epsilon\cos t\,y+
\epsilon^2(2y_{tT}+a_2y)+\epsilon^4y_{TT}
+O(\epsilon^4)y=0.}
$$

The unspecified $O(\epsilon^4)$ term includes the higher correction in $a$. Only the displayed terms through order $\epsilon^2$ are needed to determine the leading slow-amplitude system.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
