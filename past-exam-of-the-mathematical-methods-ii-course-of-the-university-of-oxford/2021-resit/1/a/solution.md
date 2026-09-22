<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Maclaurin series](../../../../maclaurin-series.md) of the [exponential function](../../../../exponential-function.md) and [sine](../../../../sine.md) give

$$
e^{x^2}=1+x^2+\frac{x^4}{2}+\frac{x^6}{6}+O(x^8),\qquad
x\sin x=x^2-\frac{x^4}{6}+\frac{x^6}{120}+O(x^8).
$$

Both the numerator and denominator first become nonzero at order $x^4$. Dividing by that common power gives the [limit](../../../../limit-of-a-function.md)

$$
\boxed{\lim_{x\to0}\frac{1+x^2-e^{x^2}}{x\sin x-x^2}
=\lim_{x\to0}\frac{-1/2+O(x^2)}{-1/6+O(x^2)}=3.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
