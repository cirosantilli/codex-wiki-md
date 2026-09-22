<h1 id="5/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [two-list functional queue](../../../../../../../two-list-functional-queue.md) has constant-time `peek` and `isEmpty`, but an individual insertion or removal can cost linear time when it reverses a rear list of length $k$. Its useful guarantee is **constant amortized time per operation along a single history starting from empty**.

For the [amortized analysis](../../../../../../../amortized-analysis.md), each item is consed into the rear once, transferred into the front at most once, and removed at most once. Charge its future reversal to the earlier insertion. Thus $m$ operations perform only $O(m)$ total list-cell work. More formally, use potential $\Phi=C\lvert\texttt{rear}\rvert$, with $C$ sufficient to pay the per-cell reversal cost. An insertion into a nonempty front increases $\Phi$ by $C$ and has constant actual cost; a reversal of $k$ cells decreases $\Phi$ by $Ck$, paying its actual cost. With $\Phi_0=0$ and $\Phi_m\geq0$,

$$
\sum_{i=1}^m c_i=\sum_{i=1}^m\bigl(c_i+\Phi_i-\Phi_{i-1}\bigr)-\Phi_m=O(m).
$$

This [amortized analysis](../../../../../../../amortized-analysis.md) is deterministic, not an average over a random workload. It assumes subsequent operations use the successive returned versions. If a persistent old version with a long rear is reused repeatedly, each independent dequeue can redo the same reversal. The simple potential accounting does not give constant amortized cost across such a branching history without further [memoization](../../../../../../../memoization.md) or a stronger persistent [FIFO queue](../../../../../../../fifo-queue.md) implementation.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Ia](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
