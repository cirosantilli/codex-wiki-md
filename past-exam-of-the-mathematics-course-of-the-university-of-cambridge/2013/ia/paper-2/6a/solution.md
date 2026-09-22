<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

Expand the function into separated terms: $f=g(x)+h(y)$, where $g=x^2-x^4$ and $h=y^8-y^4$. Then

$$
f_x=2x(1-2x^2),\qquad f_y=4y^3(2y^4-1).
$$

Put $a=2^{-1/2}$ and $b=2^{-1/4}$. The nine [critical points](../../../../../critical-point.md) are all pairs from $x\in\{0,\pm a\}$ and $y\in\{0,\pm b\}$. The diagonal [Hessian matrix](../../../../../hessian-matrix.md) has entries $2-12x^2$ and $56y^6-12y^2$.

At $(0,\pm b)$ both entries are positive, giving strict [local minima](../../../../../local-minimum.md) of value $-1/4$. At $(\pm a,\pm b)$ they have opposite signs, giving four [saddle points](../../../../../saddle-point.md) of value zero. At the three points on $y=0$ the Hessian is degenerate, so its sign alone does not classify them. Use the [higher-order test for separated extrema](../../../../../higher-order-test-for-separated-extrema.md): $h(y)=-y^4+O(y^8)$ is negative for small nonzero $y$. At $(0,0)$ the positive $x^2$ term and negative $y^4$ term give a saddle. At $(\pm a,0)$, $g-1/4=-(x^2-1/2)^2$, so every sufficiently small nonzero displacement decreases $f$ and these are strict [local maxima](../../../../../local-maximum.md).

**There are two maxima at $(\pm a,0)$, two minima at $(0,\pm b)$, and five [saddle points](../../../../../saddle-point.md): $(0,0)$ and $(\pm a,\pm b)$.**

For the [level curves](../../../../../level-curve.md), the exact zero set consists of the two parabolas $x=\pm y^2$ and the oval $x^2+y^4=1$. They cross at the four nondegenerate [saddle points](../../../../../saddle-point.md). Small positive levels enclose each maximum; small negative levels enclose each minimum. The degenerate central saddle has quartic narrowing, locally $x^2-y^4=c$. Far along the $x$ axis the function is negative, while far along the $y$ axis it is positive. These signs and zero curves determine the connectivity shown in the sketch.

<a id="6a/image-level-curves-exact-zero-set-and-all-nine-classified-critical-points-of-the-separated-quartic-octic-function"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-2-critical-contours.png)

**[Figure 1](#6a/image-level-curves-exact-zero-set-and-all-nine-classified-critical-points-of-the-separated-quartic-octic-function). Level curves, exact zero set and all nine classified critical points of the separated quartic-octic function**.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
