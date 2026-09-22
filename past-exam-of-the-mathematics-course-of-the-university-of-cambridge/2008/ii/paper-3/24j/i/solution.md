<h1 id="24j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Convergence in probability](../../../../../../convergence-in-probability.md) means $\mathbb P(|X_n-X|>\epsilon)\to0$ for every $\epsilon>0$. [Convergence in distribution](../../../../../../convergence-in-distribution.md) means $F_{X_n}(t)\to F_X(t)$ at every continuity point $t$ of $F_X$. The inclusions obtained by separating the event $|X_n-X|>\epsilon$ give

$$
F_X(t-\epsilon)-\mathbb P(|X_n-X|>\epsilon)\leq F_{X_n}(t)\leq F_X(t+\epsilon)+\mathbb P(|X_n-X|>\epsilon).
$$

Take lower and upper limits as $n\to\infty$, then $\epsilon\downarrow0$ at a continuity point. Both bounds tend to $F_X(t)$, proving that **convergence in probability implies convergence in distribution**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [24J](../../24j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
