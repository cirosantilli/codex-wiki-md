<h1 id="38c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Substitute the exact smooth solution into the [leapfrog advection scheme](../../../../../../leapfrog-advection-scheme.md) and expand the centered differences. With $\tau=\Delta t$ and $h=\Delta x$, the normalized [local truncation error](../../../../../../local-truncation-error.md) is

$$
\frac{u(x,t+\tau)-u(x,t-\tau)}{2\tau}-\frac{u(x+h,t)-u(x-h,t)}{2h}=\frac{\tau^2}{6}u_{ttt}-\frac{h^2}{6}u_{xxx}+O(\tau^4+h^4).
$$

Because $u_t=u_x$, repeated differentiation gives $u_{ttt}=u_{xxx}$. Hence

$$
\boxed{\mathcal T=\frac{\tau^2-h^2}{6}u_{xxx}+O(\tau^4+h^4).}
$$

Equivalently the unnormalized one-update residual is $\tau(\tau^2-h^2)u_{xxx}/3+O(\tau^5+\tau h^4)$. Thus the scheme is second order in space and time. When $\tau=h$, the exact translating solution $u(x,t)=F(x+t)$ satisfies the grid recurrence exactly; initialization still matters for the independent computational branch.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38C](../../38c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
