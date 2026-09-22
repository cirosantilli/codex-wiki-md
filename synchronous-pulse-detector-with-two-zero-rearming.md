# Synchronous pulse detector with two-zero rearming

↑ **Parent:** [Synchronous sequential circuit](synchronous-sequential-circuit.md)

The displayed two-register [Moore machine](moore-machine.md), initialized to $q_1q_0=00$, generates a one-clock pulse on a sampled high when ready, then waits for two consecutive sampled zeros before it can generate another. The codes $00,10,11,01$ represent ready, pulse, disabled and one-zero-seen respectively. From ready a high enters pulse; from pulse the next edge leaves for disabled on a high or one-zero-seen on a low. Disabled enters one-zero-seen on a low. A second consecutive low returns to ready, whereas a high returns to disabled. This transition analysis proves the output rule, the one-period duration and the immediate first-edge response after reset. It assumes a synchronous input meeting setup and hold requirements.

## ↑ Ancestors (7)

1. [Synchronous sequential circuit](synchronous-sequential-circuit.md)
2. [Finite-state machine](finite-state-machine.md)
3. [Formal language theory](formal-language-theory.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/3/d/solution.md)
