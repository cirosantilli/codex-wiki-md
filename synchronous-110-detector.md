# Synchronous 110 detector

↑ **Parent:** [Synchronous sequential circuit](synchronous-sequential-circuit.md)

A [synchronous sequential circuit](synchronous-sequential-circuit.md) emitting a one-cycle pulse at the first low sample after at least two consecutive high samples. Three [D flip-flops](d-flip-flop.md) can implement $q_1^+=a$, $q_2^+=q_1\land a$, and $z^+=q_2\land\neg a$, with all updates using the old state. Initializing all state bits to zero excludes a false startup history. The stored output changes only at clock edges. After a detecting low sample, $q_2$ becomes zero, so the next output is zero regardless of the next input. A longer high run still ends with the same three-sample pattern.

## ↑ Ancestors (7)

1. [Synchronous sequential circuit](synchronous-sequential-circuit.md)
2. [Finite-state machine](finite-state-machine.md)
3. [Formal language theory](formal-language-theory.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof-resit/3/e/solution.md)
