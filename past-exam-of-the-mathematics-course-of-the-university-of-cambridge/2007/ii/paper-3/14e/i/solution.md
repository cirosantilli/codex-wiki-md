<h1 id="14e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose **$A=B=\sigma/r$** in the proposed [Lyapunov function](../../../../../../lyapunov-function.md). The cubic terms cancel and direct differentiation gives

$$
\dot V=-\sigma x^2+2\sigma xy-\frac\sigma r y^2-\frac{\sigma b}r z^2
=-\sigma(x-y)^2-\sigma(1/r-1)y^2-\frac{\sigma b}r z^2.
$$

For $0<r<1$ this is negative definite, while $V$ is positive definite and radially unbounded. Finite-dimensional equivalence of these positive quadratic forms gives $\dot V\leq-cV$ for some $c>0$. Thus $V(t)\leq V(0)e^{-ct}$, every solution remains bounded and exists for all forward times, and every solution tends to zero. Therefore **the origin is globally asymptotically stable**, indeed exponentially stable.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [14E](../../14e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
