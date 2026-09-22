<h1 id="8/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**Yes: supervisor execution with interrupts enabled is normal and useful.** Much of the [operating-system kernel](../../../../../../../kernel-operating-system.md) can execute with interrupts enabled so that timers, device completions and other urgent events receive prompt service. Disabling them for every potentially long system call would cause excessive latency and could prevent receipt of the very event needed for progress.

Handlers and shared data must then be protected against interrupt-time reentrancy. Disable relevant interrupts only for short critical sequences or use an appropriate synchronization mechanism; on multiple processors, local [interrupt masking](../../../../../../../interrupt-masking.md) alone does not protect against another processor. Interrupt enablement and [kernel preemption](../../../../../../../kernel-preemption.md) are different: an interrupt can be serviced without allowing an arbitrary process context to preempt the interrupted kernel operation.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [8](../../../8.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Ia](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
