<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

The constant term belongs on the forcing side: the equation is $y''-2y'=x+1$. Set $v=y'$ to obtain the first-order linear equation $v'-2v=x+1$. A particular solution is $v_p=-x/2-3/4$, while $v_h=Ae^{2x}$. Imposing $v(0)=0$ fixes $A=3/4$. Integrating and then using $y(0)=0$ gives

$$
\boxed{y(x)=\frac38(e^{2x}-1)-\frac{x^2}{4}-\frac{3x}{4}.}
$$

Direct [differentiation](../../../differentiation.md) gives $y'=3e^{2x}/4-x/2-3/4$ and $y''=3e^{2x}/2-1/2$, so $y''-2y'-1=x$. Both initial values vanish. The nonzero exponential term is required by the initial derivative, even though the forcing is polynomial.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2013 resit](../../2013-resit-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
