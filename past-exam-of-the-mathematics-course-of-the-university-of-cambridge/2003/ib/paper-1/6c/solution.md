<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

Follow a fluid particle released at time $s$, and use $\tau$ for its running time. Its [pathline](../../../../../pathline.md) satisfies $dx/d\tau=1$, $dy/d\tau=\tau x$ and $dz/d\tau=0$, with zero position at $\tau=s$. Hence $x(\tau)=\tau-s$, $z(\tau)=0$, and

$$
y(t)=\int_s^t\tau(\tau-s)d\tau=\frac{t^3}{3}-\frac{st^2}{2}+\frac{s^3}{6}.
$$

At observation time $t$, set $x=t-s$. Substitution gives the [streakline](../../../../../streakline.md)

$$
\boxed{(x,y,z)=\left(t-s,\ \frac12t(t-s)^2-\frac16(t-s)^3,\ 0\right),\quad y=\frac12tx^2-\frac16x^3.}
$$

The curve is parameterized by release times $s\leq t$. If release starts at time zero, only $0\leq x\leq t$ is occupied. This is a [streakline](../../../../../streakline.md), the positions of different particles released at one fixed point, rather than an instantaneous [streamline](../../../../../streamline.md) of this unsteady flow.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
