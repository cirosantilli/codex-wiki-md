<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The source factor cancels the singular denominator of the [Green function](../../../../../green-s-function-split.md). Splitting the [integral](../../../../../integral-split.md) at $\xi=x$ gives

$$
y(x)=v(x)\int_{-1}^x(1+\xi)e^{-\xi}d\xi+(1+x)\int_x^1\left[1-\frac e2(1+\xi)e^{-\xi}\right]d\xi.
$$

Using $\int(1+\xi)e^{-\xi}d\xi=-(\xi+2)e^{-\xi}$, these two integrals are $e-(x+2)e^{-x}$ and $5/2-x-e(x+2)e^{-x}/2$, respectively. Simplification gives

$$
\boxed{y(x)=e^{x+1}+\frac{1-e^2}{2}(1+x)-x^2.}
$$

The exponential and linear terms are homogeneous solutions, while direct [differentiation](../../../../../differentiation.md) gives $L(-x^2)=x$ for $x\ne0$. Also $y(-1)=y(1)=0$, and the expression is analytic through zero. Uniqueness in this regular class follows because any difference is a global [linear combination](../../../../../linear-combination.md) $Ae^x+B(1+x)$: the left boundary forces $A=0$, and the right then forces $B=0$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
