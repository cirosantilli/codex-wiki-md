<h1 id="5e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A particle [pathline](../../../../../../pathline.md) follows the time-dependent [velocity field](../../../../../../velocity-field.md), so its coordinates satisfy $\dot x-x=\sin t$ and $\dot y=-y$. The second equation and the initial data give $y=e^{-t}$. Using the [integrating factor](../../../../../../integrating-factor.md) $e^{-t}$ in the first,

$$
e^{-t}x(t)=x_0+\int_0^t e^{-s}\sin s\,ds
=x_0+\frac12-\frac12e^{-t}(\sin t+\cos t).
$$

Therefore the complete [pathline](../../../../../../pathline.md) is

$$
\boxed{(x(t),y(t))
=\left((x_0+\tfrac12)e^t-\tfrac12(\sin t+\cos t),e^{-t}\right),\quad t\ge0}.
$$

If $x_0+\tfrac12\ne0$, its first coordinate grows without bound in magnitude. If $x_0=-\tfrac12$, the first coordinate remains bounded and periodic while $y\to0$. **The unique release coordinate giving a bounded particle path is $x_0=-1/2$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5E](../../5e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
