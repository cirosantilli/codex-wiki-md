<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Take $x$ horizontal, $y$ upward and $g>0$. Resolve [Newton's second law](../../../newton-s-second-law.md) into components for [projectile motion with linear drag](../../../projectile-motion-with-linear-drag.md):

$$
m\dot v_x=-\alpha v_x,\qquad
m\dot v_y=-mg-\alpha v_y,
\qquad v_x(0)=v_0\cos\theta,\quad v_y(0)=v_0\sin\theta.
$$

For $\alpha>0$, let $\tau_d=m/\alpha$. An [integrating factor](../../../integrating-factor.md) $e^{t/\tau_d}$ gives

$$
\boxed{v_x(t)=v_0\cos\theta\,e^{-t/\tau_d},\qquad
v_y(t)=\left(v_0\sin\theta+g\tau_d\right)e^{-t/\tau_d}-g\tau_d.}
$$

The relaxation [time](../../../time-in-physics.md) is $\tau_d$, and the [terminal velocity](../../../terminal-velocity.md) is $(0,-g\tau_d)$. For fixed finite $t$, expanding the [exponential function](../../../exponential-function.md) as $\alpha\to0$ gives the continuous limit $v_x=v_0\cos\theta$ and $v_y=v_0\sin\theta-gt$; the two terms proportional to $\tau_d$ cancel before taking the limit.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2017](../../2017-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
