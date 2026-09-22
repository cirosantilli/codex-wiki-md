<h1 id="a/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For every [ultrafilter](../../../../../ultrafilter.md) $\mathcal H$ on $X$, its image is an [ultrafilter](../../../../../ultrafilter.md) on the [compact space](../../../../../compact-space.md) $Y$, so it has a limit. That limit is unique because $Y$ is [Hausdorff](../../../../../hausdorff-space.md): distinct limits would have disjoint [neighborhoods](../../../../../neighbourhood-mathematics.md) both belonging to the same [proper filter](../../../../../proper-filter.md). Therefore $\Lambda$ is well-defined. Since $f[X]$ is [dense](../../../../../dense-set.md), every $b\in Y$ lies in $\overline{f[X]}$. Part (a), with $A=X$, supplies an [ultrafilter](../../../../../ultrafilter.md) mapping to $b$, proving [surjectivity](../../../../../surjective-function.md).

Suppose disjoint [subsets](../../../../../subset.md) have disjoint image [closures](../../../../../closure-topology.md). If $\mathcal H\ne\mathcal K$, choose $A\in\mathcal H$ not in $\mathcal K$; the [ultrafilter](../../../../../ultrafilter.md) criterion gives $X\setminus A\in\mathcal K$. Part (a) gives

$$
\Lambda(\mathcal H)\in\overline{f[A]},\qquad
\Lambda(\mathcal K)\in\overline{f[X\setminus A]}.
$$

The two [closures](../../../../../closure-topology.md) are disjoint by assumption, so the limits differ. Thus $\Lambda$ is [injective](../../../../../injective-function.md).

Conversely, suppose $\Lambda$ is [injective](../../../../../injective-function.md) and disjoint $A,B\subseteq X$ had a common point $b$ in their image [closures](../../../../../closure-topology.md). Part (a) would supply [ultrafilters](../../../../../ultrafilter.md) $\mathcal H,\mathcal K$ containing $A,B$ respectively, both with image limit $b$. They must be distinct, since a [proper filter](../../../../../proper-filter.md) cannot contain the disjoint [sets](../../../../../set-split.md) $A$ and $B$ simultaneously. This contradicts [injectivity](../../../../../injective-function.md). Hence

$$
\boxed{\Lambda\text{ injective}\quad\Longleftrightarrow\quad
\overline{f[A]}\cap\overline{f[B]}=\varnothing\text{ whenever }A\cap B=\varnothing.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
