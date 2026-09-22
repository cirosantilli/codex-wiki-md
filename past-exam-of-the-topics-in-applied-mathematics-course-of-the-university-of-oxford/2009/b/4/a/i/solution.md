<h1 id="b/4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) is [asymptotically stable](../../../../../../asymptotic-stability.md) when it is Lyapunov stable and attracts every initial state in some neighbourhood. [Lyapunov stability](../../../../../../lyapunov-stability.md) means that sufficiently small initial displacement stays small for all future times; attraction additionally requires convergence to the [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md). A [Lyapunov function](../../../../../../lyapunov-function.md) is a differentiable positive-definite scalar function near the [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) whose [derivative](../../../../../../derivative.md) along solutions is nonpositive. Strict negativity, or an appropriate invariant-set argument for a non-strict [derivative](../../../../../../derivative.md), gives [asymptotic stability](../../../../../../asymptotic-stability.md).

For $\nu=-1$, [equilibria](../../../../../../equilibrium-point-of-a-dynamical-system.md) satisfy $y=0$ and $x+x^3=0$, so only $(0,0)$ is real. Its [Jacobian matrix](../../../../../../jacobian-matrix.md) is $\left(\begin{smallmatrix}0&1\\-1&0\end{smallmatrix}\right)$, with [eigenvalues](../../../../../../eigenvalue.md) $\pm i$ for every $\kappa$. It is a linear [centre equilibrium](../../../../../../center-equilibrium.md), so [linearization](../../../../../../linearization.md) alone cannot decide nonlinear attraction.

Use the positive proper [energy](../../../../../../energy-split.md)

$$
E=\tfrac12y^2+\tfrac12x^2+\tfrac14x^4,\qquad\boxed{\dot E=\kappa x^2y^2.}
$$

For $\kappa<0$, [energy](../../../../../../energy-split.md) sublevel sets are [compact](../../../../../../compact-space.md) and invariant. The zero-derivative set is the union of the axes, but its only invariant subset is the origin: on $x=0,y\ne0$ one immediately leaves that axis, and on $y=0,x\ne0$ one has $\dot y=-x-x^3\ne0$. [LaSalle's invariance principle](../../../../../../lasalle-s-invariance-principle.md) therefore proves global [asymptotic stability](../../../../../../asymptotic-stability.md). At $\kappa=0$ the conserved [energy](../../../../../../energy-split.md) levels are closed [periodic orbits](../../../../../../periodic-orbit.md), giving a nonlinear [centre equilibrium](../../../../../../center-equilibrium.md). For $\kappa>0$, time reversal together with $y\mapsto-y$ converts the system to the attracting negative-$\kappa$ case, so the origin is a nonlinear repeller and is unstable. Nonzero forward trajectories cannot remain bounded; this does not assert existence for all time if finite-time escape occurs.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [B](../../../../b.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../../split.md)
7. [Topics in applied mathematics course of the University of Oxford](../../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
