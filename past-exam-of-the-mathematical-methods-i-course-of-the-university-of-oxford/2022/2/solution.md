<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

On an interval with $x\ne0$, the zero function is one solution. For a nonzero solution, set $u=y^{-2}$. Dividing the equation by two and differentiating $u$ gives the [linear ordinary differential equation](../../../linear-ordinary-differential-equation-split.md)

$$
u'-\frac2xu=-\frac1{x^3}.
$$

Its [integrating factor](../../../integrating-factor.md) is $x^{-2}$, so $(u/x^2)'=-x^{-5}$ and $u=1/(4x^2)+Cx^2$. Absorbing the factor four into the integration constant gives

$$
\boxed{y(x)=\frac{\pm2x}{\sqrt{1+Kx^4}},\quad\text{or}\quad y(x)=0.}
$$

For real solutions, choose a connected interval avoiding $x=0$ on which $1+Kx^4>0$, with a fixed sign. The special straight solutions $y=\pm2x$ are already included at $K=0$. The separate zero solution would be lost by the division used in the substitution.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2022](../../2022-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
