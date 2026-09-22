<h1 id="12/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The forcing $\sec(2x)$ is undefined at $x=\pm\pi/4$, both inside the printed interval. Therefore **there is no classical solution on the whole stated interval**. Solve separately on the three connected components obtained by removing those two points.

Choose $u_1=\cos(2x)$ and $u_2=\sin(2x)$, whose [Wronskian](../../../../wronskian.md) is two. [Variation of parameters](../../../../variation-of-parameters.md) gives $t_1'=-(1/2)\tan(2x)$ and $t_2'=1/2$, so a particular solution is $\tfrac14\cos(2x)\log|\cos(2x)|+\tfrac x2\sin(2x)$. The full answer on each regular component is

$$
\boxed{y=A\cos(2x)+B\sin(2x)+\frac14\cos(2x)\log|\cos(2x)|+\frac x2\sin(2x).}
$$

The constants $A,B$ can differ between $(-\pi/2,-\pi/4)$, $(-\pi/4,\pi/4)$ and $(\pi/4,\pi/2)$. [Differentiation](../../../../differentiation.md) gives $y''+4y=1/\cos(2x)$ wherever the forcing is defined. Although the particular solution has finite one-sided values at the singularities, its [derivative](../../../../derivative.md) has a logarithmic divergence, and the equation itself is undefined there. It cannot be promoted to one classical solution across the poles.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [12](../../12.md)
3. [2019 resit](../../../2019-resit-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
