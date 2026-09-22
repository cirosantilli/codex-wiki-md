<h1 id="22f/solution">Solution</h1>

↑ **Parent:** [22F](../22f.md)

In the supremum-norm metric, $S$ is [totally bounded](../../../../../totally-bounded-space.md) if for every $\varepsilon>0$ finitely many norm balls of radius $\varepsilon$ cover it. It is uniformly bounded if some $M$ satisfies $|f(x)|\le M$ for all $f\in S,x\in K$. It is [equicontinuous](../../../../../equicontinuity.md) if for each $x\in K$ and $\varepsilon>0$ there is a neighbourhood $U$ of $x$ with $|f(y)-f(x)|<\varepsilon$ for all $f\in S,y\in U$. This definition works for compact Hausdorff $K$ without assuming it is metrizable.

Suppose $S$ is [totally bounded](../../../../../totally-bounded-space.md). A finite radius-one net makes $\|f\|_\infty$ uniformly bounded by one plus the largest norm of a net centre. For equicontinuity, choose a finite $\varepsilon/3$ net. Continuity of each centre gives a common neighbourhood of $x$ on which all centre values vary by less than $\varepsilon/3$. Approximating any $f$ by its centre and using the [triangle inequality](../../../../../triangle-inequality.md) at $x$ and $y$ bounds its variation by $\varepsilon$. Thus both conditions follow.

Conversely suppose those two conditions hold. For each $x$, choose a neighbourhood $U_x$ on which every function varies from its value at $x$ by less than $\varepsilon/3$. Compactness provides a finite cover $U_{x_1},\ldots,U_{x_m}$. The [vectors](../../../../../vector.md) $(f(x_1),\ldots,f(x_m))$ form a bounded subset of $\mathbb C^m$, so partition their possible values into finitely many boxes of diameter less than $\varepsilon/3$ in the maximum-coordinate norm. From each occupied box choose one function as a representative. If $f$ and its representative $h$ have sample values in the same box, and $y\in U_{x_j}$, then

$$
|f(y)-h(y)|\le|f(y)-f(x_j)|+|f(x_j)-h(x_j)|+|h(x_j)-h(y)|<\varepsilon.
$$

These finitely many representatives are a norm net, proving **total boundedness is equivalent to uniform boundedness and equicontinuity**. This supplies the finite-net part of the [Arzelà-Ascoli theorem](../../../../../arzela-ascoli-theorem.md) directly.

For a bounded set that is not [totally bounded](../../../../../totally-bounded-space.md), take the standard unit [vectors](../../../../../vector.md) $S=\{e_n:n\ge1\}$ in the [Banach space](../../../../../banach-space-split.md) $\ell^2$. Their norms are one and their pairwise distances are $\sqrt2$. A ball of radius less than $\sqrt2/2$ contains at most one of them, so finitely many such balls cannot cover $S$.

## ↑ Ancestors (10)

1. [22F](../22f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
