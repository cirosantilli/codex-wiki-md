<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For positive $a,b$ and upward orientation, traverse the four edges counterclockwise. The bottom edge contributes $\int_0^a x^2dx=a^3/3$. The right edge contributes $\int_0^b2ay\,dy=ab^2$. On the top edge $x$ decreases, giving $\int_a^0(x^2-b^2)dx=-a^3/3+ab^2$. The left edge has $x=0$ and zero tangential component. Hence

$$
\boxed{\oint_{\partial S}\mathbf A\cdot d\mathbf r=\frac{a^3}{3}+ab^2-\frac{a^3}{3}+ab^2=2ab^2.}
$$

This agrees with the [surface integral](../../../../surface-integral.md) and explicitly verifies [Stokes theorem](../../../../stokes-theorem.md), including the direction of the top-edge traversal.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2014 resit](../../../2014-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
