<h1 id="32a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Dulac theorem](../../../../../../bendixson-dulac-theorem.md) states the following. Let $D$ be a simply connected region for the planar system $\dot z=f(z)$, and suppose there is a continuously differentiable function $B:D\to\mathbb R$ for which

$$
\nabla\mathbin{\cdot}(Bf)
$$

has one strict sign throughout $D$. Then there is no [periodic orbit](../../../../../../periodic-orbit.md) contained in $D$.

To prove it, suppose a periodic orbit $\Gamma$ existed and let $A$ be its interior. Simple connectedness ensures $A\subset D$. By the planar [divergence theorem](../../../../../../divergence-theorem.md),

$$
\iint_A\nabla\mathbin{\cdot}(Bf)\,dA
=\int_\Gamma Bf\mathbin{\cdot}n\,ds.
$$

The vector field $f$ is tangent to its trajectory $\Gamma$, so its scalar product with the outward normal $n$ vanishes. The right-hand side is therefore zero. The left-hand side cannot be zero because its integrand has one strict sign, a contradiction.

The [Poincaré-Bendixson theorem](../../../../../../poincare-bendixson-theorem.md) states that if a forward trajectory of a smooth planar system remains in a compact set and its nonempty [omega-limit set](../../../../../../omega-limit-set.md) contains no equilibrium point, then that omega-limit set is a periodic orbit.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [32A](../../32a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
