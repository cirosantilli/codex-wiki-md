<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The minimal [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) is unique up to an [isomorphism](../../../../../../isomorphism.md) preserving the initial state, transitions and accepting states.** We use complete [deterministic finite automata](../../../../../../deterministic-finite-automaton.md) over the fixed [alphabet](../../../../../../alphabet.md); the PDF's abbreviation FDA has this meaning. State names themselves cannot be unique.

For [words](../../../../../../string.md) $u,v\in\Sigma^*$, introduce the [Myhill-Nerode equivalence](../../../../../../myhill-nerode-equivalence.md)

$$
u\sim_Lv\quad\Longleftrightarrow\quad\forall w\in\Sigma^*\;\bigl(uw\in L\iff vw\in L\bigr).
$$

It is an [equivalence relation](../../../../../../equivalence-relation.md), and appending the same letter to equivalent [words](../../../../../../string.md) preserves it: a suffix $w$ after $ua$ is the suffix $aw$ after $u$. Since $L$ is a [regular language](../../../../../../regular-language.md), take any recognizing [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md). Words reaching the same state are equivalent, since every further suffix gives the same computation. Thus $\sim_L$ has finite index.

The [canonical residual automaton](../../../../../../canonical-residual-automaton.md) has one state $[u]$ for each class, initial state $[\epsilon]$, transition $[u]\xrightarrow{a}[ua]$, and accepting states those with $u\in L$. These choices are well-defined by [Myhill-Nerode equivalence](../../../../../../myhill-nerode-equivalence.md). Induction on the input length shows that reading $u$ reaches $[u]$, so the [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) recognizes $L$, and all its states are [accessible states of a deterministic finite automaton](../../../../../../accessible-state-of-a-deterministic-finite-automaton.md). The same state can be described by the [left quotient of a formal language](../../../../../../left-quotient-of-a-formal-language.md)

$$
u^{-1}L=\{w:uw\in L\}.
$$

Two states are different precisely when some suffix distinguishes their acceptance behavior.

Every recognizing [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) has at least as many states as there are classes: pick a representative from each class; two different representatives cannot reach the same state. The [canonical residual automaton](../../../../../../canonical-residual-automaton.md) attains this bound, and therefore is a [minimal deterministic finite automaton](../../../../../../minimal-deterministic-finite-automaton.md).

For uniqueness, let $\mathcal A$ be any [minimal deterministic finite automaton](../../../../../../minimal-deterministic-finite-automaton.md). All its states are accessible, since removing inaccessible states leaves a complete recognizing [deterministic finite automaton](../../../../../../deterministic-finite-automaton.md) with fewer states. Map a state reached by $u$ to $[u]$. This is well-defined because two [words](../../../../../../string.md) reaching the same state are equivalent. It is surjective because every class has a representative. Both sets have the minimal number of states, so it is a [bijection](../../../../../../bijection.md). It preserves the initial state and transitions by construction, and preserves accepting states by taking the [empty word](../../../../../../empty-word.md) as the suffix. This is the required [isomorphism](../../../../../../isomorphism.md) with the [canonical residual automaton](../../../../../../canonical-residual-automaton.md), proving

$$
\boxed{\text{minimal number of states}=|\Sigma^*/{\sim_L}|,\quad\text{uniqueness up to isomorphism}.}
$$

The [empty word](../../../../../../empty-word.md) is included throughout, and empty or universal [regular languages](../../../../../../regular-language.md) have the corresponding one-state complete [deterministic finite automata](../../../../../../deterministic-finite-automaton.md).

## ↑ Ancestors (11)

1. [I](../i.md)
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
