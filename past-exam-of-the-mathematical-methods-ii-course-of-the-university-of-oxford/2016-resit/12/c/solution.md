<h1 id="12/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At a [stationary point](../../../../stationary-point.md), the linear terms vanish, so $\Delta f\simeq\tfrac12(Ah^2+2Bhk+Ck^2)$, with $A=f_{xx}$, $B=f_{xy}$, $C=f_{yy}$. Let $D=AC-B^2$ be the [Hessian determinant](../../../../hessian-determinant.md). For $A\ne0$, completing the square gives

$$
2\Delta f\simeq A\left(h+\frac BA k\right)^2+\frac DA k^2.
$$

The [second-derivative test](../../../../second-derivative-test.md) therefore yields

$$
\boxed{D>0,\ A>0:\text{ strict local minimum};\quad
D>0,\ A<0:\text{ strict local maximum};\quad
D<0:\text{ saddle point}.}
$$

When $D<0$ the quadratic form is indefinite, including the case $A=0$, $B\ne0$. When $D=0$, the quadratic approximation is degenerate and the test is inconclusive: higher-order terms may produce a minimum, maximum or saddle. For nondegenerate cases the quadratic term dominates the Taylor remainder sufficiently close to the point.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [12](../../12.md)
3. [2016 resit](../../../2016-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
