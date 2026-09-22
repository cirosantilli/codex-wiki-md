<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $S$ be the original [sequence](../../../../../sequence.md) and $n=b-a$. The [loop invariant](../../../../../loop-invariant.md) is

$$
0\leq c\leq d\leq N,\qquad d-c=n,\qquad
\operatorname{bag}(u[c..d))=\operatorname{bag}(S).
$$

Here $\operatorname{bag}$ denotes the [multiset](../../../../../multiset.md) of entries. The capacity condition uses the question's assumption of sufficient space. Removing two runs of combined length $z$ and appending their merge preserves the length and [multiset](../../../../../multiset.md). It also leaves all live values in one contiguous segment.

For a nonempty live [sequence](../../../../../sequence.md), let $R$ be its number of [maximal initial runs](../../../../../maximal-initial-run.md) obtained by repeatedly cutting at strict adjacent descents. The [loop variant](../../../../../loop-variant.md) is $R-1$. If `x = d`, there is one run and the procedure returns a sorted [permutation](../../../../../permutation.md). Otherwise the iteration removes two runs and appends one; it cannot create a new descent inside that appended run. The appended run may join the last old run, further reducing $R$, so $R$ decreases by at least one. There are at most $R_0-1\leq n-1$ merges.

$$
\boxed{\text{Preserved length and multiset, plus decreasing run count, imply total correctness}.}
$$

For $n=0$, the loop is skipped and the empty segment is already sorted. No global stability claim is needed: moving a merged run behind other runs can change the order of equal-labelled occurrences.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
