<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At elimination column $k$, let $r=m-k$ be the size of the remaining trailing block. Computing its multipliers costs $r$ divisions; updating all $r^2$ entries costs $2r^2$ [floating-point operations](../../../../../floating-point-operation.md), one multiplication and one subtraction per entry. Thus the dominant count is

$$
\sum_{r=1}^{m-1}(2r^2+r)=\frac{m(m-1)(2m-1)}3+\frac{m(m-1)}2
=\boxed{\frac23m^3+O(m^2)}.
$$

Updating the right side and [back substitution](../../../../../back-substitution.md) add only $O(m^2)$ [floating-point operations](../../../../../floating-point-operation.md). Pivot searches involve comparisons and row exchanges, without changing the leading arithmetic count. Hence [Gaussian elimination](../../../../../gaussian-elimination.md) with pivoting has the requested asymptotic cost.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
