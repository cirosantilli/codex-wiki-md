<h1 id="4h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let a [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) recognizing the [regular language](../../../../../../regular-language.md) have states $Q$, start state $q_0$, accepting states $F$, and transition [function](../../../../../../function-split.md) $\delta$. Construct a [context-free grammar](../../../../../../context-free-grammar.md) with one nonterminal $A_q$ for every state, start symbol $A_{q_0}$, and productions

$$
A_q\to aA_{\delta(q,a)}\quad(q\in Q,\ a\in\Sigma),
\qquad A_q\to\varepsilon\quad(q\in F).
$$

Induction on the length of a word shows that $A_q$ derives $wA_r$ exactly when the automaton reaches $r$ from $q$ after reading $w$. The terminal production can then end the derivation precisely at an accepting state. Thus the grammar generates exactly the recognized language, proving **every [regular language](../../../../../../regular-language.md) is a [context-free language](../../../../../../context-free-language.md)**. This is actually a [right-linear grammar](../../../../../../right-linear-grammar.md), a special case of a [context-free grammar](../../../../../../context-free-grammar.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4H](../../4h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
