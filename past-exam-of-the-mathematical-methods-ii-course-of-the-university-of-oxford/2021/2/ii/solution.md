<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a fixed $x\in[0,1]$, the allowed $y$ interval is $[0,\sqrt x]$. Integrating the [joint probability density](../../../../joint-probability-density.md) over it gives the [marginal density](../../../../marginal-density.md)

$$
\boxed{f_X(x)=\begin{cases}\displaystyle\int_0^{\sqrt x}6xy\,dy=3x^2,&0\le x\le1,\\0,&\text{otherwise}.\end{cases}}
$$

For a fixed $y\in[0,1]$, the inequality $y\le\sqrt x$ is equivalent to $x\ge y^2$. The other [marginal density](../../../../marginal-density.md) is therefore

$$
\boxed{f_Y(y)=\begin{cases}\displaystyle\int_{y^2}^1 6xy\,dx=3y(1-y^4),&0\le y\le1,\\0,&\text{otherwise}.\end{cases}}
$$

As a normalization check, $\int_0^1 3x^2\,dx=1$ and $\int_0^1 3y(1-y^4)\,dy=1$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
