<h1 id="a/1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The endpoint branch has $t=(1+is)^{1/3}$ and $dt=(i/3)(1+is)^{-2/3}ds$. Its reversed orientation in the deformed contour gives

$$
I_1(x)=-\frac{ie^{ix}}3\int_0^\infty e^{-xs}(1+is)^{-2/3}\,ds.
$$

At $s=0$,

$$
(1+is)^{-2/3}=1-\frac{2i}{3}s+O(s^2).
$$

[Watson's lemma](../../../../../watson-s-lemma.md), or elementary [Laplace's method](../../../../../laplace-s-method.md) with a Taylor remainder, now yields

$$
I_1(x)=-\frac{ie^{ix}}{3x}-\frac{2e^{ix}}{9x^2}+O(x^{-3}).
$$

Adding the exact cubic-saddle contribution gives the two leading terms

$$
\boxed{I(x)=e^{i\pi/6}\Gamma(4/3)x^{-1/3}-\frac{ie^{ix}}{3x}+O(x^{-2}).}
$$

If the next term is retained, it is $-2e^{ix}/(9x^2)$. The different powers reflect a degenerate saddle at zero and an ordinary endpoint at one.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
