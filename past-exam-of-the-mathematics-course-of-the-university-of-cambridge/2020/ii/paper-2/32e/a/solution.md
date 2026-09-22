<h1 id="32e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Bendixson-Dulac criterion](../../../../../../bendixson-dulac-theorem.md) says the following. Let $D\subseteq\mathbb R^2$ be a [simply connected domain](../../../../../../simply-connected-domain.md), let $F=(f,g)$ be continuously differentiable, and suppose there is a continuously differentiable function $B$ such that

$$
\nabla\mathbin{\cdot}(BF)
=\frac{\partial(Bf)}{\partial x}
+\frac{\partial(Bg)}{\partial y}
$$

has one sign throughout $D$ and does not vanish identically on any open subset. Then $\dot z=F(z)$ has no [periodic orbit](../../../../../../periodic-orbit.md) contained in $D$.

Indeed, if a periodic orbit $\Gamma$ existed, simple connectivity would put its interior $U$ inside $D$. The vector field $F$, and hence $BF$, is tangent to $\Gamma$, so its outward flux is zero. The [divergence theorem](../../../../../../divergence-theorem.md) would give

$$
0=\int_\Gamma BF\mathbin{\cdot}n\,ds
=\iint_U\nabla\mathbin{\cdot}(BF)\,dx\,dy,
$$

contradicting the sign hypothesis.

The [Poincaré-Bendixson theorem](../../../../../../poincare-bendixson-theorem.md) states that a nonempty compact [omega-limit set](../../../../../../omega-limit-set.md) of a continuously differentiable planar flow that contains no [equilibrium point](../../../../../../equilibrium-point-of-a-dynamical-system.md) is a periodic orbit. More generally, when the omega-limit set contains only finitely many equilibria, it is either an equilibrium, a periodic orbit, or a union of equilibria and connecting trajectories.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [32E](../../32e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
