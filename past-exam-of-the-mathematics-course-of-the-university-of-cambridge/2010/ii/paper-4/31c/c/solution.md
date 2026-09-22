<h1 id="31c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This is [endpoint asymptotics after odd Gaussian cancellation](../../../../../../endpoint-asymptotics-after-odd-gaussian-cancellation.md). All interior algebraic terms cancel because $\sin t\,e^{-\lambda t^2}$ is odd. Split the interval into $[-1,1]$ and the remaining tail:

$$
\int_{-2}^1\sin t\,e^{-\lambda t^2}\,dt
=-\int_1^2\sin t\,e^{-\lambda t^2}\,dt.
$$

The right-hand integral has its minimum phase at its left endpoint, with $\phi'(1)=2$ and nonzero amplitude $\sin1$. Endpoint [Laplace method](../../../../../../laplace-s-method.md) therefore give

$$
\boxed{I(\lambda)\sim-\frac{\sin1}{2\lambda}e^{-\lambda}.}
$$

The answer is exponentially small, rather than zero; applying only the interior Gaussian approximation misses the asymmetric boundary tail.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [31C](../../31c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
