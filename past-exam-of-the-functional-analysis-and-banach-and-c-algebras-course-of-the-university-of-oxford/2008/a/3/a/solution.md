<h1 id="a/3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [weak-star topology](../../../../../weak-star-topology.md) on $X^*$ is the coarsest topology making every evaluation $\phi\mapsto\phi(x)$ continuous. Finite intersections of evaluation inequalities form a neighborhood basis. Distinct functionals differ on some $x$, so disjoint disks around their evaluation values give disjoint neighborhoods; thus the topology is Hausdorff. The [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) states that the closed [unit ball](../../../../../unit-ball.md) of $X^*$ is [compact](../../../../../compact-space.md) in this topology.

If $f\in X^{**}$ is weak-star continuous, some $x_1,\ldots,x_n$ and $\varepsilon>0$ make $|f(\phi)|<1$ whenever $|\phi(x_i)|<\varepsilon$ for every $i$. If all evaluations vanish, every scalar multiple of $\phi$ lies in this neighborhood, forcing $f(\phi)=0$. Thus $f$ vanishes on the [kernel](../../../../../kernel-of-a-linear-map-split.md) of the map $E(\phi)=(\phi(x_1),\ldots,\phi(x_n))$. It factors linearly through the finite-dimensional range of $E$. Extending that factor algebraically to $\mathbb K^n$ gives scalars $a_i$ with

$$
f(\phi)=\sum_i a_i\phi(x_i)=\phi\left(\sum_i a_ix_i\right).
$$

Consequently **$f=J_Xx$** for $x=\sum_i a_ix_i$.

For the two induced topologies, let $B$ be the common [norm](../../../../../norm.md)-closed [unit ball](../../../../../unit-ball.md) and write $\tau_j=\sigma(Y,X_j)$. Under either topology $B$ is [compact](../../../../../compact-space.md) by Banach-Alaoglu, and the ambient space is Hausdorff. If the two topologies are comparable, the identity map from $B$ with the finer topology to $B$ with the coarser one is a [continuous bijection](../../../../../continuous-bijection.md) from a [compact space](../../../../../compact-space.md) to a [Hausdorff space](../../../../../hausdorff-space.md). Such a map is a [homeomorphism](../../../../../homeomorphism.md), since it carries closed [compact](../../../../../compact-space.md) sets to closed sets. Thus **in the comparable case the topologies agree on $B$**, giving alternative (a).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
