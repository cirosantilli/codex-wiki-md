<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [survivor functions](../../../../../../survival-function.md), $F_A'(u)=-f_A(u)$ and $F_B'(u)=-f_B(u)$. The [product rule](../../../../../../product-rule.md) gives

$$
\frac{d}{du}[F_A(u)F_B(u)]=-f_A(u)F_B(u)-F_A(u)f_B(u).
$$

Integrating from 0 to $t$, using $F_A(0)=F_B(0)=1$, yields

$$
\boxed{\int_0^t f_A(u)F_B(u)\,du+\int_0^t F_A(u)f_B(u)\,du+F_A(t)F_B(t)=1.}
$$

The three terms partition the possible histories: A occurs first by time $t$, B occurs first by time $t$, or neither has occurred by $t$. The first two are the [cumulative incidence functions](../../../../../../cumulative-incidence-function.md) for the two [competing risks](../../../../../../competing-risks.md), while the third is the [survival probability](../../../../../../survival-probability.md) of their minimum. The initial value assumes nonnegative event times with no atom at zero.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
