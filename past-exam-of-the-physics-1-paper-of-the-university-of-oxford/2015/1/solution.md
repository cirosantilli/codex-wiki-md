<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take the launch point as $(x,y)=(0,0)$ and ignore air [drag](../../../drag-physics.md). In [projectile motion](../../../projectile-motion.md) with constant [gravitational acceleration](../../../gravitational-acceleration.md) $g$, a launch at [angle](../../../angle.md) $\theta$ above the horizontal gives

$$
x=v_0t\cos\theta,\qquad y=v_0t\sin\theta-\frac12gt^2.
$$

At the wall $x=l$, the height is

$$
y(l)=l\tan\theta-\frac{gl^2}{2v_0^2}\sec^2\theta
=lq-\frac{gl^2}{2v_0^2}(1+q^2),\qquad q=\tan\theta.
$$

This is a concave [quadratic polynomial](../../../quadratic-polynomial.md) in $q$, so its unique maximum satisfies $l-gl^2q/v_0^2=0$. Hence

$$
\boxed{\theta_{\max}=\arctan\frac{v_0^2}{gl},\qquad y_{\max}(l)=\frac{v_0^2}{2g}-\frac{gl^2}{2v_0^2}.}
$$

For $l=v_0^2/g$, the best trajectory has $\theta=45^\circ$ and reaches the wall at launch height. For $l>v_0^2/g$, the mathematical maximum height is negative. If the ball must stay above level ground, it lands before reaching the wall: $v_0^2/g$ is the maximum same-level [projectile range](../../../projectile-range.md). If there is no intervening ground and the wall extends below the launch height, the same optimum still applies, but its impact point is below that height.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2015](../../2015-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
