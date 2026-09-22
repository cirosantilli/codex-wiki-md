<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Normalize the specified direction to $\hat{\mathbf u}=(1,1)/\sqrt2$. At distance $s\geq0$ the squared radius is $(1+s/\sqrt2)^2+(2+s/\sqrt2)^2=5+3\sqrt2s+s^2$. The exact change $\Delta T=0.12$ therefore requires $5+3\sqrt2s+s^2=5e^{0.12}$. The positive root is

$$
\boxed{s=\frac{\sqrt{20e^{0.12}-2}-3\sqrt2}{2}.}
$$

For comparison, the initial [directional derivative](../../../../directional-derivative.md) is $(2/5,4/5)\cdot(1,1)/\sqrt2=3\sqrt2/5$. Its first-order distance estimate is

$$
\boxed{s\simeq\frac{0.12}{3\sqrt2/5}=\frac{\sqrt2}{10}.}
$$

These give approximately $0.145$ and $0.141$. The exact expression accounts for the changing gradient along a finite straight displacement.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
