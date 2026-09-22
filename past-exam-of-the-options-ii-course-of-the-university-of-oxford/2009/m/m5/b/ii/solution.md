<h1 id="m/m5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $j\geq1$, the only incoming transition is from $j-1$, so a [stationary distribution](../../../../../../stationary-distribution.md) must satisfy

$$
\pi_j=\pi_{j-1}\frac\lambda j=\pi_0\frac{\lambda^j}{j!}.
$$

Normalization gives $\pi_0e^\lambda=1$, hence

$$
\boxed{\pi_j=e^{-\lambda}\frac{\lambda^j}{j!},\qquad j\geq0}.
$$

The zero-state balance also holds: $\sum_i\pi_i(1-\lambda/(i+1))=1-\sum_{j\geq1}\pi_j=\pi_0$. Thus the Poisson distribution is indeed stationary, including when $\lambda=1$. Irreducibility gives uniqueness.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
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
