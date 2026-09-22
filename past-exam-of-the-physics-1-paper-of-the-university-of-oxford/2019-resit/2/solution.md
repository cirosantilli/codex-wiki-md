<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the [linear drag](../../../linear-drag.md) as $\mathbf F_d=-b\mathbf v$, with $b>0$, and let $m$ be the projectile's [mass](../../../mass.md). Taking upward as positive, [Newton's second law](../../../newton-s-second-law.md) gives

$$
m\dot v_y=-mg-bv_y,\qquad v_y(0)=u_0\sin\alpha.
$$

The downward [terminal velocity](../../../terminal-velocity.md) is $-v_t$, where

$$
\boxed{v_t=\frac{mg}{b}.}
$$

Equivalently, if the drag [acceleration](../../../acceleration.md) is specified as $-k\mathbf v$, then $v_t=g/k$. Solving the first-order equation,

$$
v_y(t)=(u_0\sin\alpha+v_t)e^{-bt/m}-v_t.
$$

The highest point occurs at $v_y=0$, so

$$
\boxed{t_{\rm top}=\frac mb\ln\left(1+\frac{u_0\sin\alpha}{v_t}\right)
=\frac{v_t}{g}\ln\left(1+\frac{u_0\sin\alpha}{v_t}\right).}
$$

For an upward launch this root is positive and $\dot v_y=-g$ there, confirming a maximum height. As $b\to0$, expanding the logarithm gives the drag-free result $t_{\rm top}\to u_0\sin\alpha/g$. A horizontal launch has its highest point at launch; a downward launch from the ground does not have a later airborne maximum.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
