<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Poincaré-Bendixson theorem](../../../../../poincare-bendixson-theorem.md) states that the omega-limit set of a forward orbit confined to a compact region of the plane, containing no [equilibrium points](../../../../../equilibrium-point-of-a-dynamical-system.md), is a [periodic orbit](../../../../../periodic-orbit.md).

Put $x=R\cos\theta$, $y=R\sin\theta$. Direct calculation gives

$$
\dot R=R[1-H(\theta)R^2],\quad H=1+\tfrac12\sin^2\theta-\sin^4\theta,\qquad\dot\theta=1+R^2\cos\theta\sin^3\theta.
$$

Here $1/2\leq H\leq17/16$ and $|\cos\theta\sin^3\theta|\leq3\sqrt3/16$. Thus on the inner circle $R=\sqrt3/2$ the radial velocity is positive, and on the outer circle $R=3/2$ it is negative. In their closed annulus,

$$
\dot\theta\geq1-\frac{27\sqrt3}{64}>0,
$$

so there is no equilibrium. The theorem gives a [periodic orbit](../../../../../periodic-orbit.md) in this trapping annulus.

It is asymptotically stable: the vector-field [divergence](../../../../../divergence.md) is

$$
2-4x^2-3y^2\leq2-3R^2\leq-1/4
$$

throughout the annulus. Its nontrivial [Floquet multiplier](../../../../../floquet-multiplier.md) is $\exp\int_0^T\operatorname{div}F\,dt<1$. This proves **an attracting [periodic orbit](../../../../../periodic-orbit.md) exists**. There can be only one there: two such nested orbits would enclose an annular region with zero outward flux, contradicting the strictly negative [divergence](../../../../../divergence.md) via the [divergence theorem](../../../../../divergence-theorem.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
