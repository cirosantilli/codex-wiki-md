<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $A\in\mathcal F_n$, define the bounded [stopping time](../../../../../../../stopping-time.md) $T=n+1$ on $A$ and $T=n$ on $A^c$. Before time $n$ its stopping events are empty, at time $n$ the event $\{T\leq n\}=A^c$ belongs to $\mathcal F_n$, and subsequently it has stopped everywhere. Subtract the assumed mean identity for this $T$ from that for the constant [stopping time](../../../../../../../stopping-time.md) $n$ to obtain

$$
\mathbb E\bigl[\mathbf1_A(M_{n+1}-M_n)\bigr]=0\qquad(A\in\mathcal F_n).
$$

Since $M_n$ is integrable and $\mathcal F_n$-[measurable](../../../../../../../measurability.md), this is precisely the defining property of [conditional expectation](../../../../../../../conditional-expectation.md) giving **$\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$**. Thus the [adapted process](../../../../../../../adapted-process.md) is a [martingale](../../../../../../../martingale-split.md), completing the [bounded-stopping-time characterization of a martingale](../../../../../../../bounded-stopping-time-characterization-of-a-martingale.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 34](../../../../paper-34-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
