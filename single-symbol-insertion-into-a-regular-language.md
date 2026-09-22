# Single-symbol insertion into a regular language

↑ **Parent:** [Regular language](regular-language.md)

For a fixed symbol $a$ and a [regular language](regular-language.md) $L$, inserting exactly one $a$ at an arbitrary position preserves regularity. Make two copies of a recognizing [finite-state automaton](finite-state-machine.md), one before and one after the insertion. Preserve its ordinary [automaton transitions](automaton-transition.md) in each copy, and add a transition consuming $a$ from each before-state to its matching after-state. Accept only in the after-copy. Every accepting run makes exactly one of the additional moves.

## ↑ Ancestors (6)

1. [Regular language](regular-language.md)
2. [Formal language theory](formal-language-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/models-of-computation/1/c/solution.md)
