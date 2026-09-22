<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take downward [distance](../../../distance.md) $s$ and downward [speed](../../../speed.md) $v=ds/dt\geq0$, with constant [gravitational acceleration](../../../gravitational-acceleration.md) $g>0$ and [quadratic drag](../../../quadratic-drag.md) coefficient $k>0$. The printed vector square has no standard vector meaning; the directionally consistent [drag force](../../../drag-physics.md) is $\mathbf F_d=-mk|\mathbf v|\mathbf v$. For this downward fall, [Newton's second law](../../../newton-s-second-law.md) becomes

$$
\frac{dv}{dt}=g-kv^2.
$$

The [terminal velocity](../../../terminal-velocity.md) is obtained by setting the net [force](../../../force-split.md) to zero:

$$
\boxed{v_\infty=\sqrt{g/k}\quad\text{downward}.}
$$

From rest, the [speed](../../../speed.md) increases monotonically towards this limiting value. In fact $v(t)=v_\infty\tanh(\sqrt{gk}\,t)$; thus it is a [supremum](../../../supremum.md) approached at infinite time, and a tower of finite height need not permit it to be reached.

For the required [distance](../../../distance.md), use the [chain rule](../../../chain-rule.md) $dv/dt=v\,dv/ds$. Writing $w=v^2$ gives a [linear ordinary differential equation](../../../linear-ordinary-differential-equation-split.md):

$$
\frac{dw}{ds}+2kw=2g,\qquad w(0)=0,
\qquad
v^2(s)=\frac gk\left(1-e^{-2ks}\right).
$$

Consequently,

$$
\frac{v^2}{v_\infty^2}=\frac14=1-e^{-2ks},\qquad
\boxed{s_{1/2}=\frac{1}{2k}\log\frac43.}
$$

Here $k$ has units of inverse [length](../../../length.md), so the result has the required units of [distance](../../../distance.md) and is independent of the falling [mass](../../../mass.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2021](../../2021-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
