<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $T$ consist of all finite nondecreasing paths

$$
(s_0,s_1,\ldots,s_k),qquad s_0\leq_Ss_1\leq_S\cdots\leq_Ss_k,
$$

ordered by initial-segment extension. The one-point path $(s_0)$ is least, and the predecessors of any path are its initial segments, hence linearly ordered. Force an atom at a path exactly when it is forced at the path's endpoint.

The endpoint map $e:T\to S$ is monotone and has the back property: if $e(t)\leq_Ss$, append $s$ to $t$. Induction on propositions therefore gives

$$
t\Vdash_T\psi\iff e(t)\Vdash_S\psi.
$$

In particular the roots force exactly the same propositions. This is the [unravelling of a Kripke model](../../../../../../unravelling-of-a-kripke-model.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
