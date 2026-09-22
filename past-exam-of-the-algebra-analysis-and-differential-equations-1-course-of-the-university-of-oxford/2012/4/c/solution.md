<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $F=\mathbb R^n\setminus\Omega$. This is a [closed set](../../../../closed-set.md). First assume $F$ is nonempty. The [Heine-Borel theorem](../../../../heine-borel-theorem.md) makes the nonempty bounded [closed set](../../../../closed-set.md) $K$ a [compact set](../../../../compact-space.md). By the preceding parts, $x\mapsto d(x,F)$ is a [continuous function](../../../../continuous-function.md) and is strictly positive at every $x\in K$, because $K\subset\Omega$.

The [extreme value theorem](../../../../extreme-value-theorem.md) gives $x_*\in K$ attaining its minimum. Therefore

$$
\boxed{\operatorname{dist}(K,F)=\min_{x\in K}d(x,F)=d(x_*,F)>0.}
$$

The equality with the [distance between two sets](../../../../distance-between-two-sets.md) follows by taking the two [infima](../../../../infimum.md) successively. Crucially, [compactness](../../../../compact-space.md) supplies a point attaining the minimum; positivity at each point alone would not make an arbitrary [infimum](../../../../infimum.md) positive. This is the principle that a [compact subset of an open set has positive distance from its complement](../../../../compact-subset-of-an-open-set-has-positive-distance-from-its-complement.md).

If $\Omega=\mathbb R^n$, its [complement](../../../../complement-of-a-set.md) is empty. With the usual extended-real convention $\inf\varnothing=+\infty$, the stated inequality holds in that case too.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
