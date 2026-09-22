<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose a nonconstant [periodic orbit](../../../../periodic-orbit.md) exists for the continuously differentiable planar [vector field](../../../../vector-field.md). Uniqueness implies that its image over a minimal period is a simple closed curve, enclosing a region $\Omega$ of positive area. Along the orbit, the differential form $f\,dy-g\,dx$ vanishes because $dx=f\,dt$ and $dy=g\,dt$. [Green's theorem](../../../../green-theorem.md), with positive orientation, therefore gives

$$
0=\oint_{\partial\Omega}(f\,dy-g\,dx)=\iint_\Omega(f_x+g_y)\,dx\,dy<0,
$$

a contradiction. This is the [Bendixson-Dulac criterion](../../../../bendixson-dulac-theorem.md) in the whole plane; the fact that the enclosed region also lies in the domain is essential.

For the second-order equation set $y=\dot x$. The equivalent system is $\dot x=y$, $\dot y=-(1+x^2)y-\cos x$. Its [divergence](../../../../divergence.md) is $\boxed{-(1+x^2)<0}$ throughout the plane. Hence **there are no nonconstant periodic solutions**.

The nonconstant qualification is necessary: the [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) solutions $x(t)\equiv\pi/2+k\pi$, $k\in\mathbb Z$, do exist and are periodic in the literal sense of satisfying every positive period. The source's usual dynamical interpretation of “[periodic solution](../../../../periodic-solution.md)” here is a nonconstant [periodic orbit](../../../../periodic-orbit.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2008 printed variant](../../../2008-printed-variant-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
