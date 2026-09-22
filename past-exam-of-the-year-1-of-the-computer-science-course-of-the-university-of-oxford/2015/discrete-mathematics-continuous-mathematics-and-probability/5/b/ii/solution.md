<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $h=1/N$, $x_j=jh$, and let $y_j$ approximate $y(x_j)$. The [forward Euler method](../../../../../../euler-method.md) gives the [difference equation](../../../../../../difference-equation.md)

$$
\boxed{y_{j+1}=y_j+h(-\lambda y_j)
=\left(1-\frac\lambda N\right)y_j,\qquad y_0=2.}
$$

This [geometric sequence](../../../../../../geometric-progression.md) has solution

$$
\boxed{y_j=2\left(1-\frac\lambda N\right)^j\quad(0\le j\le N),
\qquad y_N=2\left(1-\frac\lambda N\right)^N.}
$$

For fixed $\lambda$, the [limit](../../../../../../limit-of-a-function.md) as $N\to\infty$ is $2e^{-\lambda}$, as required by the exact solution.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
