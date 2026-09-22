<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A vector [line integral](../../../line-integral.md) along an oriented parametrized curve $r(t)$ is $\int a(r(t))\cdot r'(t)\,dt$; for a force field it is the work along that path. On the upper branch, set $y=t$, $x=t^2$, $0\le t\le1$. Then

$$
a\cdot dr=(t^2-t)(2t\,dt)+(t^2+t)dt
=(2t^3-t^2+t)dt,
$$

so

$$
\boxed{\int_Ca\cdot dr=\left[\frac{t^4}{2}-\frac{t^3}{3}+\frac{t^2}{2}\right]_0^1=\frac23.}
$$

The stated $x$ endpoints do not distinguish the two branches of $y^2=x$. If the lower branch is intended, the same parametrization runs from $t=0$ to $t=-1$, giving instead $\boxed{4/3}$. The two values correspond to different terminal points, $(1,1)$ and $(1,-1)$; choosing a branch is necessary to make the question unambiguous.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2017 resit](../../2017-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
