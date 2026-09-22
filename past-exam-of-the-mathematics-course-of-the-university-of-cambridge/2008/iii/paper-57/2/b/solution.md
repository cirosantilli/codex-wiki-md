<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Measuring the state from part (a) in the [computational basis](../../../../../../computational-basis.md) succeeds with [probability](../../../../../../probability.md) $p_n=\sin^2((2n+1)\theta)$. In the sparse-solution regime $0<M\leq2^{N-1}$, one has $0<\theta\leq\pi/4$. The first success interval with $p_n\geq1/2$ is $\pi/4\leq(2n+1)\theta\leq3\pi/4$. Entering it requires $n\geq\pi/(8\theta)-1/2$, so the [first half-probability Grover iterate](../../../../../../first-half-probability-grover-iterate.md) is

$$
\boxed{n_{\min}=\left\lceil\frac{\pi}{8\arcsin\sqrt{M/2^N}}-\frac12\right\rceil.}
$$

For this integer, the angle is at least $\pi/4$ and less than $\pi/4+2\theta\leq3\pi/4$, so the rounding cannot skip the required interval. Every smaller nonnegative integer has angle below $\pi/4$ and hence success below $1/2$, proving minimality. For $M\ll2^N$, the leading size is $n_{\min}\sim(\pi/8)\sqrt{2^N/M}$. If $M\geq2^{N-1}$, the initial measurement already succeeds with [probability](../../../../../../probability.md) at least one half and the smallest count is zero; if $M=0$ no search can succeed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
