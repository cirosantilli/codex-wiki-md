<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The downstream [service rate of a queue](../../../../../../service-rate-of-a-queue.md) now exceeds the upstream cap for all sufficiently large $L$, since

$$
D L^{(1+\gamma)/2}>C L^{(1+\beta)/2}\qquad(\gamma>\beta).
$$

But the [bufferless queue output](../../../../../../bufferless-queue-output.md) is always at most $u_L$. Therefore the downstream [queue overflow](../../../../../../queue-overflow.md) probability is eventually exactly zero, and

$$
\boxed{\lim_L\frac1{L^\gamma}\log\mathbb P(\mathrm{overflow})=-\infty.}
$$

This is a deterministic cap argument, stronger than merely proving superexponentially small probability.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
