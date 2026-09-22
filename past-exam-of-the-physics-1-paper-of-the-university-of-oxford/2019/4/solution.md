<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write the incoming particle [speed](../../../speed.md) as $u>0$, its final signed [speed](../../../speed.md) as $v$, and the rod's final [centre-of-mass velocity](../../../center-of-mass-velocity.md) along the impact direction as $V$. Let $b$ be the signed impact distance from the centre, and choose the sign of the [angular velocity](../../../angular-velocity.md) $\Omega$ so that the contact point's [velocity](../../../velocity.md) component is $V+b\Omega$. The rod's central [moment of inertia](../../../moment-of-inertia.md) is $I=ML^2/12$.

The [impulse](../../../impulse.md) delivered to the rod is $MV$. Conservation of linear and angular [momentum](../../../momentum-split.md) gives

$$
u=v+V,\qquad I\Omega=MbV.
$$

Using these in conservation of [kinetic energy](../../../kinetic-energy.md),

$$
u^2=v^2+V^2+\frac IM\Omega^2
\quad\Longrightarrow\quad
V=\frac{2u}{2+Mb^2/I},\qquad
v=\frac{(Mb^2/I)u}{2+Mb^2/I}.
$$

This is the equal-mass instance of the [effective contact mass](../../../effective-contact-mass.md) calculation. For $u>0$, both final speeds are nonnegative, so equal speeds require $v=V=u/2$. Therefore $Mb^2/I=2$ and

$$
\boxed{|b|=\frac L{\sqrt6}.}
$$

Both symmetric impact points lie on the rod, since $L/\sqrt6<L/2$.

More generally, the relative contact [velocity](../../../velocity.md) immediately afterwards is

$$
v-(V+b\Omega)=u-(2+Mb^2/I)V=-u.
$$

Thus its magnitude equals the incoming relative [speed](../../../speed.md) $u$ and its direction reverses. At the specified impact point, $V+b\Omega=3u/2$ and $v=u/2$, which makes the reversal particularly explicit.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2019](../../2019-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
