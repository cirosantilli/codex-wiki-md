<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**Yes: [regular languages](../../../../../../regular-language.md) are closed under the [shuffle of formal languages](../../../../../../shuffle-of-formal-languages.md).** The construction must allow letters common to both [alphabets](../../../../../../alphabet.md) to be assigned to either input [word](../../../../../../string.md).

Take complete [deterministic finite automata](../../../../../../deterministic-finite-automaton.md) $\mathcal A_i=(Q_i,\Sigma_i,\delta_i,s_i,F_i)$ recognizing $L_i$. Construct a [nondeterministic finite automaton](../../../../../../nondeterministic-finite-automaton.md) on $Q_1\times Q_2$ over $\Sigma=\Sigma_1\cup\Sigma_2$. Its initial state is $(s_1,s_2)$ and its accepting states form $F_1\times F_2$. On a letter $a$, its possible moves from $(p,q)$ are

$$
\begin{aligned}
(p,q)&\longrightarrow(\delta_1(p,a),q)&&\text{if }a\in\Sigma_1,\\
(p,q)&\longrightarrow(p,\delta_2(q,a))&&\text{if }a\in\Sigma_2.
\end{aligned}
$$

Both moves are allowed when $a$ belongs to both [alphabets](../../../../../../alphabet.md). They may coincide; that causes no difficulty.

For every run, record whether each move updated the first or the second coordinate. The letters assigned to each coordinate, in their original order, form two [words](../../../../../../string.md) $u_1,u_2$. The final coordinate states are exactly the states reached by reading $u_i$ in $\mathcal A_i$. Thus an accepting run expresses the input as an interleaving of a [word](../../../../../../string.md) of $L_1$ and a [word](../../../../../../string.md) of $L_2$.

Conversely, given such an interleaving, assign each input position to the [word](../../../../../../string.md) from which it came. The corresponding choices of transitions form a run ending in $F_1\times F_2$. This proves equality between the recognized [formal language](../../../../../../formal-language.md) and the [shuffle of formal languages](../../../../../../shuffle-of-formal-languages.md), in both directions. No assumption of disjoint [alphabets](../../../../../../alphabet.md) is needed. If one contributing [word](../../../../../../string.md) is the [empty word](../../../../../../empty-word.md), no move need update that coordinate; the initial pair is accepting exactly when both [empty words](../../../../../../empty-word.md) are accepted.

Apply the [powerset construction](../../../../../../powerset-construction.md) to this [nondeterministic finite automaton](../../../../../../nondeterministic-finite-automaton.md) to obtain a [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md). In particular,

$$
\boxed{L_1\oplus L_2\text{ is regular},\qquad \text{a recognizing DFA has at most }2^{|Q_1||Q_2|}\text{ states}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
