<h1 id="32a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $x_*$ be an [equilibrium point of a dynamical system](../../../../../../equilibrium-point-of-a-dynamical-system.md). A [Lyapunov function](../../../../../../lyapunov-function.md) on a neighbourhood of $x_*$ is a continuously differentiable function $V$ such that

$$
V(x_*)=0,\qquad V(x)>0\quad(x\ne x_*),
$$

and whose derivative along trajectories satisfies

$$
\dot V(x)=\nabla V(x)\cdot f(x)\leq0.
$$

The [First Lyapunov theorem](../../../../../../first-lyapunov-theorem.md) says that the existence of such a positive-definite $V$ proves [Lyapunov stability](../../../../../../lyapunov-stability.md) of $x_*$. If $\dot V<0$ away from $x_*$, the [Second Lyapunov theorem](../../../../../../second-lyapunov-theorem.md) strengthens this to [asymptotic stability](../../../../../../asymptotic-stability.md).

[LaSalle invariance principle](../../../../../../lasalle-s-invariance-principle.md) says that if a trajectory remains in a compact positively invariant set $\Omega$ on which $\dot V\leq0$, then it approaches the largest invariant subset of

$$
\{x\in\Omega:\dot V(x)=0\}.
$$

In particular, if that largest invariant subset consists only of $x_*$, every trajectory in $\Omega$ approaches $x_*$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [32A](../../32a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
