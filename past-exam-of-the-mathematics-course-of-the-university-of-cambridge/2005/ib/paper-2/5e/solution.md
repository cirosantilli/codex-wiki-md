<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

Use the causal [Green function](../../../../../green-s-function.md): it vanishes before the forcing time $t'$. For $t>t'$ it solves the homogeneous equation, is [continuous](../../../../../continuous-function.md) at $t=t'$ with value zero, and has first-derivative jump one. These conditions give

$$
\boxed{G(t,t')=\begin{cases}\sinh(k(t-t'))/k,&t\geq t',\\0,&t<t'.\end{cases}}
$$

Indeed the right [derivative](../../../../../derivative.md) at the forcing time is one and the left [derivative](../../../../../derivative.md) is zero, so $(\partial_t^2-k^2)G=\delta(t-t')$ distributionally. If $k=0$, use the [continuous](../../../../../continuous-function.md) limit $G(t,t')=(t-t')$ on its causal support.

For $k\ne0$, differentiating the [integral](../../../../../integral.md) solution gives

$$
\dot x(t)=\int_0^t\cosh(k(t-t'))f(t')\,dt',\qquad
\ddot x(t)=f(t)+k^2\int_0^t\frac{\sinh(k(t-t'))}{k}f(t')\,dt'.
$$

Both initial values vanish and $\ddot x-k^2x=f$. This verifies the requested representation and its sign. The $k=0$ formula similarly gives $\ddot x=f$.

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
