<h1 id="m/m5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a finite upper barrier $L>i$, let $h_i^{(L)}$ be the probability of hitting zero before $L$. It satisfies $h_0^{(L)}=1$, $h_L^{(L)}=0$, and $h_i^{(L)}=ph_{i+1}^{(L)}+qh_{i-1}^{(L)}$. For $0<q<p$, solving the second-order recurrence with roots $1$ and $r=q/p$ gives

$$
h_i^{(L)}=\frac{r^i-r^L}{1-r^L}.
$$

As $L\to\infty$, the events increase to eventual hitting of zero: any finite path reaching zero has a finite maximal height. Since $r<1$, this yields $\boxed{h_i=(q/p)^i}$, with $h_0=1$. In the endpoint case $q=0$, a positive initial state only moves upward and the [hitting probability](../../../../../../hitting-probability.md) is zero, agreeing with the positive-state formula. The finite-barrier argument selects the correct solution rather than the also-harmonic constant one.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [M5](../../../m5.md)
4. [M](../../../../m.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
