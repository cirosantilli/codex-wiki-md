# Volatile-qualified objects in C

↑ **Parent:** [C programming language](c-programming-language.md)

[Volatile-qualified objects in C](volatile-qualified-objects-in-c.md) are objects whose accesses must follow the implementation's observable-access rules even when the optimizer cannot see an ordinary program dependency. They are commonly used for device registers and state changed by an [interrupt handler](interrupt-handler.md), under the target compiler's embedded execution model. `volatile` does not by itself provide atomic multiword access, [mutual exclusion](mutual-exclusion.md) or inter-thread synchronization. Protecting a shared snapshot still requires a suitable [critical section](critical-section.md) or another synchronization protocol.[Sections 5.1.2.3 and 6.7.3, especially the implementation-defined meaning of volatile access](c11-committee-draft-n1570.md)

## ↑ Ancestors (4)

1. [C programming language](c-programming-language.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Interrupt-driven pulse sequencer](interrupt-driven-pulse-sequencer.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof-resit/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/2/b/solution.md)
- [Volatile-qualified objects in C](volatile-qualified-objects-in-c.md)
