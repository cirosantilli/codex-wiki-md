<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Substitute the path into the height before differentiating: $x^2=1+t$, $y=t-1$, so

$$
h(t)=\frac1{t+2+2(t-1)^4}.
$$

The ordinary [chain rule](../../../chain-rule.md) immediately yields

$$
\boxed{\frac{dh}{dt}=-\frac{1+8(t-1)^3}{[t+2+2(t-1)^4]^2}.}
$$

The multivariable calculation gives the same result: $h_x=-2x/(x^2+2y^4+1)^2$, $h_y=-8y^3/(x^2+2y^4+1)^2$, and $\dot h=h_x\dot x+h_y\dot y$ with $\dot x=1/(2\sqrt{1+t})$ and $\dot y=1$. The real path has $t\geq-1$; this chain-rule calculation applies for $t>-1$, and the simplified height has a finite right derivative at the endpoint even though $\dot x$ there is singular.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2013 resit](../../2013-resit-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
