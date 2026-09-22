<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**An infinite-dimensional reflexive example is $\ell^2$**, by the [Riesz representation theorem](../../../../../riesz-representation-theorem.md).

The [weak topology](../../../../../weak-topology-split.md) on $X$ is the coarsest topology making every $f\in X^*$ continuous. The [weak-star topology](../../../../../weak-star-topology.md) on $X^*$ is the coarsest making every evaluation $f\mapsto f(x)$, $x\in X$, continuous. In each case basic neighborhoods impose finitely many evaluation inequalities. The [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) states that the [closed unit ball](../../../../../closed-unit-ball.md) of a dual space is compact for its [weak-star topology](../../../../../weak-star-topology.md). The separation theorem needed here says: if $K$ is a nonempty weak-star compact [convex](../../../../../convex-function.md) subset of a dual space $E^*$ and $z\notin K$, then some $e\in E$ strictly separates them,

$$
\operatorname{Re}z(e)>\sup_{k\in K}\operatorname{Re}k(e).
$$

The real-part convention covers complex spaces; for real spaces omit it.

Let $K$ be the weak-star closure of $J_X(B_X)$ inside $B_{X^{**}}$. This is compact by Banach-Alaoglu, [convex](../../../../../convex-function.md), and nonempty. If $z\in B_{X^{**}}\setminus K$, separation in the dual pair $(X^{**},X^*)$ gives $f\in X^*$ with

$$
\operatorname{Re}z(f)>\sup_{x\in B_X}\operatorname{Re}f(x)=\|f\|.
$$

But $|z(f)|\leq\|z\|\|f\|\leq\|f\|$, a contradiction. Therefore $K=B_{X^{**}}$, proving the required [Goldstine theorem](../../../../../goldstine-theorem.md) density.

If $X$ is reflexive, $J_X$ identifies its [weak topology](../../../../../weak-topology-split.md) with the [weak-star topology](../../../../../weak-star-topology.md) of $X^{**}$ and carries $B_X$ onto $B_{X^{**}}$, so Banach-Alaoglu gives weak compactness. Conversely, if $B_X$ is weakly compact, its image is weak-star compact, hence closed in the [Hausdorff](../../../../../hausdorff-space.md) bidual topology. Density then forces $J_X(B_X)=B_{X^{**}}$. Scaling gives surjectivity on the entire bidual. Thus

$$
\boxed{B_X\text{ weakly compact}\iff X\text{ reflexive}.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
