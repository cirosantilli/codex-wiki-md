<h1 id="39a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $\tau=\Delta t$ and $h=\Delta x$, with $h^2=\tau/\mu$ for fixed $\mu>0$. Substitute a smooth exact solution of the [heat equation](../../../../../../heat-equation.md) into the [Adams-Bashforth method](../../../../../../adams-bashforth-method.md). Define its one-step defect $R$ as the left side minus the right side of the unscaled update. The centered [finite difference](../../../../../../finite-difference-split.md) satisfies

$$
D_hu=\frac{u(x-h,t)-2u(x,t)+u(x+h,t)}{h^2}=u_{xx}+\frac{h^2}{12}u_{xxxx}+O(h^4).
$$

The [Taylor expansion](../../../../../../taylor-expansion.md) in time gives

$$
u(t+\tau)-u(t)=\tau u_t+\frac{\tau^2}{2}u_{tt}+O(\tau^3),
$$



$$
\tau\left[\tfrac32D_hu(t)-\tfrac12D_hu(t-\tau)\right]=\tau u_{xx}+\frac{\tau^2}{2}u_{xxt}+\frac{\tau h^2}{12}u_{xxxx}+O(\tau^3+\tau^2h^2+\tau h^4).
$$

Since $u_t=u_{xx}$ and $u_{tt}=u_{xxt}$, the first two terms cancel, leaving

$$
\boxed{R=-\frac{\tau^2}{12\mu}u_{xxxx}+O(\tau^3)=O(\tau^2).}
$$

This is the requested local error of the unscaled update. If “local truncation error” denotes the defect divided by $\Delta t$, it is instead $O(\Delta t)$ under fixed $\mu$: the centered spatial error is then $O(h^2)=O(\Delta t)$. The scheme is second order in time at fixed spatial discretization, which is a separate order statement.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [39A](../../39a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
