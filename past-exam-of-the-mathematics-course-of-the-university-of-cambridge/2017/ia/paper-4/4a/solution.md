<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

The dimensions are $[m]=\mathsf M$, $[\alpha]=\mathsf M\mathsf T^{-1}$, $[u_0]=\mathsf L\mathsf T^{-1}$, and $[g]=\mathsf L\mathsf T^{-2}$. Under the stated model, $m,\alpha,u_0,g$ are the only parameters determining the ascent [time](../../../../../time-in-physics.md). If $m^p\alpha^q u_0^r g^s$ is dimensionless, then $p+q=0$, $r+s=0$, and $-q-r-2s=0$, leaving one independent [dimensionless variable](../../../../../dimensionless-variable.md). One convenient choice is

$$
\boxed{\lambda=\frac{\alpha u_0}{mg},\qquad T=\frac m\alpha f(\lambda).}
$$

Thus [dimensional analysis](../../../../../dimensional-analysis.md) fixes the form, but [Newton's second law](../../../../../newton-s-second-law.md) must determine the [function](../../../../../function-split.md) $f$.

Take upward [velocity](../../../../../velocity.md) as positive. Throughout ascent, [Newton's second law](../../../../../newton-s-second-law.md) with [linear drag](../../../../../linear-drag.md) gives $m\dot v=-mg-\alpha v$. An [integrating factor](../../../../../integrating-factor.md) or direct solution of this [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md) gives

$$
v(t)=\left(u_0+\frac{mg}{\alpha}\right)e^{-\alpha t/m}-\frac{mg}{\alpha}.
$$

The first zero of this [velocity](../../../../../velocity.md) is the highest point, so

$$
\boxed{f(\lambda)=\log(1+\lambda),\qquad T=\frac m\alpha\log\left(1+\frac{\alpha u_0}{mg}\right).}
$$

This [vertical ascent under linear drag](../../../../../vertical-ascent-under-linear-drag.md) has $T<u_0/g$ for $u_0>0$, since $\log(1+\lambda)<\lambda$. The limit $\alpha\to0$ recovers the no-drag ascent [time](../../../../../time-in-physics.md) $u_0/g$; $u_0=0$ gives $T=0$.

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
