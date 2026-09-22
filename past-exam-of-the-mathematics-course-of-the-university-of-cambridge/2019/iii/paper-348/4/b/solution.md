<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A standard sufficient form of [Brenier theorem](../../../../../../brenier-theorem.md) assumes $\mu,\nu\in\mathcal P(\mathbb R^d)$ have finite second [moments](../../../../../../moment.md) and $\mu\ll\mathcal L^d$, that is, [absolute continuity of measures](../../../../../../absolute-continuity-of-measures.md) with respect to [Lebesgue measure](../../../../../../lebesgue-measure.md). For the cost $|x-y|^2$, there exists a unique optimal [transport plan](../../../../../../transport-plan.md), and it is induced by a [transport map](../../../../../../transport-map.md):

$$
\boxed{\pi^\dagger=(\operatorname{Id},\nabla\Phi)_\#\mu,\qquad T^\dagger=\nabla\Phi,\qquad(\nabla\Phi)_\#\mu=\nu.}
$$

Here $\Phi$ is a [proper convex function](../../../../../../proper-convex-function.md), which may be chosen [sequentially lower semicontinuous](../../../../../../sequential-lower-semicontinuity.md), and its [gradient](../../../../../../gradient.md) exists $\mu$-almost everywhere. The map $\nabla\Phi$ is unique $\mu$-almost everywhere and is the unique minimizer of the [Monge optimal transport problem](../../../../../../monge-optimal-transport-problem.md); its cost equals the [Kantorovich optimal transport problem](../../../../../../kantorovich-optimal-transport-problem.md) minimum. Equivalently, it is the unique [gradient](../../../../../../gradient.md) of a [convex function](../../../../../../convex-function.md) transporting $\mu$ to $\nu$.

The uniqueness claim concerns the map and the [transport plan](../../../../../../transport-plan.md), not a globally unique potential. The potential may be shifted by a constant, and additional nonuniqueness away from the source can occur. No density assumption is required on $\nu$. A primary reference is [Brenier's Polar factorization and monotone rearrangement of vector-valued functions](https://www.ceremade.dauphine.fr/~carlier/Brenier91.pdf).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
