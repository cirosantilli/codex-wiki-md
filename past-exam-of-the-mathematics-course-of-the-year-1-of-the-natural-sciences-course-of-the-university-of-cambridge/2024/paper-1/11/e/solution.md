<h1 id="11/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Since $x=\cos y$ with real $y$, necessarily $-1\leq x\leq1$. Use [Euler's formula](../../../../../euler-s-formula.md) and set $w=e^{iy}\ne0$. Then

$$
2x=w+w^{-1},\qquad w^2-2xw+1=0,
$$

so the [quadratic equation](../../../../../quadratic-equation.md) gives $w=x\pm i\sqrt{1-x^2}$. Let $q=x+i\sqrt{1-x^2}$. It lies on the upper half of the [unit circle](../../../../../complex-unit-circle.md), so $q=e^{i\theta}$ with $0\leq\theta\leq\pi$. Choose the [complex logarithm](../../../../../complex-logarithm.md) value $\ln q=i\theta$, taking $\ln(-1)=i\pi$ at $x=-1$. The two roots are $e^{\pm i\theta}$, so $e^{iy}=e^{\pm i\theta}$ gives $y=\pm\theta+2n\pi$.

Because $i\ln q=-\theta$, this set of real solutions is exactly

$$
\boxed{y=\pm i\ln\left(x+i\sqrt{1-x^2}\right)+2n\pi,\qquad n\in\mathbb Z.}
$$

The formula includes $x=\pm1$: the two sign families then coincide after adjusting $n$. No real $y$ exists if $|x|>1$.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [11](../../11.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
