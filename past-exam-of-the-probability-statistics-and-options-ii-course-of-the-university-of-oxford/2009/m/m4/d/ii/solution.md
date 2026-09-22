<h1 id="m/m4/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The total is the [independent](../../../../../../independent-random-variables.md) random sum $Z_t=\sum_{j=1}^{N_t}Y_j$, with the empty sum zero. Conditional on $N_t=n$, its moment generating function is $M_Y(\theta)^n$. The Poisson probability generating function therefore gives

$$
\boxed{M_{Z_t}(\theta)=\exp\{\lambda t(M_Y(\theta)-1)\}.}
$$

Assuming a moment generating function in a neighborhood of zero, write $\mu=\mathbb E[Y]$ and $s^2=\operatorname{Var}(Y)$. Conditional [expectation](../../../../../../expected-value-split.md) and [variance](../../../../../../variance-split.md) yield

$$
\boxed{\mathbb E[Z_t]=\lambda t\mu,\qquad\operatorname{Var}(Z_t)=\lambda t(s^2+\mu^2)=\lambda t\mathbb E[Y^2].}
$$

The second contribution to the [variance](../../../../../../variance-split.md) is due to randomness in the number of arriving coaches, not just randomness in the occupancy of each coach.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [M4](../../../m4.md)
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
