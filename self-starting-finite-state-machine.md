# Self-starting finite-state machine

↑ **Parent:** [Finite-state machine](finite-state-machine.md)

A hardware [finite-state machine](finite-state-machine.md) whose implemented transitions eventually leave every unused [state encoding](state-encoding.md) and enter the intended valid state set. If recovery must hold for arbitrary inputs, it is not enough that some input sequence can escape: there must be no indefinitely surviving unused-state path under any input sequence. Since the unused-state graph is finite, absence of a [directed cycle](directed-cycle.md) among unused states gives a uniform finite recovery bound. A reset or initialization rule may still be required to give the valid state its intended meaning.

## ↑ Ancestors (6)

1. [Finite-state machine](finite-state-machine.md)
2. [Formal language theory](formal-language-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2018/digital-systems-linear-algebra-introduction-to-formal-proof/1/e/solution.md)
