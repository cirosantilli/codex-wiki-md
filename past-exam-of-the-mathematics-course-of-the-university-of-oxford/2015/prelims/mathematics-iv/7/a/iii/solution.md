<h1 id="7/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [fixed-point iteration](../../../../../../../fixed-point-iteration.md) stays inside $[0,7]$ because $G$ maps that interval to itself. A [fixed point](../../../../../../../fixed-point.md) satisfies $\xi=\sqrt{2+\xi}$, so $\xi\ge0$ and

$$
\xi^2-\xi-2=(\xi-2)(\xi+1)=0.
$$

Only $\xi=2$ is admissible; $-1$ fails the unsquared equation. With $q=1/(2\sqrt2)$, the [mean value theorem](../../../../../../../mean-value-theorem.md) gives the [error bound](../../../../../../../error-bound.md)

$$
|x_{k+1}-2|=|G(x_k)-G(2)|\le q|x_k-2|.
$$

Induction yields $|x_k-2|\le q^k|x_0-2|\le5q^k\to0$, since $0<q<1$. Therefore, for every allowed starting value,

$$
\boxed{\lim_{k\to\infty}x_k=2.}
$$

This estimate proves convergence directly, without assuming in advance that the sequence has a limit.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Mathematics IV](../../../../mathematics-iv-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
