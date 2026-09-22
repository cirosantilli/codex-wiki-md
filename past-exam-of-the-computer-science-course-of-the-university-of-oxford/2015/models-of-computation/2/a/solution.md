<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [nondeterministic pushdown automaton](../../../../../pushdown-automaton.md) is a [tuple](../../../../../finite-tuple.md)

$$
M=(Q,\Sigma,\Gamma,\delta,q_0,Z_0,F),\qquad
\delta:Q\times(\Sigma\cup\{\varepsilon\})\times\Gamma
\longrightarrow\mathcal P_{\mathrm{fin}}(Q\times\Gamma^*).
$$

Here $Q$ is a nonempty [finite set](../../../../../finite-set.md) of control states, $\Sigma$ a finite input [alphabet](../../../../../alphabet.md), $\Gamma$ a finite [stack alphabet](../../../../../stack-alphabet.md), $q_0\in Q$ the initial control state, $Z_0\in\Gamma$ the initial [stack](../../../../../stack-data-structure.md) symbol, and $F\subseteq Q$ the final control states. The notation $\mathcal P_{\mathrm{fin}}$ requires each transition to have only finitely many choices. Since the domain is finite, the whole transition specification is finite.

A [pushdown automaton configuration](../../../../../pushdown-automaton-configuration.md) is $(q,w,\alpha)\in Q\times\Sigma^*\times\Gamma^*$, recording the control state, unread input [word](../../../../../string.md), and [stack](../../../../../stack-data-structure.md) contents. Write the top of the [stack](../../../../../stack-data-structure.md) on the left. For $a\in\Sigma$, the one-step relation is

$$
(q,aw,X\beta)\vdash_M(r,w,\gamma\beta)
\quad\text{if }(r,\gamma)\in\delta(q,a,X).
$$

An [epsilon transition](../../../../../epsilon-transition.md) instead has

$$
(q,w,X\beta)\vdash_M(r,w,\gamma\beta)
\quad\text{if }(r,\gamma)\in\delta(q,\varepsilon,X).
$$

Thus a move replaces the top [stack](../../../../../stack-data-structure.md) symbol $X$ by the [word](../../../../../string.md) $\gamma$, whose leftmost symbol becomes the new top. It consumes one input symbol or no input symbol. Under this convention there is no move from an empty [stack](../../../../../stack-data-structure.md).

For [acceptance by final state](../../../../../acceptance-by-final-state.md), the recognized [formal language](../../../../../formal-language.md) is

$$
\boxed{L(M)=\{w\in\Sigma^*: (q_0,w,Z_0)\vdash_M^*(f,\varepsilon,\alpha)
\text{ for some }f\in F,\ \alpha\in\Gamma^*\}.}
$$

Here $\vdash_M^*$ allows any finite number of moves, including zero. The entire input must have been consumed; the final [stack](../../../../../stack-data-structure.md) need not be empty. Acceptance requires at least one such run of the [nondeterministic pushdown automaton](../../../../../pushdown-automaton.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Models of computation](../../../models-of-computation-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
