# Interrupt

↑ **Parent:** [Operating system](operating-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interrupt)

An [interrupt](interrupt.md) redirects [CPU](central-processing-unit.md) execution to an [interrupt handler](interrupt-handler.md) in response to an event. Here the main case is an asynchronous hardware [interrupt](interrupt.md): a timer or device requests attention independently of the instruction currently being executed. A device completing a receive operation can announce that its data is ready while the [CPU](central-processing-unit.md) is running another program. [Interrupt-driven input-output](interrupt-driven-input-output.md) illustrates this with an explicit timeline. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 6, section 6.3: timer interrupts and regaining control](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-mechanisms.pdf)

A [synchronous processor exception](synchronous-processor-exception.md), such as a [page fault](page-fault.md) caused by a particular memory access, is tied to instruction execution. A [system call](system-call.md) is an intentional program request for an [operating-system kernel](kernel-operating-system.md) service. These routes can share entry machinery, and an instruction named a software interrupt can implement a [system call](system-call.md), but this does not make that request an asynchronous device event. For example, the [Linux kernel](linux-kernel.md) on [x86](x86.md) documents separate entries for external [interrupts](interrupt.md), divide exceptions, `syscall` and `int 0x80`. [Linux kernel documentation, Kernel Entries: interrupt, exception and system-call entry points](https://docs.kernel.org/arch/x86/entry_64.html)

The usual device route is a request through an [interrupt controller](interrupt-controller.md), architecture-specific entry, and dispatch to an [interrupt handler](interrupt-handler.md). In the [Linux kernel](linux-kernel.md), generic handling separates controller operations from flow handling and [device driver](device-driver.md) callbacks. Requests can arrive through a pin or a message, and several devices can share a request source. Routing, priorities and [interrupt masking](interrupt-masking.md) determine which requests can be delivered; notification therefore need not mean immediate execution of the [interrupt handler](interrupt-handler.md). [Linux kernel documentation, generic IRQ handling: abstraction layers and interrupt control flow](https://docs.kernel.org/core-api/genericirq.html)[Linux kernel documentation, What is an IRQ?: pin and packet requests, shared sources](https://docs.kernel.org/core-api/irq/concepts.html)

The [CPU](central-processing-unit.md) and entry code preserve the state needed to resume interrupted execution, including the [instruction pointer](instruction-pointer.md). Handling may enter a higher [processor privilege level](processor-privilege-level.md) when interrupting ordinary program execution, but an [interrupt](interrupt.md) can also arrive while privileged code is already running. The protected entry route and handler placement depend on the architecture and [operating system](operating-system.md); a [microkernel](microkernel.md) need not place all [device driver](device-driver.md) work where a [monolithic kernel](monolithic-kernel.md) does. An [interrupt](interrupt.md) entry is also distinct from a [context switch](context-switch.md) to another [operating-system process](process-computing.md). [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 6, sections 6.2–6.3: protected entry, saved state and switching](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-mechanisms.pdf)[Linux kernel documentation, Kernel Entries: entry from user mode and already executing kernel code](https://docs.kernel.org/arch/x86/entry_64.html)

// Target: computer-science.bigb

**Table of contents**

- [Interrupt-driven input-output](interrupt-driven-input-output.md)
- [Interrupt handler](interrupt-handler.md)
- [Interrupt controller](interrupt-controller.md)
- [Interrupt masking](interrupt-masking.md)

## ↑ Ancestors (3)

1. [Operating system](operating-system.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Context switch](context-switch.md)
- [Direct memory access](direct-memory-access.md)
- [Interrupt](interrupt.md)
- [Interrupt controller](interrupt-controller.md)
- [Interrupt-driven input-output](interrupt-driven-input-output.md)
- [Interrupt handler](interrupt-handler.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/8/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/8/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5/8/b/solution.md)
- [Polled input-output](polled-input-output.md)
- [Scheduling preemption](scheduling-preemption.md)
- [Synchronous processor exception](synchronous-processor-exception.md)
