<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $A\in\mathcal F$ and consider the traces

$$
\mathcal T=\{A\cap B:B\in\mathcal F\setminus\{A\}\}\subseteq\mathcal P(A).
$$

For distinct $B,C\in\mathcal F\setminus\{A\}$, the hypothesis applied in both orders says

$$
A\cap B\not\subseteq C,
\qquad
A\cap C\not\subseteq B.
$$

Equivalently, neither trace contains the other. Thus the traces are distinct and form an [antichain](../../../../../../antichain.md) in the Boolean lattice on the $2r$ points of $A$. By [Sperner theorem](../../../../../../sperner-s-theorem.md),

$$
|\mathcal F|-1=|\mathcal T|\leq\binom{2r}{r},
$$

which is the required bound.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
