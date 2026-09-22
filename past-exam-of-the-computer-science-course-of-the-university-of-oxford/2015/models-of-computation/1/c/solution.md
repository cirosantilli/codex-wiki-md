<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $A=(Q,\{0,1\},\delta,q_0,F)$ be a [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) recognizing $L$. Construct a [nondeterministic finite automaton](../../../../../nondeterministic-finite-automaton.md) $B$ with [automaton state](../../../../../automaton-state.md) [set](../../../../../set-split.md) $Q\times\{0,1\}$. Its second coordinate records whether the extra zero has already been consumed. Start at $(q_0,0)$ and make exactly the [automaton states](../../../../../automaton-state.md) in $F\times\{1\}$ accepting.

For each $q\in Q$, $i\in\{0,1\}$, and $a\in\{0,1\}$, include the ordinary [automaton transition](../../../../../automaton-transition.md)

$$
(q,i)\xrightarrow{a}(\delta(q,a),i).
$$

Also include the extra [automaton transition](../../../../../automaton-transition.md)

$$
\boxed{(q,0)\xrightarrow{0}(q,1)\qquad(q\in Q).}
$$

This consumes the inserted zero without changing the simulated [automaton state](../../../../../automaton-state.md) of $A$. At a zero in layer zero, both the ordinary and extra choices are available. There are no [automaton transitions](../../../../../automaton-transition.md) from layer one back to layer zero.

If $xy\in L$, run $A$ on $x$ in layer zero, consume the extra zero by the displayed [automaton transition](../../../../../automaton-transition.md), and run $A$ on $y$ in layer one. The resulting run accepts $x0y$ in $B$.

Conversely, every accepting run of $B$ starts in layer zero and finishes in layer one, so it uses exactly one extra [automaton transition](../../../../../automaton-transition.md). Split its input as $x0y$ at that move. Removing that consumed zero leaves precisely a run of $A$ on $xy$, ending in $F$. Hence $xy\in L$. The construction also permits an insertion at either end, including insertion into the [empty word](../../../../../empty-word.md).

Therefore $L(B)=L'$. Since $B$ has $2|Q|$ [automaton states](../../../../../automaton-state.md), **$L'$ is a [regular language](../../../../../regular-language.md)**. This is a [single-symbol insertion into a regular language](../../../../../single-symbol-insertion-into-a-regular-language.md).

$$
\boxed{L'=L(B)\text{ is regular}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
