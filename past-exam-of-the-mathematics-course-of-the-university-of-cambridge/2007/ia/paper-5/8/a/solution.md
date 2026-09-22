<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [processor privilege level](../../../../../../processor-privilege-level.md) distinguishes user execution from the privileged [operating-system kernel](../../../../../../kernel-operating-system.md). In user state, privileged instructions such as changing page-table control registers, reconfiguring devices or altering protected interrupt controls are forbidden and trap if attempted. Memory accesses are also checked against user-access permissions. Supervisor state permits the kernel to manage these resources; protected transition mechanisms keep user programs from merely setting the privilege bit themselves.

[Interrupt masking](../../../../../../interrupt-masking.md) controls delivery of maskable asynchronous [interrupts](../../../../../../interrupt.md). Enabled interrupts allow devices and timers to transfer control to the kernel between instructions; disabling them permits short critical operations without those particular interruptions. It does not normally disable synchronous exceptions, faults or nonmaskable interrupts. These two kinds of status bits are independent: privilege determines which instructions and accesses are authorized, whereas the interrupt mask determines which asynchronous events can preempt execution. **Privilege protects the machine; interrupt enablement controls asynchronous entry.**

## ↑ Ancestors (11)

1. [A](../a.md)
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
