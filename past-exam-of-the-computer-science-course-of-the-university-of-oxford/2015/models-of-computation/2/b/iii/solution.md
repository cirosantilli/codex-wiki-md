<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the standard [conversion of a context-free grammar to a pushdown automaton](../../../../../../conversion-of-a-context-free-grammar-to-a-pushdown-automaton.md), implementing a [leftmost derivation](../../../../../../leftmost-derivation.md) on a [stack](../../../../../../stack-data-structure.md). Take control states $q_s,q,q_f$, input [alphabet](../../../../../../alphabet.md) $\{a,b\}$, [stack alphabet](../../../../../../stack-alphabet.md) $\{S,T,U,a,b,\bot\}$, initial control state $q_s$, initial [stack](../../../../../../stack-data-structure.md) symbol $\bot$, and sole final control state $q_f$. The symbol $\bot$ is a fresh [stack bottom marker](../../../../../../stack-bottom-marker.md). As in part (a), the top of the [stack](../../../../../../stack-data-structure.md) is written on the left.

Initialize with

$$
\delta(q_s,\varepsilon,\bot)=\{(q,S\bot)\}.
$$

In control state $q$, replace a top [nonterminal symbol](../../../../../../nonterminal-symbol.md) by one of its [production rule](../../../../../../production-rule.md) right-hand sides:

$$
\begin{aligned}
\delta(q,\varepsilon,S)&=\{(q,UST),(q,ST),(q,\varepsilon)\},\\
\delta(q,\varepsilon,U)&=\{(q,a),(q,aT)\},\\
\delta(q,\varepsilon,T)&=\{(q,b)\}.
\end{aligned}
$$

The replacements are written in the order in which they are to be processed. For example, replacing $S$ by $UST$ leaves $U$ on top; an implementation using individual push operations pushes $T$, then $S$, then $U$.

Match and pop top [terminal symbols](../../../../../../terminal-symbol.md) by

$$
\delta(q,a,a)=\{(q,\varepsilon)\},\qquad
\delta(q,b,b)=\{(q,\varepsilon)\}.
$$

Finally include

$$
\delta(q,\varepsilon,\bot)=\{(q_f,\bot)\}.
$$

All unlisted transitions have no choices; $q_f$ has no outgoing transitions. This is [acceptance by final state](../../../../../../acceptance-by-final-state.md), leaving the bottom marker on the [stack](../../../../../../stack-data-structure.md). Taking the last transition too early cannot cause false acceptance, because an unread input suffix remains and $q_f$ cannot consume it.

For correctness, after initialization the [stack](../../../../../../stack-data-structure.md) contains the unprocessed part of a sentential form. Expanding a top [nonterminal symbol](../../../../../../nonterminal-symbol.md) simulates one step of a [leftmost derivation](../../../../../../leftmost-derivation.md), and popping a matching [terminal symbol](../../../../../../terminal-symbol.md) transfers it to the already-read input prefix. Thus if the input prefix consumed so far is $u$ and the [stack](../../../../../../stack-data-structure.md) above $\bot$ is $\alpha$, then $S\Rightarrow_G^*u\alpha$. Acceptance gives $S\Rightarrow_G^*w$ for the entire input $w$.

Conversely, any [leftmost derivation](../../../../../../leftmost-derivation.md) of $w$ specifies choices of these transitions: expand the next [nonterminal symbol](../../../../../../nonterminal-symbol.md), and read each resulting leading [terminal symbol](../../../../../../terminal-symbol.md) when it reaches the top. After all symbols of $w$ are consumed, only $\bot$ remains, enabling the move to $q_f$. **The [nondeterministic pushdown automaton](../../../../../../pushdown-automaton.md) therefore recognizes exactly $L(G)$.** The [empty word](../../../../../../empty-word.md) is accepted by choosing $S\to\varepsilon$ after initialization.

$$
\boxed{L(M)=L(G),\qquad F=\{q_f\}.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Models of computation](../../../../models-of-computation-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
