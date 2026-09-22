<h1 id="26i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An arrival at time $u\in[0,t]$ is still present at $t$ exactly when its [independent](../../../../../../independent-random-variables.md) service time exceeds $t-u$. Thinning the marked [Poisson process](../../../../../../poisson-process.md) with this retention probability gives a Poisson count with parameter

$$
m_t=\lambda\int_0^t\mathbb P(S>t-u)\,du
=\lambda\int_0^t\mathbb P(S>v)\,dv.
$$

Thus

$$
\boxed{Q(t)\sim\operatorname{Poisson}(m_t).}
$$

This reasoning allows atoms in the service-time distribution; the strict survival inequality correctly treats a customer whose service has ended.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26I](../../26i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
