<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The successive [derivatives](../../../derivative.md) are $f^{(n)}(x)=(-6)^ne^{-6x}$, so $f^{(n)}(-4)=(-6)^ne^{24}$. Substitution in the [Taylor series](../../../taylor-series.md) formula about $a=-4$ gives

$$
\boxed{e^{-6x}=e^{24}\sum_{n=0}^{\infty}\frac{(-6)^n(x+4)^n}{n!}
=e^{24}\left[1-6(x+4)+18(x+4)^2-36(x+4)^3+\cdots\right].}
$$

The [ratio test](../../../ratio-test.md) shows convergence for every finite real or complex $x$: the absolute ratio of successive terms is $6|x+4|/(n+1)\to0$. This is also the usual [exponential function](../../../exponential-function.md) series applied to $e^{24}e^{-6(x+4)}$, proving that the series equals the stated function everywhere.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2019](../../2019-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
