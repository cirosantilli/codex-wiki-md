<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $h=x-\pi/2$. The trigonometric identity $\sin(\pi/2+h)=\cos h$ changes the expression to $h^2/(\cos h-1)$. Since $\cos h-1=-h^2/2+O(h^4)$,

$$
\boxed{\lim_{x\to\pi/2}\frac{(x-\pi/2)^2}{\sin x-1}=-2}.
$$

The negative sign is also forced geometrically: near its maximum, $\sin x-1$ is negative while the numerator is nonnegative. Both numerator and denominator vanish quadratically, so one application of a first-derivative argument alone would not yet resolve the indeterminate form.

## ↑ Ancestors (12)

1. [C](../c.md)
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
