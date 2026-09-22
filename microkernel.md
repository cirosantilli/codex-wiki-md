# Microkernel

↑ **Parent:** [Kernel (operating system)](kernel-operating-system.md)

An [operating-system kernel](kernel-operating-system.md) design retaining essential protected mechanisms while moving services into [user-space services](user-space-service.md). [Address spaces](address-space.md), [software threads](thread-computing.md) and [IPC](inter-process-communication.md) form a useful small foundation: the [operating-system kernel](kernel-operating-system.md) protects private state and controls communication, while a [file system](file-system-split.md) service interprets requests about [files](computer-file.md). This [separation of mechanism and policy](separation-of-mechanism-and-policy.md) permits different service implementations to use the same protected interface. [Liedtke, On micro-kernel construction, section 2, pp. 238–240: minimality criterion, address spaces, threads and IPC; section 3, pp. 240–241: user-level services](on-micro-kernel-construction-by-jochen-liedtke.md)

The useful question is which authority a service needs. A [device driver](device-driver.md) may require access to a device while having no permission to overwrite an unrelated application's [computer memory](computer-memory.md). A [microkernel](microkernel.md) makes such [protection domains](protection-domain.md) possible; their actual boundaries depend on the chosen [memory protection](memory-protection.md) and [security capabilities](capability-computer-security.md).

**Table of contents**

- [Microkernel file-read example](microkernel-file-read-example.md)
- [Microkernel service failure isolation](microkernel-service-failure-isolation.md)
- [Microkernel communication cost](microkernel-communication-cost.md)
- [seL4](sel4.md)
  - [seL4 verification scope](sel4-verification-scope.md)

## ↑ Ancestors (4)

1. [Kernel (operating system)](kernel-operating-system.md)
2. [Operating system](operating-system-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Formal specification](formal-specification.md)
- [Inter-process communication](inter-process-communication.md)
- [Interrupt](interrupt.md)
- [Kernel (operating system)](kernel-operating-system.md)
- [Microkernel](microkernel.md)
- [Microkernel file-read example](microkernel-file-read-example.md)
- [Microkernel service failure isolation](microkernel-service-failure-isolation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/2/d/solution.md)
- [seL4](sel4.md)
- [Separation of mechanism and policy](separation-of-mechanism-and-policy.md)
- [User-space service](user-space-service.md)
