<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply [Hadamard gates](../../../../../../../hadamard-gate.md) to $|0^m\rangle$ to prepare

$$
2^{-m/2}\sum_{x=0}^{2^m-1}|x\rangle.
$$

Reversibly compute the efficiently decidable predicate $[x<Q]$ into an ancillary qubit and measure it. The success probability is $Q/2^m>1/2$, and conditioned on success the first register is exactly

$$
|\xi\rangle=\frac1{\sqrt Q}\sum_{b=0}^{Q-1}|b\rangle.
$$

Restart after a failed measurement. After $L=\lceil\log_2(1/\delta)\rceil$ attempts, the probability that all attempts fail is below $\delta$, so the state is prepared with probability at least $1-\delta$ using a number of gates polynomial in $m$ and $\log(1/\delta)$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
