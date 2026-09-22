<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Fix a finite [alphabet](../../../../../alphabet.md) $\Sigma$. A [regular expression](../../../../../regular-expression.md) is built recursively from $\varnothing$, $\varepsilon$, and the letters $a\in\Sigma$, using union, concatenation, and [Kleene star](../../../../../kleene-star.md). Its interpretation is a [formal language](../../../../../formal-language.md): the basic expressions denote $\varnothing$, $\{\varepsilon\}$, and $\{a\}$, while $E+F$, $EF$, and $E^*$ denote $L(E)\cup L(F)$, $\{uv:u\in L(E),v\in L(F)\}$, and all finite concatenations of members of $L(E)$, including the empty concatenation. In particular, $\varnothing$ and $\varepsilon$ are different expressions with different meanings.

**[Kleene theorem](../../../../../kleene-theorem.md) identifies exactly the languages described by [regular expressions](../../../../../regular-expression.md) with those recognized by [finite-state automata](../../../../../finite-state-machine.md).** Start with a [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) ([DFA](../../../../../deterministic-finite-automaton.md)) having states $1,\ldots,s$, initial state $q_0$, accepting set $F$, and transition function $\delta$. Let $R_{ij}^{(k)}$ describe paths from $i$ to $j$ whose internal states lie among $1,\ldots,k$. At stage zero use the union of letters labelling direct transitions from $i$ to $j$, with $\varepsilon$ added if $i=j$; use $\varnothing$ if there are no such possibilities. Define the [finite-state path expressions](../../../../../finite-state-path-expression.md) recursively by

$$
R_{ij}^{(k)}=R_{ij}^{(k-1)}+R_{ik}^{(k-1)}\bigl(R_{kk}^{(k-1)}\bigr)^*R_{kj}^{(k-1)}.
$$

A path either avoids $k$ internally or decomposes at its visits to $k$: an initial piece into $k$, any number of return pieces at $k$, and a final piece out. Each piece has no internal occurrence of $k$. This proves the recursion by induction, including paths with $i=k$ or $j=k$, where empty pieces are permitted. Thus

$$
\boxed{E_M=\sum_{f\in F}R_{q_0f}^{(s)}}
$$

is a [regular expression](../../../../../regular-expression.md) for the [DFA](../../../../../deterministic-finite-automaton.md)'s accepted [formal language](../../../../../formal-language.md). An empty accepting set gives the expression $\varnothing$. This is the path form of [state elimination for finite automata](../../../../../state-elimination-for-finite-automata.md).

A [nondeterministic finite automaton](../../../../../nondeterministic-finite-automaton.md) ([NFA](../../../../../nondeterministic-finite-automaton.md)) replaces a single successor state by a set $\Delta(q,a)$ of possible successors. It accepts $w=a_1\cdots a_m$ if **there exists an accepting run** $q_0,q_1,\ldots,q_m$ with $q_j\in\Delta(q_{j-1},a_j)$ and $q_m\in F$. Rejection means that no accepting run exists, rather than that some run rejects. For an [Epsilon-NFA](../../../../../epsilon-nfa.md), transitions labelled $\varepsilon$ consume no symbol; acceptance means a path whose non-epsilon labels spell $w$. In particular, acceptance of the empty word is tested using the [epsilon closure](../../../../../epsilon-closure.md) of the initial state.

**The same [Kleene theorem](../../../../../kleene-theorem.md) holds for [nondeterministic finite automata](../../../../../nondeterministic-finite-automaton.md).** For an [NFA](../../../../../nondeterministic-finite-automaton.md) without epsilon transitions, the [powerset construction](../../../../../powerset-construction.md) has state set $\mathcal P(Q)$, initial state $\{q_0\}$, transition $S\mapsto\bigcup_{q\in S}\Delta(q,a)$ on letter $a$, and accepting subsets meeting $F$. Induction on word length shows that its state is exactly the set of possible current [NFA](../../../../../nondeterministic-finite-automaton.md) states. For an [Epsilon-NFA](../../../../../epsilon-nfa.md), start from $E(\{q_0\})$, where $E$ is [epsilon closure](../../../../../epsilon-closure.md), and use

$$
S\longmapsto E\left(\bigcup_{q\in S}\Delta(q,a)\right).
$$

This [subset construction with epsilon transitions](../../../../../subset-construction-with-epsilon-transitions.md) preserves the accepted [formal language](../../../../../formal-language.md) and gives a [DFA](../../../../../deterministic-finite-automaton.md) with at most $2^{|Q|}$ states. The already proved direction of [Kleene theorem](../../../../../kleene-theorem.md) therefore gives a [regular expression](../../../../../regular-expression.md) for every [NFA](../../../../../nondeterministic-finite-automaton.md) language.

For the converse, recursively construct an [Epsilon-NFA](../../../../../epsilon-nfa.md) with a designated initial state and final state for a [regular expression](../../../../../regular-expression.md). Use two states with no connecting path for $\varnothing$, one epsilon edge for $\varepsilon$, and one edge labelled $a$ for $a$. Keep component state sets disjoint. Union uses a fresh initial state with epsilon edges into both components, and epsilon edges from their finals to a fresh final. Concatenation joins the first final to the second initial by an epsilon edge. For [Kleene star](../../../../../kleene-star.md), use fresh initial and final states, an epsilon edge directly between them for zero iterations, an edge into the old initial, and epsilon edges from the old final both back to the old initial and out to the new final. Each construction has exactly the intended union, concatenation, or iteration semantics. Induction on the [regular expression](../../../../../regular-expression.md) proves correctness; the [subset construction with epsilon transitions](../../../../../subset-construction-with-epsilon-transitions.md) then gives a [DFA](../../../../../deterministic-finite-automaton.md). This proves both directions of [Kleene theorem](../../../../../kleene-theorem.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
