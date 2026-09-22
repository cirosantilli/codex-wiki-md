<h1 id="4a/solution">Solution</h1>

↑ **Parent:** [4A](../4a.md)

Measure displacement downward from the release point and take downward speed $v\geq0$. [Newton's second law](../../../../../newton-s-second-law.md) with [quadratic drag](../../../../../quadratic-drag.md) gives

$$
m\frac{dv}{dt}=mg-\gamma v^2,
\qquad v(0)=0.
$$

Writing

$$
V=\sqrt{\frac{mg}{\gamma}},
\qquad k=\sqrt{\frac{g\gamma}{m}},
$$

separation of variables gives the [terminal velocity](../../../../../terminal-velocity.md) solution

$$
v(t)=V\tanh(kt).
$$

The distance fallen by time $t$ is therefore

$$
y(t)=\int_0^tv(s)ds
=\frac{m}{\gamma}\log\cosh(kt).
$$

Setting $y(t)=h$ and solving for $t$ yields

$$
\boxed{t=\sqrt{\frac{m}{g\gamma}}\,
\operatorname{arcosh}\!\left(e^{\gamma h/m}\right)}.
$$

## ↑ Ancestors (10)

1. [4A](../4a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
