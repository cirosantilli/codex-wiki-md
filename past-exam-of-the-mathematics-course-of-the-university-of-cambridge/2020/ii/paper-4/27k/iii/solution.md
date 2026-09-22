<h1 id="27k/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Poisson output theorem for a feedback queue](../../../../../../poisson-output-theorem-for-a-feedback-queue.md), equivalently the [Burke theorem](../../../../../../burke-s-theorem.md) applied to the effective queue-length process with service rate $\delta\mu$, shows that successful departures in equilibrium form a [Poisson process](../../../../../../poisson-process.md) of rate $\lambda$.

The process of all entries into the queue is different. Its long-run rate is

$$
\lambda+(1-\delta)\mu\,\mathbb P(Q>0)
=\lambda+(1-\delta)\mu\frac{\lambda}{\delta\mu}
=\frac\lambda\delta.
$$

Immediately after any queue-entry event the server is busy, so the conditional probability of another entry in the next interval of length $h$ is

$$
[\lambda+(1-\delta)\mu]h+o(h):
$$

the next entry can be external or can be a service completion followed by feedback. A Poisson process of the displayed long-run rate would instead give $(\lambda/\delta)h+o(h)$. These coefficients are unequal when $\lambda<\delta\mu$, since

$$
\lambda+(1-\delta)\mu-\frac\lambda\delta
=(1-\delta)\left(\mu-\frac\lambda\delta\right)>0.
$$

**Hence the combined arrival process is not Poissonian.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [27K](../../27k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
