<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $h=x+3$, so $x=-3(1-h/3)$. The [negative binomial series](../../../../negative-binomial-series.md) gives $(1-u)^{-4}=\sum_{n=0}^\infty\binom{n+3}{3}u^n$ for $|u|<1$. Hence the exact [Taylor series](../../../../taylor-series.md) is

$$
\boxed{\frac7{x^4}=\frac7{81}\sum_{n=0}^\infty\binom{n+3}{3}\left(\frac{x+3}{3}\right)^n,\qquad|x+3|<3.}
$$

The initial terms are $\frac7{81}[1+4h/3+10h^2/9+20h^3/27+\cdots]$. Equivalently the coefficient of $(x+3)^n$ is $7(n+3)!/[6n!3^{n+4}]$, obtained by differentiating $7x^{-4}$ repeatedly and evaluating at $-3$.

The radius of convergence is three, set by the pole at $x=0$. At either endpoint $h=\pm3$, the terms fail to tend to zero, so neither endpoint is included.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2019 resit](../../../2019-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
