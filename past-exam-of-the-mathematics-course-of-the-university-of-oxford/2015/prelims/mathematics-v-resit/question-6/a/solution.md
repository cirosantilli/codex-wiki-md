<h1 id="question-6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $w$ be the difference of two solutions. It is a [harmonic function](../../../../../../harmonic-function.md) in the open [rectangle](../../../../../../rectangle.md), continuous on its [closure](../../../../../../closure-topology.md), with

$$
w(x,0)=0,\qquad w_y(x,\pi)=0,\qquad
w_x(0,y)=w_x(\pi,y)=0.
$$

Interpret these [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md) classically on the open edges, with the corresponding first [derivatives](../../../../../../derivative.md) extending there. We use the [strong maximum principle for harmonic functions](../../../../../../strong-maximum-principle-for-harmonic-functions.md) together with [even reflection across a homogeneous Neumann boundary](../../../../../../even-reflection-across-a-homogeneous-neumann-boundary.md). This avoids imposing differentiability at the two bottom corners, where the original data fail a [corner compatibility condition for mixed boundary data](../../../../../../corner-compatibility-condition-for-mixed-boundary-data.md).

By continuity on the compact [rectangle](../../../../../../rectangle.md), $w$ attains a maximum $M$. Suppose $M>0$. It cannot occur on the bottom edge, where $w=0$. If it occurs in the interior, the [strong maximum principle for harmonic functions](../../../../../../strong-maximum-principle-for-harmonic-functions.md) makes $w$ constant, contradicting its bottom value. If it occurs on an open vertical or top edge, the zero [normal derivative](../../../../../../normal-derivative.md) allows an even [reflection](../../../../../../reflection-mathematics.md) across that edge. The reflected [harmonic function](../../../../../../harmonic-function.md) then has an interior maximum, giving the same contradiction.

The only remaining possibilities are the two top corners. Reflect evenly across both meeting edges. This gives a bounded [harmonic function](../../../../../../harmonic-function.md) on a punctured neighbourhood of the corner. The [removable singularity for a bounded harmonic function](../../../../../../removable-singularity-for-a-bounded-harmonic-function.md) fills the centre with its continuous value. The corner is now an interior maximum, again impossible. Therefore $w\leq0$. Applying the identical argument to $-w$ gives $w\geq0$.

Thus $\boxed{w=0}$, and **the solution is unique** among the continuous classical solutions with the stated edge conditions.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Question 6](../../question-6.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
