<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

Differentiate the [Friedmann equation](../../../../../friedmann-equations.md)

$$
H^2=\frac{8\pi G}{3c^2}\rho-\frac{kc^2}{R^2a^2}
$$

and use the [cosmological perfect-fluid continuity equation](../../../../../cosmological-perfect-fluid-continuity-equation.md)

$$
\dot\rho=-3H(\rho+P).
$$

After dividing by $2H$,

$$
\dot H=-\frac{4\pi G}{c^2}(\rho+P)
+\frac{kc^2}{R^2a^2}.
$$

Since $\ddot a/a=\dot H+H^2$, eliminating the curvature term gives the [Friedmann acceleration equation](../../../../../friedmann-acceleration-equation.md)

$$
\boxed{
\frac{\ddot a}{a}
=-\frac{4\pi G}{3c^2}(\rho+3P)
}.
$$

Under the [strong energy condition in a Friedmann universe](../../../../../strong-energy-condition-in-a-friedmann-universe.md), $\rho+3P\geq0$, so $\ddot a/a\leq0$. Therefore

$$
\dot H=\frac{\ddot a}{a}-H^2\leq-H^2,
$$

and wherever $H\ne0$,

$$
\boxed{
\frac d{dt}H^{-1}
=-\frac{\dot H}{H^2}\geq1
}.
$$

If $H(t_0)>0$, integrating the inequality backward shows that $H^{-1}$ reaches zero no later than $t_0-H(t_0)^{-1}$. Thus $H\to+\infty$ and $a\to0$ at a finite time in the past. If $H(t_0)<0$, the same argument forward in time makes $H\to-\infty$ and $a\to0$ at a finite future time. The sign of $H$ distinguishes an expanding universe with a past Big Bang from a contracting universe ending in a [Big Crunch](../../../../../big-crunch.md). Hence a Friedmann universe obeying the strong energy condition cannot remain nonsingular for unlimited proper time in both directions.

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
