<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose the heavier particle's outgoing [velocity](../../../velocity.md) above the initial direction. Let its [speed](../../../speed.md) be $V$, and let the lighter particle have components $(v\cos\theta,-v\sin\theta)$. Thus $\theta$ and $\phi$ are nonnegative deflections on opposite sides. [Conservation of momentum](../../../momentum-conservation.md) gives

$$
mu=mv\cos\theta+MV\cos\phi,
\qquad mv\sin\theta=MV\sin\phi.
$$

The [elastic collision](../../../elastic-collision.md) conserves [kinetic energy](../../../kinetic-energy.md):

$$
mu^2=mv^2+MV^2.
$$

Taking the squared magnitude of the vector [momentum](../../../momentum-split.md) equation yields

$$
m^2v^2=m^2u^2+M^2V^2-2mMuV\cos\phi.
$$

Eliminate $v^2$ with the [kinetic energy](../../../kinetic-energy.md) equation. For a nontrivial [collision](../../../collision.md), $V\ne0$, so

$$
(M+m)V=2mu\cos\phi.
$$

Substituting back into the two [momentum](../../../momentum-split.md) components gives

$$
v\cos\theta=\frac{u(m-M\cos2\phi)}{m+M},
\qquad
v\sin\theta=\frac{uM\sin2\phi}{m+M}.
$$

Therefore

$$
\boxed{\tan\theta=\frac{\sin2\phi}{m/M-\cos2\phi}.}
$$

The ratio alone does not determine the quadrant: for $M>m$, the lighter particle can move backwards. The two component equations select the correct $0\leq\theta\leq\pi$. At $m/M=\cos2\phi$, the outgoing direction is perpendicular to the initial direction; the displayed [tangent](../../../tangent.md) has a pole there.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2021 resit](../../2021-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
