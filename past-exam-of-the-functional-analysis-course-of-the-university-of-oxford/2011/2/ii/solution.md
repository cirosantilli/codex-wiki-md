<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [weak topology](../../../../weak-topology-split.md) is coarser than the [norm](../../../../norm.md) topology, so [norm convergence](../../../../norm-convergence.md) implies [weak convergence](../../../../weak-convergence.md), and

$$
\overline C^{\|\cdot\|}\subseteq\overline C^{\mathrm{weak}}.
$$

For the reverse inclusion, let $x\notin K=\overline C^{\|\cdot\|}$. The set $K$ is closed and convex. The [Hahn-Banach separation theorem](../../../../hahn-banach-separation-theorem.md) supplies $f\in X^*$ and $a\in\mathbb R$ such that $f(x)>a\geq\sup_{y\in K}f(y)$. The set $\{z:f(z)>a\}$ is weakly open, contains $x$ and misses $C$. Hence $x$ is outside the weak [closure](../../../../closure-topology.md) as well. If $C$ is empty the equality is immediate. Therefore

$$
\boxed{\overline C^{\mathrm{weak}}=\overline C^{\|\cdot\|}\quad\text{for every convex }C.}
$$

The separating functional explains the role of convexity: an arbitrary norm-closed subset need not be weakly closed.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the functional analysis course of the University of Oxford](../../../split.md)
5. [Functional analysis course of the University of Oxford](../../../../functional-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
