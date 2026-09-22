<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $J:\mathbf{CompHaus}\hookrightarrow\mathbf{Top}$ be the inclusion. Both [categories](../../../../../../category-split.md) are [locally small categories](../../../../../../locally-small-category.md). By the [Tychonoff theorem](../../../../../../tychonoff-s-theorem.md), small [products in a category](../../../../../../product-category-theory.md) of [compact Hausdorff spaces](../../../../../../compact-hausdorff-space.md) are compact Hausdorff, with their ordinary product topology. The [equalizer](../../../../../../equaliser.md) of two continuous maps between compact Hausdorff spaces is closed in the source: it is the inverse image of the closed diagonal of the target. Hence it is again compact Hausdorff. The usual construction of small [categorical limits](../../../../../../categorical-limit.md) from products and equalizers proves that $\mathbf{CompHaus}$ is a [complete category](../../../../../../complete-category.md), and that $J$ preserves its small limits as limits in $\mathbf{Top}$.

We verify the [solution-set condition](../../../../../../solution-set-condition.md) for an arbitrary [topological space](../../../../../../topological-space.md) $X$. Put $\kappa=|X|$ and $\theta=2^{2^\kappa}$. Given a continuous map $f:X\to K$ with $K$ compact Hausdorff, let

$$
Y=\overline{f(X)}\subseteq K.
$$

This closed subspace is compact Hausdorff, and $f(X)$ is dense in it. The allowed cardinal estimate therefore gives $|Y|\leq\theta$. The map $f$ factors through the continuous map $X\to Y$ and the subspace inclusion $Y\hookrightarrow K$.

Choose a fixed set $S$ of cardinality $\theta$. Consider all compact Hausdorff topologies on subsets of $S$, together with all continuous maps from $X$ into the resulting spaces. There are only a set of such topologies and functions. Every $Y$ above is homeomorphic to one of these spaces after relabelling its underlying set. Consequently every $X\to JK$ factors through a member of this set of maps. This proves the solution-set condition, including $X=\varnothing$.

The [general adjoint functor theorem](../../../../../../freyd-general-adjoint-functor-theorem.md) now gives the [compact Hausdorff reflection](../../../../../../compact-hausdorff-reflection.md)

$$
\boxed{\beta:\mathbf{Top}\longrightarrow\mathbf{CompHaus},\qquad\beta\dashv J.}
$$

Its unit $\eta_X:X\to J\beta X$ is universal for continuous maps from $X$ to compact Hausdorff spaces. For arbitrary $X$, this is a reflection, and the unit is not required to be a topological embedding.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
