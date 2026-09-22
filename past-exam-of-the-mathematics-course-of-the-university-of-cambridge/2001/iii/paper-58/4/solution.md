<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Fix $\varepsilon>0$ and put $\eta=\varepsilon/2$. For each pair $s,t\in T$, choose $a_{s,t}\in A$ whose errors at these two points are smaller than $\eta$. By [continuity](../../../../../continuous-function.md), there is a neighborhood $U_{s,t}$ of $t$ on which $a_{s,t}>f-\eta$. For a fixed $s$, these neighborhoods cover the [compact space](../../../../../compact-space.md) $T$. Choose a finite subcover $U_{s,t_1},\ldots,U_{s,t_m}$ and form

$$
b_s=\max_{1\le j\le m}a_{s,t_j}\in A.
$$

Then $b_s>f-\eta$ everywhere, while $b_s(s)<f(s)+\eta$, because every chosen [function](../../../../../function-split.md) has error smaller than $\eta$ at $s$. Since $b_s$ is continuous, there is a neighborhood $W_s$ of $s$ on which $b_s<f+\eta$.

A second use of [compactness](../../../../../compact-space.md) supplies $W_{s_1},\ldots,W_{s_q}$ covering $T$. Set

$$
a=\min_{1\le i\le q}b_{s_i}\in A.
$$

Every $b_{s_i}$ is above $f-\eta$, so their minimum is also above it. At each point at least one $b_{s_i}$ is below $f+\eta$, and hence so is their minimum. This proves $\|a-f\|_\infty\le\eta<\varepsilon$. The two finite operations are the essential mechanism in [lattice approximation from two-point approximation](../../../../../lattice-approximation-from-two-point-approximation.md); no closure under addition or multiplication has been assumed.

For the corollary take $A$ to consist of all [continuous](../../../../../continuous-function.md) [piecewise linear functions](../../../../../piecewise-linear-function.md) on $[0,1]$. On a common finite partition, the maximum or minimum of two affine pieces can change which piece it selects only at their crossing. Adding those finitely many crossings to the partition shows that $A$ is closed under both operations. For two distinct points, the affine [polynomial](../../../../../polynomial-split.md) through the two prescribed values belongs to $A$ and matches $f$ exactly there; for equal points use a [constant function](../../../../../constant-function.md). The proved criterion therefore gives **density of continuous piecewise linear functions in $C[0,1]$ in the supremum norm**. Concretely, interpolation on a partition of maximum gap $h$ also gives error at most $\omega(f,h)$ by [uniform continuity](../../../../../uniform-continuity.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
