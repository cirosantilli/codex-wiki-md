# Three-sample run detector

↑ **Parent:** [Finite-state machine](finite-state-machine.md)

Store the two previous input [bits](bit.md) in $p,q$. At the next [clock edge](clock-edge.md), use $w=a\land p\land q$ and update $(p,q)'=(a,p)$. The output is high exactly when the present input and previous two samples are all high. Replacing each input by its [negation](negation.md) detects a three-sample low run. Both detectors can share the same two history [bits](bit.md), using $a\land p\land q$ and $\neg a\land\neg p\land\neg q$. With initial history zero, the high detector cannot trigger before three actual high samples have occurred.

## ↑ Ancestors (6)

1. [Finite-state machine](finite-state-machine.md)
2. [Formal language theory](formal-language-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Debounced toggle switch](debounced-toggle-switch.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/3/a/solution.md)
