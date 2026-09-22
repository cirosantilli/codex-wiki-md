<h1 id="30a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The direct [First Lyapunov theorem](../../../../../../first-lyapunov-theorem.md) says that a continuously differentiable positive-definite function $V$ near an equilibrium, with $\dot V\leq0$, proves stability. [LaSalle invariance principle](../../../../../../lasalle-s-invariance-principle.md) says that in a [compact](../../../../../../compact-space.md) positively invariant set, trajectories approach the largest invariant subset of $\{\dot V=0\}$. Under the terminology in which “first theorem” means the linearization theorem, [eigenvalues](../../../../../../eigenvalue.md) with negative real part imply [asymptotic stability](../../../../../../asymptotic-stability.md), while zero-real-part [eigenvalues](../../../../../../eigenvalue.md) leave the test inconclusive. Here the linearization has [eigenvalues](../../../../../../eigenvalue.md) $0,-k$, so the direct criterion is needed.

Write $y=\dot x$ and choose

$$
V(x,y)=\frac{y^2}2+\int_0^x\sin^3s\,ds
=\frac{y^2}2+\frac23-\cos x+\frac13\cos^3x.
$$

Near zero, $V=y^2/2+x^4/4+O(x^6)$ is positive definite. Along solutions,

$$
\dot V=y(-ky-\sin^3x)+\sin^3x\,y=\boxed{-ky^2\leq0}.
$$

The component containing the origin of a sufficiently small closed sublevel set is [compact](../../../../../../compact-space.md), lies in $|x|<\pi$ and is positively invariant. The set $\dot V=0$ has $y=0$; to remain there also requires $\sin^3x=0$, so its largest invariant subset is just the origin. The two theorems establish **the origin is asymptotically stable**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30A](../../30a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
