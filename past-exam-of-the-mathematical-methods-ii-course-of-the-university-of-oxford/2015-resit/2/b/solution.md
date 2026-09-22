<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Combine the two singular terms before taking the [limit](../../../../limit-of-a-function.md):

$$
\frac{\log(1+x)}{x^2}-\frac1x=\frac{\log(1+x)-x}{x^2}.
$$

For $x$ near zero, within the real domain $x>-1$, the [Maclaurin series](../../../../maclaurin-series.md) is $\log(1+x)=x-x^2/2+O(x^3)$. Hence

$$
\frac{\log(1+x)-x}{x^2}=-\frac12+O(x),\qquad\boxed{\lim_{x\to0}\left(\frac{\log(1+x)}{x^2}-\frac1x\right)=-\frac12}.
$$

The two individual terms have divergent limits; their leading singularities cancel. Evaluating them separately as an “infinity minus infinity” subtraction would not justify the finite result.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
