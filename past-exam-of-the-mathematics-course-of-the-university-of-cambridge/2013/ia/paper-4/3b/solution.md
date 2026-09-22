<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

Use [zero-relative-velocity mass shedding](../../../../../zero-relative-velocity-mass-shedding.md): the released sand initially shares the balloon's vertical [velocity](../../../../../velocity.md), rather than being actively ejected. Let $q=M+m(t)$ and let a positive mass $\delta m$ be shed in a short interval $dt$. The [momentum](../../../../../momentum.md) of the balloon and that newly released sand changes by

$$
(q-\delta m)(v+dv)+\delta m\,v-qv=q\,dv+O(dt^2).
$$

The leading external impulse is $(T-qg)dt$. [Newton's second law](../../../../../newton-s-second-law.md) applied to this combined material system therefore gives

$$
\boxed{(M+m)\dot v=T-(M+m)g.}
$$

Writing $\frac d{dt}(qv)=T-qg$ for the remaining balloon alone would omit the outgoing [momentum](../../../../../momentum.md) flux. A nonzero relative ejection [velocity](../../../../../velocity.md) would instead produce a [rocket equation](../../../../../rocket-equation.md) thrust term.

Initial mechanical equilibrium gives $T=(M+m_0)g$. Write $\lambda=m_0/t_0$, so $m=m_0-\lambda t$ up to depletion. Then

$$
\dot v=g\frac{\lambda t}{M+m_0-\lambda t}
=g\frac{t}{A-t},\qquad A=\frac{M+m_0}{\lambda}>t_0.
$$

Integrating from rest,

$$
v(t)=g\left[A\log\frac{A}{A-t}-t\right].
$$

Since $A/t_0=1+M/m_0$ and $A/(A-t_0)=1+m_0/M$, the final upward [speed](../../../../../speed.md) is

$$
\boxed{v(t_0)=gt_0\left[\left(1+\frac{M}{m_0}\right)
\log\left(1+\frac{m_0}{M}\right)-1\right].}
$$

The acceleration is nonnegative throughout release, consistent with the upward motion.

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
