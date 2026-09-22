<h1 id="a/1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A subset is [totally bounded](../../../../../totally-bounded-space.md) if for every $\varepsilon>0$ it has a finite cover by balls of radius $\varepsilon$. If its [closure](../../../../../closure-topology.md) is [compact](../../../../../compact-space.md), the cover by all such balls has a finite subcover, proving total boundedness.

Conversely, cover $S$ by finitely many balls of radius $2^{-r}$ at stage $r$. Starting with all indices, at least one ball contains infinitely many of the currently indexed terms. Retain those indices as $\sigma_r$. These sets are infinite and nested, and two terms indexed by $\sigma_r$ have distance less than $2^{1-r}$. Choose increasing $n_r\in\sigma_r$; then $(x_{n_r})$ is Cauchy, because all its terms after stage $r$ lie in that same ball. If $M$ is complete it converges. To cover sequences in the [closure](../../../../../closure-topology.md) as well, approximate their $n$th terms by points of $S$ at distance less than $1/n$ and apply this argument. The corresponding subsequence in the [closure](../../../../../closure-topology.md) has the same limit. [Sequential compactness](../../../../../sequentially-compact-space.md) therefore proves **total boundedness implies relative compactness in a complete ambient space**.

The [Arzelà-Ascoli theorem](../../../../../arzela-ascoli-theorem.md) says a subset of $C[0,1]$ is [relatively compact](../../../../../relatively-compact-subset.md) exactly when it is uniformly bounded and [equicontinuous](../../../../../equicontinuity.md). Pointwise boundedness together with [equicontinuity](../../../../../equicontinuity.md) is an equivalent version here. In the specified derivative-bounded family, the mean-value estimate gives $|f(t)-f(s)|\leq|t-s|$, uniformly over the family, while $\|f\|_\infty\leq1$. Thus this family is [relatively compact](../../../../../relatively-compact-subset.md).

For $V$, the image of the [unit ball](../../../../../unit-ball.md) has sup [norm](../../../../../norm.md) at most one and derivative $f$ of sup [norm](../../../../../norm.md) at most one; it lies in that family, so **$V$ is [compact](../../../../../compact-space.md)**.

For $W$, take $f_n=n\mathbf1_{[0,1/n]}$, each of $L^1$ [norm](../../../../../norm.md) one. Then $Wf_n(t)=\min(nt,1)$. Every subsequence converges pointwise to zero at $t=0$ and to one at every $t>0$. This limit is discontinuous, so no subsequence converges uniformly to a continuous function. Thus **$W$ is not [compact](../../../../../compact-space.md)**. The same integration formula has different compactness properties because the domain unit balls impose different controls.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [1](../../1.md)
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
