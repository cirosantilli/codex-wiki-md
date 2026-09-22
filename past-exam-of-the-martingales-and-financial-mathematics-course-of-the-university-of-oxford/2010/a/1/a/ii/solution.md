<h1 id="a/1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $\varepsilon>0$, define the measurable decreasing tail events

$$
A_n(\varepsilon)=\bigcup_{m\geq n}\{|f_m-f|>\varepsilon\}
=\left\{\sup_{m\geq n}|f_m-f|>\varepsilon\right\}.
$$

If $f_n\to f$ almost everywhere, every point outside its null exceptional set eventually leaves each such tail event, so $\mu(\bigcap_nA_n(\varepsilon))=0$. [Continuity from above of a measure](../../../../../../continuity-from-above-of-a-measure.md) applies because $\mu(E)<\infty$, giving $\mu(A_n(\varepsilon))\to0$.

Conversely, assume these measures tend to zero. For each positive integer $k$, the intersection $\bigcap_nA_n(1/k)$ has measure zero. Outside the union of these countably many null sets, every $k$ has an index after which $|f_m-f|\leq1/k$ for all later $m$. Hence $f_m\to f$ there. This proves the desired equivalence. The argument uses all positive thresholds; replacing the intersection of tail events by a single strict limsup inequality at the same threshold would mishandle equality cases.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
