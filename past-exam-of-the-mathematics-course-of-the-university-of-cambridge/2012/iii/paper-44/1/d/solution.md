<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define $U(x)=U_0(\delta_x)$, where $\delta_x$ is the [Dirac measure](../../../../../../dirac-measure.md) at $x$. For the full [sigma-algebra](../../../../../../sigma-algebra.md) of subsets of a finite $E$, affineness directly gives $U_0(\lambda)=\sum_{x\in E}\lambda(\{x\})U(x)$.

The statement also holds for an arbitrary [sigma-algebra](../../../../../../sigma-algebra.md) on a [finite set](../../../../../../finite-set.md). List each [atom of a sigma-algebra](../../../../../../atom-of-a-sigma-algebra.md) as $A_1,\ldots,A_r$ and choose $x_j\in A_j$. Points in one atom have identical [Dirac measures](../../../../../../dirac-measure.md) on this [sigma-algebra](../../../../../../sigma-algebra.md), so $U$ is constant on each atom and is measurable. Every [probability measure](../../../../../../probability-measure.md) decomposes as $\lambda=\sum_j\lambda(A_j)\delta_{x_j}$, whence

$$
\boxed{U_0(\lambda)=\sum_j\lambda(A_j)U(x_j)=\int_EU(x)\,\lambda(dx).}
$$

This is the [expected utility representation on a finite measurable space](../../../../../../expected-utility-representation-on-a-finite-measurable-space.md). It does not silently assume that each singleton is measurable.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
