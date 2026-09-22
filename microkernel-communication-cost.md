# Microkernel communication cost

↑ **Parent:** [Microkernel](microkernel.md)

For the [microkernel file-read example](microkernel-file-read-example.md), distinguish [system call](system-call.md) entry/exit, [security capability](capability-computer-security.md) lookup, payload transfer, [process scheduling](process-scheduling.md) and [context switches](context-switch.md) from the service's actual [file](computer-file.md) lookup and read work. Entering a privileged [processor privilege level](processor-privilege-level.md) and switching to a different [address space](address-space.md) are different events. A change of [address space](address-space.md) can affect the [translation lookaside buffer](translation-lookaside-buffer.md); running different code and touching different [computer memory](computer-memory.md) can cause [cache misses](cache-miss.md). Neither event implies that every [translation lookaside buffer](translation-lookaside-buffer.md) entry or [cache line](cache-line.md) must be discarded.

A larger copied payload requires more transfer work; sharing [memory pages](memory-page.md) can avoid copying that bulk data but introduces mapping and [synchronization](synchronization-computing.md) work. A service that requests another service adds another [IPC](inter-process-communication.md) exchange. If the cached [file](computer-file.md) data were absent, communication with a [device driver](device-driver.md) and the [input-output](input-output.md) wait would also matter. Blocking behind other requests affects observed response time even when the individual [IPC](inter-process-communication.md) operations are cheap.

These are cost sources, not timings or a universal ranking against a [monolithic kernel](monolithic-kernel.md). Implementation and [CPU](central-processing-unit.md) details matter: the construction analysis separates protected entry costs, [address space](address-space.md) switching, [translation lookaside buffer](translation-lookaside-buffer.md) effects and [memory cache](cache-computing.md) effects. [Liedtke, On micro-kernel construction, section 4.1, pp. 241–244: kernel-user switches, address-space switches, and discussion of hardware-dependent cache and TLB effects](on-micro-kernel-construction-by-jochen-liedtke.md)

## ↑ Ancestors (5)

1. [Microkernel](microkernel.md)
2. [Kernel (operating system)](kernel-operating-system.md)
3. [Operating system](operating-system.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)
