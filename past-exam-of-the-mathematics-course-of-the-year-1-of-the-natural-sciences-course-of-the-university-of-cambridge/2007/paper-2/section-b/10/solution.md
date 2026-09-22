<h1 id="section-b/10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

Substitute $u(y,t)=Y(y)T(t)$ into the [diffusion equation](../../../../../diffusion-equation-split.md) and divide on a region where both factors are nonzero. This gives $Y''/Y=T'/(\nu T)$. The two sides depend on different variables, so they equal a separation [constant](../../../../../constant-mathematics.md) $a$:

$$
\boxed{Y''=aY,\qquad T'=\nu aT.}
$$

These identities then extend through the zeros of the separated factors. The zero [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) require $Y(0)=Y(1)=0$. For a nontrivial solution, $a$ must be negative: $a=0$ gives only a vanishing linear function and $a>0$ gives only a vanishing hyperbolic-sine solution. Writing $a=-k^2$ gives $Y=A\sin(ky)$, and $k=n\pi$, $n=1,2,\ldots$. Consequently the separated modes of [free viscous decay between parallel plates](../../../../../free-viscous-decay-between-parallel-plates.md) are $\sin(n\pi y)e^{-\nu n^2\pi^2t}$.

The first initial condition selects the lowest mode:

$$
\boxed{u(y,t)=\sin(\pi y)e^{-\nu\pi^2t}.}
$$

The [superposition principle](../../../../../superposition-principle.md) for a homogeneous [linear differential equation](../../../../../linear-differential-equation.md) states that any linear combination of solutions is again a solution, with the same combination of homogeneous [boundary conditions](../../../../../boundary-condition.md) and initial data. It therefore gives

$$
\boxed{u(y,t)=\sin(\pi y)e^{-\nu\pi^2t}+\frac1{10}\sin(3\pi y)e^{-9\nu\pi^2t}.}
$$

The higher spatial mode decays nine times as fast, so the [velocity](../../../../../velocity.md) profile approaches a multiple of the first sine mode before vanishing altogether.

## ↑ Ancestors (13)

1. [10](../10.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
