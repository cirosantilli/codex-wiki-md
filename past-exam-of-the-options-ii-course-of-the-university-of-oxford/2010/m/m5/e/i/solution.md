<h1 id="m/m5/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $i\geq1$, the stationarity equation is

$$
\pi_i=a\pi_{i-1}+(1-a-b)\pi_i+b\pi_{i+1},
$$

which rearranges to the stated recurrence. At zero,

$$
\pi_0=(1-a)\pi_0+b\pi_1,
\qquad\boxed{b\pi_1=a\pi_0.}
$$

Define the adjacent probability current $J_i=a\pi_i-b\pi_{i+1}$. The recurrence says $J_i=J_{i-1}$, and the boundary equation says $J_0=0$. Hence $\pi_{i+1}=(a/b)\pi_i$ for all $i$. Since $\rho=a/b<1$, [normalization](../../../../../../normalization.md) gives

$$
\boxed{\pi_i=(1-\rho)\rho^i,\qquad\rho=\frac ab,\quad i\geq0.}
$$

The adjacent balance equations also verify stationarity directly. If $a=0$, this formula means the point mass at zero; otherwise the [birth-death chain](../../../../../../birth-death-chain.md) is irreducible and this is its unique stationary [probability distribution](../../../../../../probability-distribution-split.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [E](../../e.md)
3. [M5](../../../m5.md)
4. [M](../../../../m.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
