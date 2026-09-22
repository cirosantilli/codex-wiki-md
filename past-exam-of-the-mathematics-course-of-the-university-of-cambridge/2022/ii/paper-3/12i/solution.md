<h1 id="12i/solution">Solution</h1>

↑ **Parent:** [12I](../12i.md)

A state $q$ is [accessible](../../../../../accessible-state-of-a-deterministic-finite-automaton.md) when

$$
\widehat\delta(q_0,w)=q
$$

for some word $w\in\Sigma^*$. States $p$ and $q$ are equivalent, or [indistinguishable](../../../../../indistinguishable-states-of-a-deterministic-finite-automaton.md), when

$$
\widehat\delta(p,w)\in F
\quad\Longleftrightarrow\quad
\widehat\delta(q,w)\in F
$$

for every continuation $w$.

This equivalence is preserved by transitions: if $p\sim q$, then $\delta(p,a)\sim\delta(q,a)$. Hence define $D/{\sim}$ with states $[q]$, initial state $[q_0]$, transition

$$
\overline\delta([q],a)=[\delta(q,a)],
$$

and accepting classes $[q]$ with $q\in F$. Induction on word length gives

$$
\widehat{\overline\delta}([q_0],w)
=[\widehat\delta(q_0,w)],
$$

so $D$ and its [quotient deterministic finite automaton by indistinguishable states](../../../../../quotient-deterministic-finite-automaton-by-indistinguishable-states.md) accept the same language. If two quotient states were equivalent, their representatives would be equivalent in $D$, so the classes would be equal. Thus no two distinct quotient states are equivalent.

For the unary alphabet, accessibility means that all states occur on the orbit

$$
q_0,\ q_1=\delta(q_0,1),\ q_2,\ldots.
$$

Finiteness makes this orbit a directed tail entering a directed cycle. The quotient retains exactly one accepting state and merges precisely those positions having the same future acceptance pattern.

More explicitly, if the unique accepting state lies before the cycle, every state after it can never reach acceptance and these states collapse to one rejecting sink. The minimal diagram is then a directed chain from the initial state through the unique accepting state and onward to that sink, which has a self-loop.

If the accepting state lies on the cycle, all cycle states are distinct because their next visits to the accepting state occur in different residue classes modulo the cycle length. Any remaining tail is a chain feeding the cycle. In a minimal diagram with a nonempty tail, the accepting state is the cycle vertex immediately preceding the entry vertex; otherwise the final tail state has the same future acceptance sequence as a cycle state and would be merged. A pure cycle with one accepting vertex is also possible. These are exactly the minimal [accessible unary DFAs](../../../../../accessible-unary-deterministic-finite-automaton.md) with one accepting state.

## ↑ Ancestors (10)

1. [12I](../12i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
