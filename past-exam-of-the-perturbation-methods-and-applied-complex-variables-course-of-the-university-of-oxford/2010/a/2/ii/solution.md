<h1 id="a/2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $g_x(t)=(1+xt)^{-1}$. Repeated [integration by parts](../../../../../integration-by-parts.md) using the factor $e^{-t}$ gives

$$
I(x)=\sum_{n=0}^Ng_x^{(n)}(0)+\int_0^\infty e^{-t}g_x^{(N+1)}(t)dt.
$$

Boundary terms at infinity vanish, and $g_x^{(n)}(t)=(-1)^nn!x^n(1+xt)^{-n-1}$. Therefore

$$
I(x)=\sum_{n=0}^N(-1)^nn!x^n+R_N(x),\qquad
|R_N(x)|\leq(N+1)!x^{N+1}\quad(x>0).
$$

For every fixed $N$, this is $o(x^N)$ as $x\downarrow0$, proving

$$
\boxed{I(x)\sim\sum_{n\geq0}(-1)^nn!x^n.}
$$

For each fixed $x>0$ the displayed infinite series diverges, since successive term magnitudes have ratio $(n+1)x\to\infty$. Its usefulness is precisely that of an [asymptotic expansion](../../../../../asymptotic-expansion-split.md), not a convergent power series.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
