<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First, suppressing [kernel preemption](../../../../../../kernel-preemption.md) simplifies protection of shared kernel data on a uniprocessor: another ordinary kernel execution cannot be scheduled in the middle of a short update which temporarily breaks an invariant. Fewer paths require preemption-specific locking and reentrancy handling, making the [operating-system kernel](../../../../../../kernel-operating-system.md) easier to implement correctly.

Second, it avoids involuntary kernel [context switches](../../../../../../context-switch.md) and their scheduler, register-save and cache-disruption costs, and can make the execution of short kernel operations more predictable. The tradeoff is greater scheduling latency if a kernel operation runs too long. **Simpler synchronization and lower switching overhead are the two reasons.** Non-preemptive kernel code can still receive [interrupts](../../../../../../interrupt.md) or block voluntarily, and multiprocessor execution still requires synchronization; non-preemption is not a substitute for all locking.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
