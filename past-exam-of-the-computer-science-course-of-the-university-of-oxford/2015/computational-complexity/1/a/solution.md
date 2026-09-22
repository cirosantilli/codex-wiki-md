<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Exactly the [regular languages](../../../../../regular-language.md).** A [read-only-from-left Turing acceptor](../../../../../read-only-from-left-turing-acceptor.md) has only its current control state as usable memory: it never changes a tape symbol, and its head never returns to an earlier cell. This is the behaviour of a [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) while it reads the [input](../../../../../input-computer-science.md).

To make the correspondence precise, retain the control states and the transitions on the [input](../../../../../input-computer-science.md) [alphabet](../../../../../alphabet.md). Replace accepting and rejecting halts by absorbing states, so that halting before the end of a [word over an alphabet](../../../../../string.md) has the same effect on every continuation. For each remaining state $q$, follow the transitions on blank symbols and mark $q$ accepting in the [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) exactly when this blank-only continuation eventually accepts. This marking is a finite calculation: either a halting state is reached or a state repeats, after which the blank-only run loops. The resulting [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) accepts exactly the same [formal language](../../../../../formal-language.md) as the [read-only-from-left Turing acceptor](../../../../../read-only-from-left-turing-acceptor.md). If the latter is a decider, the blank-only run from every reachable end-of-input state halts.

Conversely, simulate any [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) by a [read-only-from-left Turing acceptor](../../../../../read-only-from-left-turing-acceptor.md), using its state transitions while reading the [input](../../../../../input-computer-science.md). At the first blank symbol, halt and accept or reject according to the current [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) state. This machine halts on every [input](../../../../../input-computer-science.md) and decides the required [regular language](../../../../../regular-language.md).

$$
\boxed{\text{ROFL-decidable languages}=\text{regular languages}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
