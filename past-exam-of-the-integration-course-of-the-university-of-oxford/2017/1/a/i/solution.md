<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If $\sum_nm^*(A_n)=\infty$, the required inequality is automatic. Otherwise each $A_n$ has finite [Lebesgue outer measure](../../../../../lebesgue-outer-measure.md). Fix $\varepsilon>0$. By the defining [infimum](../../../../../infimum.md), for each $n\geq1$ choose a countable [interval](../../../../../interval-mathematics.md) cover $\{J_{n,k}:k\geq1\}$ with

$$
\sum_{k\geq1}|J_{n,k}|<m^*(A_n)+\varepsilon2^{-n}.
$$

The family indexed by $(n,k)\in\mathbb N^2$ is countable and covers $\bigcup_nA_n$. Since all lengths are nonnegative, its total length is at most $\sum_nm^*(A_n)+\varepsilon$. Taking the infimum over covers of the union and then letting $\varepsilon\downarrow0$ gives

$$
\boxed{m^*\!\left(\bigcup_{n\geq1}A_n\right)\leq\sum_{n\geq1}m^*(A_n).}
$$

This proves [countable subadditivity of Lebesgue outer measure](../../../../../countable-subadditivity-of-lebesgue-outer-measure.md) directly from interval covers, without assuming that any $A_n$ is measurable.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
