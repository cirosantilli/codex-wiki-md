<h1 id="e/e3/b/ii/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use three nested [sequences](../../../../../../../sequence.md):

$$
A_3=\left\{\left(\frac1n+\frac1{n^2m},\frac1{n^2m^2k}\right):n,m,k\geq1\right\}.
$$

For fixed $n,m$, letting $k\to\infty$ produces the point $(1/n+1/(n^2m),0)$. Letting $m\to\infty$ produces $(1/n,0)$, and letting $n\to\infty$ produces $(0,0)$. Accordingly, put

$$
B=\left\{\left(\frac1n+\frac1{n^2m},0\right):n,m\geq1\right\},\qquad
C=\{(1/n,0):n\geq1\}.
$$

The successive derived sets are

$$
\boxed{A_3'=B\cup C\cup\{(0,0)\},\quad A_3''=C\cup\{(0,0)\},\quad A_3^{\prime\prime\prime}=\{(0,0)\}.}
$$

To see that no limits are missing, take any [convergent sequence](../../../../../../../convergent-sequence.md) of distinct points from $A_3$. If $n$ is unbounded, a subsequence has $n\to\infty$ and converges to the origin. Otherwise fix $n$ on a subsequence. Unbounded $m$ then forces limit $(1/n,0)$; with $n,m$ fixed, distinctness forces unbounded $k$, giving the corresponding point of $B$. The same argument, with one index fewer at each stage, proves the next two equalities. Distinct $n$-clusters are separated away from the origin because their first coordinates lie in the disjoint [intervals](../../../../../../../interval-mathematics.md) $[1/n,1/n+1/n^2]$.

The original set has positive second coordinates, the first derived set has isolated $B$-points on the axis, the second has infinitely many $C$-points, and the third is a singleton. All three required successive inequalities follow. This is a [three-stage accumulation tower](../../../../../../../three-stage-accumulation-tower.md).

## ↑ Ancestors (15)

1. [3](../3.md)
2. [Ii](../../ii.md)
3. [B](../../../b.md)
4. [E3](../../../../e3.md)
5. [E](../../../../../e.md)
6. [2012](../../../../../../2012-split.md)
7. [Past exam of the options II course of the University of Oxford](../../../../../../split.md)
8. [Options II course of the University of Oxford](../../../../../../../options-ii-course-of-the-university-of-oxford.md)
9. [Year 2 of the mathematics course of the University of Oxford](../../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
10. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
11. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
12. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
13. [University of Oxford](../../../../../../../university-of-oxford-split.md)
14. [List of universities](../../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../../split.md)
