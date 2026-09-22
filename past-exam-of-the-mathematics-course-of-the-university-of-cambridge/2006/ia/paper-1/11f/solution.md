<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

A real [sequence](../../../../../sequence.md) has limit $a\in\mathbb R$ if, for every $\varepsilon>0$, there is $N$ such that $|a_n-a|<\varepsilon$ for all $n\ge N$. It tends to $+\infty$ if, for every real $M$, eventually $a_n>M$; it tends to $-\infty$ if eventually $a_n<M$ for every real $M$.

The [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) states that every [bounded sequence](../../../../../bounded-sequence.md) of real numbers has a real convergent [subsequence](../../../../../subsequence.md). This proves the claim for bounded sequences. If the sequence is unbounded above, every tail remains unbounded above because a finite prefix is bounded. Choose indices $n_j$ increasing with $a_{n_j}>j$. This subsequence tends to $+\infty$. If it is unbounded below, choose $a_{n_j}<-j$ to obtain a subsequence tending to $-\infty$. This proves the [extended real subsequence theorem](../../../../../extended-real-subsequence-theorem.md).

For the final example, a [bounded sequence with vanishing increments need not converge](../../../../../bounded-sequence-with-vanishing-increments-need-not-converge.md). Take

$$
\boxed{a_n=\sin\sqrt n.}
$$

The [mean value theorem](../../../../../mean-value-theorem.md) gives

$$
|a_{n+1}-a_n|\le\sqrt{n+1}-\sqrt n=\frac1{\sqrt{n+1}+\sqrt n}\longrightarrow0.
$$

Nevertheless, along $n_j=\lfloor(\pi/2+2\pi j)^2\rfloor$, the square-root rounding error tends to zero, so $a_{n_j}\to1$. Along $m_j=\lfloor(3\pi/2+2\pi j)^2\rfloor$, it tends to $-1$. These two [subsequences](../../../../../subsequence.md) have different limits, proving nonconvergence.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
