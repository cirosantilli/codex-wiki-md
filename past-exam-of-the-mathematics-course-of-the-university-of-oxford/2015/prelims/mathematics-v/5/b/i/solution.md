<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Substitute the [separated solution](../../../../../../../separated-solution.md) $y=e^{-\alpha t}F(t)\sin(nx)$ into the [damped wave equation](../../../../../../../damped-wave-equation.md). Its [time derivatives](../../../../../../../time-derivative.md) give

$$
y_{tt}+2\alpha y_t=e^{-\alpha t}(F''-\alpha^2F)\sin(nx),
$$

whereas $y_{xx}=-n^2e^{-\alpha t}F\sin(nx)$. Thus

$$
F''+(n^2-\alpha^2)F=0,\qquad F(0)=0,\quad F'(0)=1.
$$

The last two conditions follow from $y(x,0)=0$ and $y_t(x,0)=\sin(nx)$. For $0<\alpha<n$, let $\nu=\sqrt{n^2-\alpha^2}>0$. The [simple harmonic motion](../../../../../../../simple-harmonic-motion.md) equation has [solution of a differential equation](../../../../../../../solution-of-a-differential-equation.md)

$$
\boxed{F(t)=\frac{\sin(\nu t)}\nu,\qquad \nu=\sqrt{n^2-\alpha^2}.}
$$

This is an [underdamped](../../../../../../../underdamping.md) [normal mode](../../../../../../../normal-mode.md): its oscillations have the decaying factor $e^{-\alpha t}$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
