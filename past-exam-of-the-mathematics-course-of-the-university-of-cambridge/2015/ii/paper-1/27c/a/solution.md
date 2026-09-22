<h1 id="27c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\operatorname{Re}z>0$, the [gamma function](../../../../../../gamma-function.md) is

$$
\Gamma(z)=\int_0^\infty t^{z-1}e^{-t}dt.
$$

Rotate the integration ray through $\pi/2$, or insert a damping factor and then let it vanish. With the principal power, [contour rotation](../../../../../../contour-rotation.md) gives

$$
\boxed{\int_0^\infty t^{\gamma-1}e^{it}dt=e^{i\pi\gamma/2}\Gamma(\gamma),\qquad0<\gamma<1}.
$$

For the damping argument, $\int t^{\gamma-1}e^{-(\epsilon-i)t}dt=\Gamma(\gamma)(\epsilon-i)^{-\gamma}$, and Dirichlet tail estimates justify the limit. The condition $\gamma>0$ ensures integrability at zero; $\gamma<1$ makes the amplitude tend to zero and permits conditional convergence at infinity. At $\gamma=1$, the upper-end oscillation has no limit; larger $\gamma$ also fails ordinary improper convergence. These restrictions concern this improper integral, not its analytic regularizations.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27C](../../27c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
