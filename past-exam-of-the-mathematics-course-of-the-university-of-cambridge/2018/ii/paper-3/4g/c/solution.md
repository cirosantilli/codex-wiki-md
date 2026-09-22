<h1 id="4g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The original grammar generates

$$
\mathcal L(G)=\{a^n b c^n:n\geq0\},
$$

because each use of $S\to ASc$ adds one $a$ on the left and one $c$ on the right, and $S\to B\to b$ terminates the derivation.

Introduce nonterminals $S_0,X,C$ and use

$$
\begin{aligned}
S_0&\to AX\mid b,\\
S&\to AX\mid b,\\
X&\to SC,\\
A&\to a,\\
C&\to c.
\end{aligned}
$$

Every production is in [Chomsky normal form](../../../../../../chomsky-normal-form.md). The production $X\to SC$ completes one matched $a,c$ pair, while either start-like symbol terminates with $b$, so the grammar generates exactly the same language. **These productions are a valid $G_{\rm Chom}$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4G](../../4g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
