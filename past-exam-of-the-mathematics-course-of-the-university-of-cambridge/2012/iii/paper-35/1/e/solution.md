<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Work in the intended $\kappa\geq8$ regime. On one probability-one event, all positive points have finite swallowing times and the strict ordering from part (d) holds for all pairs. Finiteness for arbitrary points follows from finiteness for rational points and monotonicity. Reflection supplies the negative-axis version on the same event.

Fix $r>0$ and suppose the [Loewner trace](../../../../../../trace-of-a-loewner-chain.md) has not visited $r$ by $T(r)$. Its image up to this finite time is compact, so a small interval $I$ about $r$, together with a thin upper collar, is disjoint from the whole trace segment. Every point of that collar belongs to the same component of the complement at every earlier time. Thus all points in a smaller interval are disconnected from infinity at precisely the same time as $r$: before $T(r)$ none is swallowed, and at $T(r)$ all are. This contradicts strict ordering for two positive points in that interval.

Therefore $r$ is visited by time $T(r)$. It cannot be visited before its swallowing time, so the visit occurs at $T(r)$. The same deterministic argument works for every real $r<0$ by reflection, while $0$ is the starting point. Hence

$$
\boxed{\gamma[0,\infty)\supseteq\mathbb R\quad\text{almost surely},\qquad\kappa\geq8.}
$$

The threshold matters. If part (e) is read as retaining only $\kappa>4$, it is false: for $4<\kappa<8$, part (d) gives positive probability of swallowing a nonempty interval at one time, although a continuous trace can visit at most one of its points at that instant. Interior points of that swallowed boundary interval cannot subsequently be reached in capacity time: a later visit, by continuity, would make the curve stay inside an already filled hull for a time interval, contradicting strictly increasing [half-plane capacity](../../../../../../half-plane-capacity.md). Thus the preceding $\kappa\geq8$ conclusion is the necessary intended qualification.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
