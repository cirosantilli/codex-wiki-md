<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

Call an index $n$ a peak if $a_n\geq a_m$ for every $m>n$. If there are infinitely many peaks, list their indices increasingly. Each selected value is at least every later selected value, so this gives a nonincreasing [subsequence](../../../../../subsequence.md).

If there are only finitely many peaks, choose an index beyond the last one. Every index from then onward has a later index with strictly larger value. Select these recursively: $n_{j+1}>n_j$ with $a_{n_{j+1}}>a_{n_j}$. This gives an increasing [subsequence](../../../../../subsequence.md). Neither [complex argument](../../../../../argument-complex-analysis.md) requires the original [sequence](../../../../../sequence.md) to be bounded. **Every real [sequence](../../../../../sequence.md) therefore has a monotone [subsequence](../../../../../subsequence.md)**, as asserted by the [monotone subsequence theorem](../../../../../monotone-subsequence-theorem.md).

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
