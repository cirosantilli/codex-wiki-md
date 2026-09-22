<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The trial function $y=x(1-x)$ gives

$$
J[y]=\int_0^1x^3(1-x)^2dx=\frac1{60},\qquad
I[y]=\int_0^1x(1-2x)^2dx+k^2\int_0^1x(1-x)^2dx=\frac16+\frac{k^2}{12}.
$$

Its [Rayleigh quotient](../../../../rayleigh-quotient.md) is $5k^2+10$, yielding the upper bound. Conversely, $1/x\geq x$ on $(0,1)$ and the derivative energy is nonnegative, so $I[y]\geq k^2J[y]$ for every admissible $y$. Part (b) therefore gives

$$
\boxed{k\leq z_{k,1}\leq\sqrt{5k^2+10}}.
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
