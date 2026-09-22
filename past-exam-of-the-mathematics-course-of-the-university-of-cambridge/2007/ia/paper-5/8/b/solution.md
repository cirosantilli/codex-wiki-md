<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A system call or other synchronous trap from user code enters the privileged handler, saving the prior execution status; entry may also mask interrupts depending on the architecture. A device or timer [interrupt](../../../../../../interrupt.md) similarly saves the interrupted context, selects the privileged interrupt handler and commonly adjusts the interrupt mask to control nesting. A return-from-trap or return-from-interrupt instruction restores the saved status, ordinarily returning to user state with interrupts enabled.

These are three distinct transition situations. In addition, the [operating-system kernel](../../../../../../kernel-operating-system.md) can explicitly enable or disable interrupts around a critical section using privileged instructions. The exact entry mask is architecture-dependent; entering supervisor state does not logically require interrupts to remain disabled throughout the handler.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
