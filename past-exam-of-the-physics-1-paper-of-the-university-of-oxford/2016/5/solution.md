<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Choose the cylinder's [velocity](../../../velocity.md) to be $v\hat{\mathbf x}$, and the ball's laboratory [velocity](../../../velocity.md) to be $u(\cos\theta,\sin\theta)$. By [Galilean velocity addition](../../../galilean-velocity-addition.md), the ball's [velocity](../../../velocity.md) relative to the cylinder is

$$
\mathbf u'=\bigl(u\cos\theta-v,\ u\sin\theta\bigr).
$$

For a suitably centred entry without hitting a wall, the cylinder's axis must be parallel to this relative [velocity](../../../velocity.md). Its oriented [angle](../../../angle.md) $\alpha$ to the cylinder's direction of travel is therefore

$$
\boxed{\alpha=\operatorname{atan2}(u\sin\theta,u\cos\theta-v).}
$$

Equivalently, $\tan\alpha=u\sin\theta/(u\cos\theta-v)$, with the quadrant chosen from the two components. For $v/u\ll1$,

$$
\boxed{\alpha=\theta+\frac vu\sin\theta+O((v/u)^2).}
$$

Thus the extra tilt relative to the ball's original direction is approximately $(v/u)\sin\theta$. The use of $\operatorname{atan2}$ also covers nearly transverse incidence, where taking an unqualified inverse tangent could select the wrong axis direction.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2016](../../2016-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
