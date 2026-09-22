<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In a submultiplicative [matrix norm](../../../../matrix-norm.md), the exponential series is absolutely convergent. Its [Cauchy product](../../../../cauchy-product.md) can therefore be grouped by the total degree:

$$
e^Ae^B=\sum_{n=0}^{\infty}\sum_{j=0}^n\frac{A^jB^{n-j}}{j!(n-j)!}
=\sum_{n=0}^{\infty}\frac1{n!}\sum_{j=0}^n\binom nj A^jB^{n-j}.
$$

When $AB=BA$, the inner sum is $(A+B)^n$ by the [binomial theorem](../../../../binomial-theorem.md). Thus $\boxed{e^Ae^B=e^{A+B}}$. The commutation assumption is used precisely in that binomial expansion; absolute convergence alone does not supply it.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [10](../../10.md)
3. [2016 resit](../../../2016-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
