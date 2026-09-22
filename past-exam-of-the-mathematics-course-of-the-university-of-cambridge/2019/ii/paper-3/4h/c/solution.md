<h1 id="4h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Introduce nonterminals for the terminals and one for the pair $bb$:

$$
A\to a,
\qquad B\to b,
\qquad C\to c,
\qquad U\to BB.
$$

Because the original start symbol occurs on a right-hand side, take a fresh start symbol $S_0$. After eliminating the [unit production](../../../../../../unit-production.md) $S\to T$, one grammar in [Chomsky normal form](../../../../../../chomsky-normal-form.md) is

$$
\begin{aligned}
S_0&\to SU\mid AS\mid CC,\\
S&\to SU\mid AS\mid CC,\\
U&\to BB,\\
A&\to a,\qquad B\to b,\qquad C\to c.
\end{aligned}
$$

The original grammar generates exactly

$$
\{a^i cc b^{2j}:i,j\geq0\}.
$$

The displayed grammar generates the same set: $AS$ adds an $a$ on the left, $SU$ adds one $bb$ pair on the right, and $CC$ terminates the derivation with $cc$. Since the original grammar does not generate $\epsilon$,

$$
\boxed{\mathcal L(G)=\mathcal L(G_{\rm Chom}).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4H](../../4h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
