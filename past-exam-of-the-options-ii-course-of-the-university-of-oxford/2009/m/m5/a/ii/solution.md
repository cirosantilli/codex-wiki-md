<h1 id="m/m5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First assume $0<q<p<1$. Stop the nearest-neighbour walk on reaching zero or a finite upper level $L>i$. Its probability $h_i^{(L)}$ of reaching zero first solves $h_i^{(L)}=ph_{i+1}^{(L)}+qh_{i-1}^{(L)}$, with boundary values one and zero. Solving this second-order recurrence gives

$$
h_i^{(L)}=\frac{(q/p)^i-(q/p)^L}{1-(q/p)^L}.
$$

Absorption in the finite interval occurs almost surely: from every interior state there is a uniformly positive probability of an absorbing run within $L$ steps. As $L\to\infty$, the events of hitting zero before $L$ increase to the event of ever hitting zero, since a path reaching zero at a finite time has a finite maximum before then. Consequently

$$
\boxed{h_i=(q/p)^i}.
$$

This limiting argument selects the actual [hitting probability](../../../../../../hitting-probability.md), rather than just an arbitrary bounded solution of the infinite recurrence. If $q=0$, the walk moves deterministically upwards from positive states and the probability is zero there; from state zero it is one. These agree with the formula interpreted separately at $i=0$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [M5](../../../m5.md)
4. [M](../../../../m.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
