<h1 id="26i/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

After closing, the count can only decrease. Thus $V(t)>v$ is the event that at least one mosquito remains at $t+v$. The zero probability of a Poisson count yields the [clearance time after closing an infinite-server queue](../../../../../../clearance-time-after-closing-an-infinite-server-queue.md):

$$
\boxed{\mathbb P(V(t)>v)
=1-\exp\left[-\lambda\int_v^{t+v}\mathbb P(S>s)\,ds\right],\qquad v\geq0.}
$$

The clearance time has an atom at zero of mass $e^{-m_t}$, corresponding to an empty room when the window closes.

## ↑ Ancestors (11)

1. [E](../e.md)
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
