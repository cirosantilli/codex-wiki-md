<h1 id="8/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In an ordinary general-purpose [operating system](../../../../../../../operating-system.md), **untrusted user code should not be allowed to disable the system's timer and device interrupts**. Otherwise a nonterminating program could prevent scheduling and device service. User mode is not a reason to permit arbitrary writes to protected interrupt controls.

A restricted trusted environment can nevertheless make this combination useful: a kernel may permit a short, bounded user-level real-time or device operation to run without maskable interrupts, or provide a virtualized per-task interrupt mask which delays that task's notifications while leaving system service active. Such permission must not let an untrusted task disable global service indefinitely. On a uniprocessor a short hardware-masked interval can reduce interruption latency, but it does not prevent faults, nonmaskable interrupts or activity on other cores. Thus the combination is meaningful in controlled cases, not a normal synchronization technique for arbitrary user programs.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
