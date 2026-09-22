<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $n\ne1$ and a nonzero solution, set $v=y^{1-n}$. Since $v'=(1-n)y^{-n}y'$, multiplying the [Bernoulli differential equation](../../../../bernoulli-differential-equation.md) by $(1-n)y^{-n}$ gives the [linear ordinary differential equation](../../../../linear-ordinary-differential-equation-split.md)

$$
\boxed{v'+(1-n)p(x)v=(1-n)q(x).}
$$

An [integrating factor](../../../../integrating-factor.md) $\mu=\exp((1-n)\int p(x)\,dx)$ gives $v=\mu^{-1}(C+(1-n)\int\mu q\,dx)$. Recover $y$ from $y^{1-n}=v$ on an appropriate real or complex branch. This substitution can omit the zero solution, which must be checked in the original equation. For $n=1$, no substitution is needed: $y'+(p-q)y=0$ is already a [linear ordinary differential equation](../../../../linear-ordinary-differential-equation-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
