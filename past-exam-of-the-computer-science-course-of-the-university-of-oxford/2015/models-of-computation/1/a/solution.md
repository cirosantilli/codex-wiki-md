<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [nondeterministic finite automaton](../../../../../nondeterministic-finite-automaton.md), allowing the [epsilon transitions](../../../../../epsilon-transition.md) used in this paper, is a [tuple](../../../../../finite-tuple.md)

$$
M=(Q,\Sigma,\delta,q_0,F),\qquad
\delta:Q\times(\Sigma\cup\{\varepsilon\})\longrightarrow\mathcal P(Q).
$$

Here $Q$ is a nonempty [finite set](../../../../../finite-set.md) of [automaton states](../../../../../automaton-state.md), $\Sigma$ is a finite [alphabet](../../../../../alphabet.md), $\mathcal P(Q)$ is the [power set](../../../../../power-set.md) of $Q$, $q_0\in Q$ is the initial [automaton state](../../../../../automaton-state.md), and $F\subseteq Q$ is the [set](../../../../../set-split.md) of accepting [automaton states](../../../../../automaton-state.md). The symbol $\varepsilon\notin\Sigma$ denotes the [empty word](../../../../../empty-word.md). Membership $r\in\delta(q,a)$ permits an [automaton transition](../../../../../automaton-transition.md) from $q$ to $r$ consuming $a$ when $a\in\Sigma$, or consuming nothing when $a=\varepsilon$.

The recognized [formal language](../../../../../formal-language.md) is

$$
\boxed{L(M)=\{w\in\Sigma^*: \text{some finite path from }q_0\text{ to a state in }F\text{ has label }w\}.}
$$

The label of a [graph path](../../../../../path-in-a-graph.md) is the [concatenation](../../../../../concatenation.md) of its labels with all occurrences of $\varepsilon$ omitted. Thus acceptance requires consuming the entire input [word](../../../../../string.md); a single successful choice of [automaton transitions](../../../../../automaton-transition.md) suffices. A path of length zero is allowed, so the [empty word](../../../../../empty-word.md) is accepted whenever $q_0\in F$, or an accepting [automaton state](../../../../../automaton-state.md) is reachable by [epsilon transitions](../../../../../epsilon-transition.md). If [epsilon transitions](../../../../../epsilon-transition.md) are excluded from the definition of a [nondeterministic finite automaton](../../../../../nondeterministic-finite-automaton.md), the displayed version is called an [Epsilon-NFA](../../../../../epsilon-nfa.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Models of computation](../../../models-of-computation-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
