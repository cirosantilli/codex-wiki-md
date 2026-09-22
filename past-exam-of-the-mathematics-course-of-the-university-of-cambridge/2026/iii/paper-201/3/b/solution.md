<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume $\sup_n\mathbb E|M_n|<\infty$. For every pair of [rationals](../../../../../../rational-number.md) $a<b$, [Doob upcrossing inequality](../../../../../../doob-upcrossing-inequality.md) gives

$$
(b-a)\mathbb E U_\infty[a,b]
\leq\sup_n\mathbb E(M_n-a)^-<\infty
$$

by [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md). Thus every rational interval is upcrossed only finitely often almost surely. If a real sequence has distinct [limit inferior](../../../../../../limit-inferior.md) and [limit superior](../../../../../../limit-superior.md), it completes infinitely many upcrossings of some rational interval between them. Hence $M_n$ converges in the [extended real line](../../../../../../extended-real-number-line.md) almost surely.

[Fatou lemma](../../../../../../fatou-s-lemma.md) gives

$$
\mathbb E\!\left[\liminf_n|M_n|\right]
\leq\liminf_n\mathbb E|M_n|<\infty,
$$

so the limit is finite almost surely and integrable. This is the $L^1$-bounded form of the [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
