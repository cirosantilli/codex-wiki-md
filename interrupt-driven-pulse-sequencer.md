# Interrupt-driven pulse sequencer

↑ **Parent:** [Finite-state machine](finite-state-machine.md)

A pulse sequencer can separate event capture from output timing. A short [interrupt handler](interrupt-handler.md) acknowledges the [event latch](single-bit-event-latch.md) and increments a pending count. An independent [finite-state machine](finite-state-machine.md) consumes one count on entering `ON`, changes to `GAP` after the pulse width, and enters `IDLE` only after the mandatory off interval. Even an empty queue must not bypass `GAP`: an arrival immediately after light-off would otherwise start too soon.

The pending count equals recorded events minus started pulses. A [critical section](critical-section.md) protects its read-modify-write operations; declaring shared state as in [volatile-qualified objects in C](volatile-qualified-objects-in-c.md) does not alone make each update an [atomic operation](atomic-operation.md). Separate sequencers for different channels allow simultaneous pulses while one [hardware timer](hardware-timer.md) schedules their earliest deadline. Finite queue capacity, detector rearming and dispatch resolution remain explicit assumptions.

## ↑ Ancestors (6)

1. [Finite-state machine](finite-state-machine.md)
2. [Formal language theory](formal-language-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/2/a/solution.md)
