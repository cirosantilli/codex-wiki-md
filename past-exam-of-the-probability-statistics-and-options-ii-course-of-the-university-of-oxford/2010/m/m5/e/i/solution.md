<h1 id="m/m5/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The stationarity equation at an interior state collects arrivals from its two neighbors and itself:

$$
\pi_i=a\pi_{i-1}+(1-a-b)\pi_i+b\pi_{i+1}.
$$

This rearranges to the required recurrence. At zero, stationarity gives $\pi_0=(1-a)\pi_0+b\pi_1$, hence $\boxed{b\pi_1=a\pi_0}$.

The recurrence says the flux $a\pi_{i-1}-b\pi_i$ equals $a\pi_i-b\pi_{i+1}$. The boundary equation makes that flux zero, so $\pi_i=(a/b)^i\pi_0$. Since $0\le a/b<1$, normalization gives

$$
\boxed{\pi_i=(1-a/b)(a/b)^i\quad(i\ge0).}
$$

When $a=0$ this means $\pi_0=1$ and $\pi_i=0$ for $i>0$. The probability assumptions also require $a,b\ge0$, $a+b\le1$, as implicit in the transition rules.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [E](../../e.md)
3. [M5](../../../m5.md)
4. [M](../../../../m.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
