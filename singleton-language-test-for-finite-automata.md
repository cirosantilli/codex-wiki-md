# Singleton-language test for finite automata

↑ **Parent:** [Finite-state machine](finite-state-machine.md)

To decide whether a [finite-state automaton](finite-state-machine.md) accepts exactly one distinct [word](string.md), first obtain some accepted [word](string.md) $w$ by a [finite automaton emptiness test](finite-automaton-emptiness-test.md). If there is none, answer no. Otherwise construct a [finite-state automaton](finite-state-machine.md) for the accepted [formal language](formal-language.md) minus the [singleton](singleton-mathematics.md) $\{w\}$ and test it for emptiness. Answer yes exactly when that difference is empty. [Subset construction](subset-construction-with-epsilon-transitions.md) handles multiple accepting runs without confusing runs with distinct [words](string.md).

## ↑ Ancestors (6)

1. [Finite-state machine](finite-state-machine.md)
2. [Formal language theory](formal-language-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/models-of-computation/3/d/i/solution.md)
