<h1 id="a/1/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

The [function](../../../../../function-split.md) $e^{-x^2}/x$ is strictly decreasing from infinity to zero on $x>0$, so there is a unique positive root, which tends to infinity. Let $L=\log(1/\epsilon)$. Taking [logarithms](../../../../../logarithm.md) gives

$$
x^2+\log x=L.
$$

First $x^2\sim L$. Put $x=\sqrt L+d$ with $d=o(\sqrt L)$, expand, and cancel $L$:

$$
2\sqrt L\,d+d^2+\tfrac12\log L
+\log(1+d/\sqrt L)=0.
$$

The leading balance gives $d=-(\log L)/(4\sqrt L)$. Substitution leaves a residual $O((\log L)^2/L)$; the [derivative](../../../../../derivative.md) of $x^2+\log x$ is of order $\sqrt L$, so the root error is $O((\log L)^2/L^{3/2})$. Thus

$$
\boxed{x=\sqrt L-\frac{\log L}{4\sqrt L}
+O\!\left(\frac{(\log L)^2}{L^{3/2}}\right).}
$$

The second term is logarithmic rather than a constant multiple of $L^{-1/2}$. This is [logarithmic inversion of a Gaussian divided by its argument](../../../../../logarithmic-inversion-of-a-gaussian-divided-by-its-argument.md).

## ↑ Ancestors (13)

1. [Vi](../vi.md)
2. [1](../../1.md)
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
