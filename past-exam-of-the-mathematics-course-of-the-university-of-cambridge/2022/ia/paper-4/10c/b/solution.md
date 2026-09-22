<h1 id="10c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The circular constraint is

$$
x=R\sin\theta,\qquad z=R\cos\theta.
$$

Its tangent in the $xz$-plane is $(\cos\theta,0,-\sin\theta)$, while the [normal force](../../../../../../normal-force.md) is radial. Projecting the equations from part (a) onto this tangent eliminates the normal force and gives

$$
\boxed{
R\ddot\theta
=-g\sin\theta+\Omega^2R\cos\theta\sin\theta
-2\Omega\dot y\cos\theta}.
$$

Because the ramp is translation-invariant along $y$, $N_y=0$; using $\dot x=R\dot\theta\cos\theta$ gives

$$
\boxed{\ddot y=\Omega^2y+2\Omega R\dot\theta\cos\theta}.
$$

For rest in the rotating frame, $\dot\theta=\dot y=\ddot\theta=\ddot y=0$. Assuming $\Omega\ne0$, the second equation gives $y=0$, and the first gives

$$
\sin\theta(\Omega^2R\cos\theta-g)=0.
$$

On the semicircular ramp the rest points are therefore

$$
\boxed{\theta=0,\ y=0}
$$

and, when $\Omega^2R\geq g$,

$$
\boxed{\theta=\pm\arccos\frac{g}{\Omega^2R},\ y=0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10C](../../10c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
