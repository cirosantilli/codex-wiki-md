<h1 id="4h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $K$ be the [diagonal halting set](../../../../../../diagonal-halting-set.md), which is [undecidable](../../../../../../undecidable-decision-problem.md). The pumping argument below actually holds for every subset $K\subseteq\mathbb N$; nonregularity needs the stated convention, or at least a set of exponents whose unary language is nonregular.

The [pumping lemma for regular languages](../../../../../../pumping-lemma-for-regular-languages.md) holds with [pumping length](../../../../../../pumping-length.md) one. For an accepted nonempty word, pump its first symbol. A word containing only $1$s remains in $1^*$ even if that symbol is deleted. If there is a zero and a nonempty prefix before its last zero, pumping the first symbol leaves the last zero and its following $n\in K$ ones unchanged. If the word is $01^n$, pumping its initial zero produces $0^i1^n$; this is accepted for $i\geq1$, and for $i=0$ it belongs to $1^*$. In every case the pumped substring is nonempty and lies in the first position.

If $L$ were a [regular language](../../../../../../regular-language.md), closure under intersection would make

$$
L\cap01^*=\{01^n:n\in K\}
$$

regular. A [finite-state automaton](../../../../../../finite-state-machine.md) for this intersection would decide membership of $n$ in the [diagonal halting set](../../../../../../diagonal-halting-set.md) by reading $01^n$, a contradiction. Thus **$L$ satisfies the pumping lemma but is not regular**, under the usual meaning of $\mathbb K$. If $K$ were arbitrary, the printed conclusion would be false, for example for $K=\mathbb N$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4H](../../4h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
