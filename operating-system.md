# Operating system

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Operating_system)

An [operating system](operating-system.md) manages the resources that let programs run and cooperate. [Operating-system processes](#process-computing) organize running work, [virtual memory](virtual-memory.md) supplies protected [address spaces](virtual-memory.md#address-space), and a [file system](file-system.md) supplies named [files](file-system.md#computer-file) that can outlive the [operating-system process](#process-computing) that created them. The [operating-system kernel](#kernel-operating-system) enforces the core mechanisms; [system calls](#system-call) let programs request its services. Separating these responsibilities makes it possible to share a [file](file-system.md#computer-file) while keeping the participating [operating-system processes](#process-computing)' [address spaces](virtual-memory.md#address-space) isolated. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 39, introduction: processes, address spaces and persistent storage](https://pages.cs.wisc.edu/~remzi/OSTEP/file-intro.pdf)

A concrete example makes the separation useful: two [operating-system processes](#process-computing) can each use [file descriptor](#file-descriptor) `3`, yet refer to different [files](file-system.md#computer-file); two different names can instead refer to the same [file](file-system.md#computer-file) through [hard links](file-system.md#hard-link). Neither a name nor a small [integer](integer.md) identifies an object without its context. [Virtual memory](virtual-memory.md) has a related distinction: the same [virtual address](virtual-memory.md#virtual-address) in different [address spaces](virtual-memory.md#address-space) can designate different [physical addresses](computer-science.md#physical-address).

[Unix](#unix) provides an influential example of this design. In their July 1974 paper, Dennis M. Ritchie and Ken Thompson date its earliest version to approximately 1969–70 and describe [operating-system processes](#process-computing), a hierarchical [file system](file-system.md), and [inodes](file-system.md#inode) separating [directory entries](file-system.md#directory-entry) from [file metadata](file-system.md#file-metadata). This is a documented historical example, rather than a claim that every [operating system](operating-system.md) uses [Unix](#unix) conventions. [Ritchie and Thompson, The UNIX Time-Sharing System, Communications of the ACM 17(7), 1974, sections 1, 3 and 4](https://www.cs.cmu.edu/~15712/papers/ritchie74.pdf)

**Table of contents**

- [POSIX](#posix)
- [Unix](#unix)
- [Windows XP](#windows-xp)
- [Polled input-output](#polled-input-output)
- [Access matrix](#access-matrix)
  - [Capability (computer security)](#capability-computer-security)
    - [Reply capability](#reply-capability)
- [File system](file-system.md)
  - [Computer file](file-system.md#computer-file)
    - [File offset](file-system.md#file-offset)
    - [File metadata](file-system.md#file-metadata)
    - [File data block](file-system.md#file-data-block)
  - [File-system directory](file-system.md#file-system-directory)
    - [Directory entry](file-system.md#directory-entry)
  - [File-system namespace](file-system.md#file-system-namespace)
    - [Hard link](file-system.md#hard-link)
      - [Unlinking an open file](file-system.md#unlinking-an-open-file)
    - [Symbolic link](file-system.md#symbolic-link)
  - [Buffer cache](file-system.md#buffer-cache)
    - [Buffered device block](file-system.md#buffered-device-block)
      - [Buffer cache key](file-system.md#buffer-cache-key)
      - [Buffer cache validity](file-system.md#buffer-cache-validity)
      - [Dirty buffer](file-system.md#dirty-buffer)
      - [Clean buffer](file-system.md#clean-buffer)
      - [Pinned buffer](file-system.md#pinned-buffer)
    - [Buffer cache writeback](file-system.md#buffer-cache-writeback)
    - [Buffer cache eviction](file-system.md#buffer-cache-eviction)
    - [Buffer cache state model](file-system.md#buffer-cache-state-model)
      - [Buffer cache access trace](file-system.md#buffer-cache-access-trace)
    - [xv6 buffer cache](file-system.md#xv6-buffer-cache)
    - [Page cache](file-system.md#page-cache)
      - [Linux buffer head](file-system.md#linux-buffer-head)
      - [Linux folio](file-system.md#linux-folio)
      - [iomap](file-system.md#iomap)
  - [File-system journaling](file-system.md#file-system-journaling)
    - [File-system crash consistency](file-system.md#file-system-crash-consistency)
    - [File-system transaction](file-system.md#file-system-transaction)
      - [File-system transaction durability](file-system.md#file-system-transaction-durability)
        - [fsync](file-system.md#fsync)
    - [Write-ahead logging](file-system.md#write-ahead-logging)
      - [Journal payload](file-system.md#journal-payload)
      - [Journal commit record](file-system.md#journal-commit-record)
      - [Journal checkpoint](file-system.md#journal-checkpoint)
      - [Journal replay](file-system.md#journal-replay)
    - [File-system journaling mode](file-system.md#file-system-journaling-mode)
  - [File-system allocation bitmap](file-system.md#file-system-allocation-bitmap)
    - [Block allocation bitmap](file-system.md#block-allocation-bitmap)
    - [Inode allocation bitmap](file-system.md#inode-allocation-bitmap)
  - [Storage flush](file-system.md#storage-flush)
  - [Atomic storage write](file-system.md#atomic-storage-write)
  - [ext4](file-system.md#ext4)
  - [File-system backup](file-system.md#file-system-backup)
  - [Access control list](file-system.md#access-control-list)
  - [File Allocation Table](file-system.md#file-allocation-table)
    - [FAT32](file-system.md#fat32)
  - [NTFS](file-system.md#ntfs)
  - [Inode](file-system.md#inode)
- [Synchronous processor exception](#synchronous-processor-exception)
- [Device driver](#device-driver)
- [Interrupt](#interrupt)
  - [Interrupt-driven input-output](#interrupt-driven-input-output)
  - [Interrupt handler](#interrupt-handler)
  - [Interrupt controller](#interrupt-controller)
  - [Interrupt masking](#interrupt-masking)
- [Processor privilege level](#processor-privilege-level)
- [Multics](#multics)
- [Multiprogramming](#multiprogramming)
- [Virtual memory](virtual-memory.md)
  - [Address space](virtual-memory.md#address-space)
    - [Virtual address](virtual-memory.md#virtual-address)
  - [Address translation](virtual-memory.md#address-translation)
  - [Memory management unit](virtual-memory.md#memory-management-unit)
  - [Memory protection](virtual-memory.md#memory-protection)
  - [Copy-on-write](virtual-memory.md#copy-on-write)
    - [Copy-on-write fault handling](virtual-memory.md#copy-on-write-fault-handling)
    - [Copy-on-write page accounting](virtual-memory.md#copy-on-write-page-accounting)
  - [Thrashing (computer science)](virtual-memory.md#thrashing-computer-science)
  - [Working set](virtual-memory.md#working-set)
    - [Working set size](virtual-memory.md#working-set-size)
  - [Resident set](virtual-memory.md#resident-set)
  - [Memory-mapped file](virtual-memory.md#memory-mapped-file)
    - [Backing file](virtual-memory.md#backing-file)
    - [mmap](virtual-memory.md#mmap)
      - [munmap](virtual-memory.md#munmap)
    - [Memory-mapped file offset translation](virtual-memory.md#memory-mapped-file-offset-translation)
    - [Shared file mapping](virtual-memory.md#shared-file-mapping)
    - [Private file mapping](virtual-memory.md#private-file-mapping)
    - [Memory-mapped file synchronization](virtual-memory.md#memory-mapped-file-synchronization)
      - [msync](virtual-memory.md#msync)
  - [Memory segmentation](virtual-memory.md#memory-segmentation)
  - [Paging](virtual-memory.md#paging)
    - [Memory page](virtual-memory.md#memory-page)
    - [Page frame](virtual-memory.md#page-frame)
    - [Demand paging](virtual-memory.md#demand-paging)
    - [Page replacement](virtual-memory.md#page-replacement)
      - [CLOCK page replacement](virtual-memory.md#clock-page-replacement)
      - [LRU replacement](virtual-memory.md#lru-replacement)
        - [LRU cache](virtual-memory.md#lru-cache)
        - [LRU stack property](virtual-memory.md#lru-stack-property)
      - [FIFO page replacement](virtual-memory.md#fifo-page-replacement)
        - [FIFO cache](virtual-memory.md#fifo-cache)
      - [Page-reference trace](virtual-memory.md#page-reference-trace)
      - [Optimal page replacement](virtual-memory.md#optimal-page-replacement)
      - [Bélády's anomaly](virtual-memory.md#belady-s-anomaly)
      - [Dirty memory page](virtual-memory.md#dirty-memory-page)
        - [Page writeback](virtual-memory.md#page-writeback)
      - [Page-replacement cost accounting](virtual-memory.md#page-replacement-cost-accounting)
    - [Page fault](virtual-memory.md#page-fault)
      - [Page fault rate](virtual-memory.md#page-fault-rate)
    - [Translation lookaside buffer](virtual-memory.md#translation-lookaside-buffer)
      - [TLB hit](virtual-memory.md#tlb-hit)
      - [TLB miss](virtual-memory.md#tlb-miss)
      - [Address space identifier](virtual-memory.md#address-space-identifier)
    - [Page table](virtual-memory.md#page-table)
      - [Page table entry](virtual-memory.md#page-table-entry)
      - [Multi-level page table](virtual-memory.md#multi-level-page-table)
        - [Two-level address translation](virtual-memory.md#two-level-address-translation)
        - [Sparse page table allocation](virtual-memory.md#sparse-page-table-allocation)
        - [Sv39 page table](virtual-memory.md#sv39-page-table)
      - [Page table walk](virtual-memory.md#page-table-walk)
- [Set-user-ID execution](#set-user-id-execution)
- [Protection domain](#protection-domain)
- [User-space service](#user-space-service)
- [Separation of mechanism and policy](#separation-of-mechanism-and-policy)
- [Inter-process communication](#inter-process-communication)
  - [IPC endpoint](#ipc-endpoint)
- [Kernel (operating system)](#kernel-operating-system)
  - [System call](#system-call)
    - [Fork (system call)](#fork-system-call)
  - [Linux kernel](#linux-kernel)
  - [Monolithic kernel](#monolithic-kernel)
  - [Microkernel](#microkernel)
    - [Microkernel file-read example](#microkernel-file-read-example)
    - [Microkernel service failure isolation](#microkernel-service-failure-isolation)
    - [Microkernel communication cost](#microkernel-communication-cost)
    - [seL4](#sel4)
      - [seL4 verification scope](#sel4-verification-scope)
  - [Kernel preemption](#kernel-preemption)
- [Process scheduling](#process-scheduling)
  - [Ready queue](#ready-queue)
  - [CPU burst](#cpu-burst)
  - [Round-robin scheduling](#round-robin-scheduling)
    - [Scheduling quantum](#scheduling-quantum)
  - [Scheduling preemption](#scheduling-preemption)
  - [Scheduling response time](#scheduling-response-time)
  - [Scheduling turnaround time](#scheduling-turnaround-time)
  - [Scheduling waiting time](#scheduling-waiting-time)
  - [Context switch](#context-switch)
    - [Execution context](#execution-context)
- [Process (computing)](#process-computing)
  - [File descriptor](#file-descriptor)
    - [Open file description](#open-file-description)
  - [Thread (computing)](#thread-computing)
    - [Race condition](#race-condition)
    - [Synchronization (computing)](#synchronization-computing)
      - [Mutual exclusion](#mutual-exclusion)
        - [Critical section](#critical-section)
        - [Mutex](#mutex)
          - [Spinlock](#spinlock)
            - [Test-and-set](#test-and-set)
        - [Thread interleaving](#thread-interleaving)
          - [Lost update](#lost-update)
      - [Safety property](#safety-property)
      - [Liveness property](#liveness-property)
        - [Starvation freedom](#starvation-freedom)
      - [Deadlock](#deadlock)
        - [Deadlock freedom](#deadlock-freedom)
        - [Lock ordering](#lock-ordering)
      - [Memory model](#memory-model)
        - [Sequential consistency](#sequential-consistency)
        - [Data race](#data-race)
        - [Happens-before](#happens-before)
          - [Acquire-release synchronization](#acquire-release-synchronization)
      - [Atomic operation](#atomic-operation)
        - [Atomic read-modify-write](#atomic-read-modify-write)

## POSIX

↑ **Parent:** [Operating system](operating-system.md)

The Portable Operating System Interface standards specify interfaces and observable behaviour for portable programs, including [file descriptors](#file-descriptor), [hard links](file-system.md#hard-link) and [unlinking an open file](file-system.md#unlinking-an-open-file). Their requirements do not prescribe one on-storage [inode](file-system.md#inode) layout. The worked examples below use [POSIX](#posix) [Unix](#unix) semantics for ordinary [files](file-system.md#computer-file). [The Open Group, POSIX.1-2024, definitions of files, directories and file descriptors](https://pubs.opengroup.org/onlinepubs/9799919799/basedefs/V1_chap03.html)

// Target: computer-science.bigb

## Unix

↑ **Parent:** [Operating system](operating-system.md)

An operating-system family with process, file and pipe abstractions. The traditional discretionary file-permission model separates owner, group and other users and read, write and execute rights. Individual Unix systems can add richer [access control lists](file-system.md#access-control-list) and other protection mechanisms.

// Destination: computer-science.bigb

## Windows XP

↑ **Parent:** [Operating system](operating-system.md)

A member of the Windows NT operating-system family. Executive services such as object, memory and input-output management execute in privileged kernel mode. Its object-level [access control lists](file-system.md#access-control-list) and subject tokens permit finer authorization policies than traditional owner-group-other file permissions.

// Destination: computer-science.bigb

## Polled input-output

↑ **Parent:** [Operating system](operating-system.md)

In [polled input-output](#polled-input-output), the [CPU](computer-science.md#central-processing-unit) explicitly checks a device's status to discover whether work is ready or an operation has completed. Repeatedly checking in a tight loop is busy polling; periodic checks can instead leave time for other work. [Interrupt-driven input-output](#interrupt-driven-input-output) changes how readiness is discovered, while [DMA](computer-science.md#direct-memory-access) changes how payload data moves. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 36, sections 36.3–36.5: polling, interrupts and DMA](https://pages.cs.wisc.edu/~remzi/OSTEP/file-devices.pdf)

Use the model drawn under [interrupt-driven input-output](#interrupt-driven-input-output): device events occur at times $2,5,9$, while polls occur at $0,2,4,6,8,10,12$. Assume each event remains pending until detected and an event simultaneous with a poll is visible to that poll. The detection times are $2,6,10$, giving delays $0,1,1$. Four of the seven checks find no new event. These are event-detection delays, not completion times for servicing the events.

More generally, for polls at $0,\Delta,2\Delta,\ldots$ with $\Delta>0$, an event at time $t\geq0$ is first detected at

$$
d(t)=\Delta\left\lceil\frac{t}{\Delta}\right\rceil,\qquad 0\leq d(t)-t<\Delta.
$$

The [ceiling function](calculus.md#ceiling-function) chooses the first poll at or after the event. To verify the bound, that poll is less than one interval beyond $t$; if $t$ is itself a poll time, the delay is zero by the stated visibility convention. This argument assumes instantaneous checks, persistent pending status and an uninterrupted poll schedule. It does not describe missed transient events or a [CPU](computer-science.md#central-processing-unit) too busy to maintain that schedule.

The attraction of [polled input-output](#polled-input-output) is simple control and the possibility of processing several ready items in one visit. Busy polling spends [CPU](computer-science.md#central-processing-unit) time even when nothing is ready, but short waits or frequent events can make avoiding repeated [interrupt](#interrupt) entry worthwhile. The right choice depends on actual checking, notification and service costs. See [interrupt-driven input-output](#interrupt-driven-input-output) for a documented combination of both strategies. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 36, section 36.4: polling and interrupt tradeoffs](https://pages.cs.wisc.edu/~remzi/OSTEP/file-devices.pdf)

// Destination: computer-science.bigb

## Access matrix

↑ **Parent:** [Operating system](operating-system.md)

An authorization table with subjects or protection domains as rows, objects as columns, and sets of allowed operations as entries. An [access control list](file-system.md#access-control-list) stores an object column; a capability list stores a subject row. This representation is not a numerical linear map and has no ordinary floating-point matrix inverse.

// Destination: computer-science.bigb

### Capability (computer security)

↑ **Parent:** [Access matrix](#access-matrix)

An unforgeable reference carrying authority to perform specified operations on an object. In [seL4](#sel4), the [operating-system kernel](#kernel-operating-system) stores [security capabilities](#capability-computer-security) in protected slots; an [integer](integer.md) naming a slot is not itself freely forgeable authority. Guessing another [operating-system process](#process-computing)'s slot number does not give access to its [security capability](#capability-computer-security). [Capabilities tutorial, Background: What is a capability?; CNodes and CSlots](computer-science-bibliography.md#capabilities-tutorial-by-sel4-project)

#### Reply capability

↑ **Parent:** [Capability (computer security)](#capability-computer-security)

A [security capability](#capability-computer-security) authorizing a reply to a particular waiting caller. In the [seL4](#sel4) tutorial's [IPC](#inter-process-communication) model, a call establishes one-time reply authority, allowing a [user-space service](#user-space-service) to return to the correct client. The exact representation depends on the [operating-system kernel](#kernel-operating-system) configuration. [IPC tutorial, Background: System calls, seL4\_Call and reply capabilities](computer-science-bibliography.md#ipc-tutorial-by-sel4-project)

## File system

↑ **Parent:** [Operating system](operating-system.md)

[This section is present in another page, follow this link to view it.](file-system.md)

## Synchronous processor exception

↑ **Parent:** [Operating system](operating-system.md)

A processor event attributable to instruction execution, such as a [page fault](virtual-memory.md#page-fault) during a memory access or a divide exception on [x86](computer-science.md#x86). This causal connection distinguishes it from the asynchronous device [interrupts](#interrupt) discussed here. It also differs from a programming language's [exception handling](programming-language.md#exception-handling), which specifies how program-level exceptions propagate. [Linux kernel documentation, Kernel Entries: architecturally defined exceptions](https://docs.kernel.org/arch/x86/entry_64.html)

## Device driver

↑ **Parent:** [Operating system](operating-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Device_driver)

Software supplying device-specific operations behind an [operating system](operating-system.md) interface. For these examples its responsibilities include [DMA](computer-science.md#direct-memory-access) setup and completion handling, or checking status for [polled input-output](#polled-input-output). [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 36, section 36.7: the driver abstraction](https://pages.cs.wisc.edu/~remzi/OSTEP/file-devices.pdf)

## Interrupt

↑ **Parent:** [Operating system](operating-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interrupt)

An [interrupt](#interrupt) redirects [CPU](computer-science.md#central-processing-unit) execution to an [interrupt handler](#interrupt-handler) in response to an event. Here the main case is an asynchronous hardware [interrupt](#interrupt): a timer or device requests attention independently of the instruction currently being executed. A device completing a receive operation can announce that its data is ready while the [CPU](computer-science.md#central-processing-unit) is running another program. [Interrupt-driven input-output](#interrupt-driven-input-output) illustrates this with an explicit timeline. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 6, section 6.3: timer interrupts and regaining control](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-mechanisms.pdf)

A [synchronous processor exception](#synchronous-processor-exception), such as a [page fault](virtual-memory.md#page-fault) caused by a particular memory access, is tied to instruction execution. A [system call](#system-call) is an intentional program request for an [operating-system kernel](#kernel-operating-system) service. These routes can share entry machinery, and an instruction named a software interrupt can implement a [system call](#system-call), but this does not make that request an asynchronous device event. For example, the [Linux kernel](#linux-kernel) on [x86](computer-science.md#x86) documents separate entries for external [interrupts](#interrupt), divide exceptions, `syscall` and `int 0x80`. [Linux kernel documentation, Kernel Entries: interrupt, exception and system-call entry points](https://docs.kernel.org/arch/x86/entry_64.html)

The usual device route is a request through an [interrupt controller](#interrupt-controller), architecture-specific entry, and dispatch to an [interrupt handler](#interrupt-handler). In the [Linux kernel](#linux-kernel), generic handling separates controller operations from flow handling and [device driver](#device-driver) callbacks. Requests can arrive through a pin or a message, and several devices can share a request source. Routing, priorities and [interrupt masking](#interrupt-masking) determine which requests can be delivered; notification therefore need not mean immediate execution of the [interrupt handler](#interrupt-handler). [Linux kernel documentation, generic IRQ handling: abstraction layers and interrupt control flow](https://docs.kernel.org/core-api/genericirq.html)[Linux kernel documentation, What is an IRQ?: pin and packet requests, shared sources](https://docs.kernel.org/core-api/irq/concepts.html)

The [CPU](computer-science.md#central-processing-unit) and entry code preserve the state needed to resume interrupted execution, including the [instruction pointer](computer-science.md#instruction-pointer). Handling may enter a higher [processor privilege level](#processor-privilege-level) when interrupting ordinary program execution, but an [interrupt](#interrupt) can also arrive while privileged code is already running. The protected entry route and handler placement depend on the architecture and [operating system](operating-system.md); a [microkernel](#microkernel) need not place all [device driver](#device-driver) work where a [monolithic kernel](#monolithic-kernel) does. An [interrupt](#interrupt) entry is also distinct from a [context switch](#context-switch) to another [operating-system process](#process-computing). [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 6, sections 6.2–6.3: protected entry, saved state and switching](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-mechanisms.pdf)[Linux kernel documentation, Kernel Entries: entry from user mode and already executing kernel code](https://docs.kernel.org/arch/x86/entry_64.html)

// Target: computer-science.bigb

### Interrupt-driven input-output

↑ **Parent:** [Interrupt](#interrupt)

In [interrupt-driven input-output](#interrupt-driven-input-output), a device signals an [interrupt](#interrupt) when attention is needed, letting the [CPU](computer-science.md#central-processing-unit) avoid repeatedly checking an idle device. The [interrupt handler](#interrupt-handler) determines what happened and arranges the required work; notification itself does not move the payload. [DMA](computer-science.md#direct-memory-access) can supply that separate data-transfer mechanism.

For a toy comparison, let events occur at times $2,5,9$. Ideal [interrupt](#interrupt) notification happens at those same times, while [polled input-output](#polled-input-output) at $0,2,4,6,8,10,12$ detects them at $2,6,10$. The polling delays are $0,1,1$; ideal notification delays are all zero. Events are assumed to remain pending, with a simultaneous event visible to a poll. The chart is a model, not a measurement: it excludes [interrupt](#interrupt) delivery and dispatch latency, [interrupt handler](#interrupt-handler) service time, and polling overhead. Its zero-delay row is not a real-hardware guarantee.

<a id="image-ideal-interrupt-notification-versus-periodic-polled-input-output-for-three-persistent-device-events"></a>
![](interrupt-versus-polling-timeline.png)

**[Figure 1](#image-ideal-interrupt-notification-versus-periodic-polled-input-output-for-three-persistent-device-events). Ideal interrupt notification versus periodic polled input-output for three persistent device events**.

The useful idea is to spend attention when something changes. Sparse events can leave long stretches for useful [CPU](computer-science.md#central-processing-unit) work instead of busy checks. At high event rates, repeated entry and service overhead can consume that saving. Batching notifications can reduce their frequency while delaying some events; switching to [polled input-output](#polled-input-output) during active periods is another option. No strategy is universally faster. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 36, section 36.4: interrupt costs and coalescing](https://pages.cs.wisc.edu/~remzi/OSTEP/file-devices.pdf)

The [Linux kernel](#linux-kernel)'s NAPI mechanism is a concrete combination: an [interrupt](#interrupt) normally schedules event processing, which polls for work with a receive budget. Further [interrupts](#interrupt) remain masked during that polling, and are enabled again when polling finishes. NAPI also supports busy polling; the exact processing context and configuration vary. This is a documented [Linux kernel](#linux-kernel) design, not a requirement on every [operating system](operating-system.md). [Linux kernel documentation, NAPI: basic operation, datapath API, scheduling and IRQ masking](https://docs.kernel.org/networking/napi.html)

### Interrupt handler

↑ **Parent:** [Interrupt](#interrupt)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interrupt_handler)

Code entered to handle an [interrupt](#interrupt). It identifies and acknowledges relevant device state and arranges service, possibly deferring work. The [Linux kernel](#linux-kernel)'s generic flow layer and [device driver](#device-driver) callback have distinct responsibilities. [Linux kernel documentation, generic IRQ handling: interrupt control flow and default flow implementations](https://docs.kernel.org/core-api/genericirq.html)

### Interrupt controller

↑ **Parent:** [Interrupt](#interrupt)

Hardware managing and routing [interrupt](#interrupt) requests to a [CPU](computer-science.md#central-processing-unit), with architecture-dependent masking and priority rules. The [Linux kernel](#linux-kernel) encapsulates its operations separately from generic flow handlers. [Linux kernel documentation, generic IRQ handling: chip-level hardware encapsulation](https://docs.kernel.org/core-api/genericirq.html)

// Destination: computer-science.bigb

### Interrupt masking

↑ **Parent:** [Interrupt](#interrupt)

Disabling selected asynchronous interrupt delivery, normally under privileged control. It does not necessarily disable processor exceptions, nonmaskable interrupts or activity on other processors.

// Target: computer-science.bigb

## Processor privilege level

↑ **Parent:** [Operating system](operating-system.md)

// Target: computer-science.bigb

## Multics

↑ **Parent:** [Operating system](operating-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multics)

// Target: computer-science.bigb

## Multiprogramming

↑ **Parent:** [Operating system](operating-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiprogramming)

Keeping several [operating-system processes](#process-computing) available so [process scheduling](#process-scheduling) can run another when one waits. Increasing their number can increase the combined [working set](virtual-memory.md#working-set) demand beyond the available [page frames](virtual-memory.md#page-frame), producing [memory thrashing](virtual-memory.md#thrashing-computer-science) rather than more useful [CPU](computer-science.md#central-processing-unit) work.

## Virtual memory

↑ **Parent:** [Operating system](operating-system.md)

[This section is present in another page, follow this link to view it.](virtual-memory.md)

## Set-user-ID execution

↑ **Parent:** [Operating system](operating-system.md)

Execution of a suitable executable with effective user identity set to its owner. A privileged executable writable by untrusted users permits code replacement and privilege escalation.

// Target: computer-science.bigb

## Protection domain

↑ **Parent:** [Operating system](operating-system.md)

A boundary within which code exercises a particular set of permissions. An [address space](virtual-memory.md#address-space) describes accessible [virtual addresses](virtual-memory.md#virtual-address); a [protection domain](#protection-domain) also concerns authority over other objects, such as [software threads](#thread-computing) and [IPC endpoints](#ipc-endpoint). Two [address spaces](virtual-memory.md#address-space) may deliberately share a writable [memory page](virtual-memory.md#memory-page), so separation of [address spaces](virtual-memory.md#address-space) alone does not make their contents independent.

## User-space service

↑ **Parent:** [Operating system](operating-system.md)

An [operating system](operating-system.md) service executing at an application's [processor privilege level](#processor-privilege-level), outside the [operating-system kernel](#kernel-operating-system). A [microkernel](#microkernel) can host a [file system](file-system.md) or [device driver](#device-driver) this way. Its granted [security capabilities](#capability-computer-security) and [memory protection](virtual-memory.md#memory-protection) determine its authority; the label [user-space service](#user-space-service) does not imply that it has little authority.

## Separation of mechanism and policy

↑ **Parent:** [Operating system](operating-system.md)

Distinguishing the operations a system can enforce from the choices about how to use them. In a [microkernel](#microkernel), a protected [IPC](#inter-process-communication) operation can deliver requests while a [user-space service](#user-space-service) decides which [files](file-system.md#computer-file) a caller may read. The division is a design choice: every real mechanism still has rules and limits.

## Inter-process communication

↑ **Parent:** [Operating system](operating-system.md)

Communication between [operating-system processes](#process-computing), including controlled message delivery and deliberately shared [computer memory](computer-science.md#computer-memory). A [microkernel](#microkernel) supplies [IPC](#inter-process-communication) across [protection domains](#protection-domain), allowing [user-space services](#user-space-service) to cooperate without making all their private [computer memory](computer-science.md#computer-memory) accessible to each other.

### IPC endpoint

↑ **Parent:** [Inter-process communication](#inter-process-communication)

A communication object on which [software threads](#thread-computing) send or receive [IPC](#inter-process-communication) messages. In [seL4](#sel4), an [IPC endpoint](#ipc-endpoint) is an [operating-system kernel](#kernel-operating-system) object with waiting senders or receivers; access requires a suitable [security capability](#capability-computer-security). [IPC tutorial, Background: endpoint queues](computer-science-bibliography.md#ipc-tutorial-by-sel4-project)

## Kernel (operating system)

↑ **Parent:** [Operating system](operating-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kernel_(operating_system))

The [operating-system kernel](#kernel-operating-system) is the core of an [operating system](operating-system.md), controlling access to resources and supplying mechanisms used by [operating-system processes](#process-computing). [Processor privilege levels](#processor-privilege-level) let it enforce boundaries that ordinary programs cannot simply overwrite. The [operating-system kernel](#kernel-operating-system) connects [process scheduling](#process-scheduling), [virtual memory](virtual-memory.md) and [file system](file-system.md) operations; a [system call](#system-call) requests a service across that boundary. A [monolithic kernel](#monolithic-kernel) and a [microkernel](#microkernel) divide services differently, so the location of every [file system](file-system.md) service is a design choice.

For the toy [file system](file-system.md), opening `a` resolves its [directory entry](file-system.md#directory-entry) to [inode](file-system.md#inode) 42, establishes an [open file description](#open-file-description), and returns [file descriptor](#file-descriptor) `3`. Later reads use that [file descriptor](#file-descriptor) to reach the existing [open file description](#open-file-description), without resolving the spelling `a` again. This explains how [unlinking an open file](file-system.md#unlinking-an-open-file) preserves access: the open reference survives the [directory entry](file-system.md#directory-entry). The per-[operating-system process](#process-computing) table interpreting `3` is maintained by the [operating-system kernel](#kernel-operating-system); `3` itself is the small [integer](integer.md) passed by the program, not [inode](file-system.md#inode) 42. [The Open Group, POSIX.1-2024, open: file descriptor to open file description to file](https://pubs.opengroup.org/onlinepubs/9799919799/functions/open.html)

### System call

↑ **Parent:** [Kernel (operating system)](#kernel-operating-system)

A request from a program for an [operating-system kernel](#kernel-operating-system) service. In the [Unix](#unix) examples here, opening, reading, linking and unlinking [files](file-system.md#computer-file) request controlled changes or access to [operating system](operating-system.md) resources. The [operating-system kernel](#kernel-operating-system) checks the request and performs the permitted operation; an interface specified by [POSIX](#posix) does not by itself dictate every internal implementation detail.

#### Fork (system call)

↑ **Parent:** [System call](#system-call)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fork_(system_call))

A [system call](#system-call) creating a child [operating-system process](#process-computing) from a parent. The [Linux kernel](#linux-kernel) documents [copy-on-write](virtual-memory.md#copy-on-write) for ordinary inherited private [memory pages](virtual-memory.md#memory-page), with separate [address spaces](virtual-memory.md#address-space) but shared [open file descriptions](#open-file-description) for inherited [file descriptors](#file-descriptor). [fork(2) — Linux manual page](computer-science-bibliography.md#fork-2-linux-manual-page)

### Linux kernel

↑ **Parent:** [Kernel (operating system)](#kernel-operating-system)

A concrete [operating-system kernel](#kernel-operating-system) whose documented [file system](file-system.md) interface distinguishes a name-associated `dentry`, an object-associated `inode`, and a `file` object created for an open instance. An [inode](file-system.md#inode) can have several name-associated objects. This illustrates the distinction among [directory entries](file-system.md#directory-entry), [inodes](file-system.md#inode) and [open file descriptions](#open-file-description); it does not imply identical structures in every [operating system](operating-system.md). [Linux kernel documentation, Overview of the Linux Virtual File System: directory entries, inode objects and file objects](https://docs.kernel.org/filesystems/vfs.html)

// Target: computer-science.bigb

### Monolithic kernel

↑ **Parent:** [Kernel (operating system)](#kernel-operating-system)

A kernel design in which major operating-system services execute within one privileged address space and can call one another directly. Avoiding cross-domain communication can improve performance, while increasing the trusted code base and the reach of a faulty service.

// Destination: computer-science.bigb

### Microkernel

↑ **Parent:** [Kernel (operating system)](#kernel-operating-system)

An [operating-system kernel](#kernel-operating-system) design retaining essential protected mechanisms while moving services into [user-space services](#user-space-service). [Address spaces](virtual-memory.md#address-space), [software threads](#thread-computing) and [IPC](#inter-process-communication) form a useful small foundation: the [operating-system kernel](#kernel-operating-system) protects private state and controls communication, while a [file system](file-system.md) service interprets requests about [files](file-system.md#computer-file). This [separation of mechanism and policy](#separation-of-mechanism-and-policy) permits different service implementations to use the same protected interface. [Liedtke, On micro-kernel construction, section 2, pp. 238–240: minimality criterion, address spaces, threads and IPC; section 3, pp. 240–241: user-level services](computer-science-bibliography.md#on-micro-kernel-construction-by-jochen-liedtke)

The useful question is which authority a service needs. A [device driver](#device-driver) may require access to a device while having no permission to overwrite an unrelated application's [computer memory](computer-science.md#computer-memory). A [microkernel](#microkernel) makes such [protection domains](#protection-domain) possible; their actual boundaries depend on the chosen [memory protection](virtual-memory.md#memory-protection) and [security capabilities](#capability-computer-security).

#### Microkernel file-read example

↑ **Parent:** [Microkernel](#microkernel)

Consider an original toy [file system](file-system.md) service in [address space](virtual-memory.md#address-space) B and a client in [address space](virtual-memory.md#address-space) A, on one [CPU](computer-science.md#central-processing-unit). The service holds a five-[byte](computer-science.md#byte) cached [file](file-system.md#computer-file) containing `LIME` followed by a newline. The client already has service handle `9`, permission to read that [file](file-system.md#computer-file), and a [security capability](#capability-computer-security) to send requests to [IPC endpoint](#ipc-endpoint) E. Handle `9` is interpreted by the service; it is neither a [virtual address](virtual-memory.md#virtual-address) nor an [operating-system kernel](#kernel-operating-system) object identifier. All relevant [memory pages](virtual-memory.md#memory-page) are resident, and this read needs no [device driver](#device-driver).

<a id="image-a-cached-file-read-uses-ipc-between-separate-address-spaces-with-authority-checked-by-the-microkernel"></a>
![](microkernel-file-read-message-path.png)

**[Figure 2](#image-a-cached-file-read-uses-ipc-between-separate-address-spaces-with-authority-checked-by-the-microkernel). A cached file read uses IPC between separate address spaces, with authority checked by the microkernel**.

- The client submits `READ(7, 9, 0, 4)`: request identifier `7`, handle `9`, [byte](computer-science.md#byte) offset `0`, and requested length `4`. A [system call](#system-call) enters the [microkernel](#microkernel); the [security capability](#capability-computer-security) is checked before delivery on [IPC endpoint](#ipc-endpoint) E. The client waits for a reply.
- A waiting service [software thread](#thread-computing) receives the request. The service checks the handle's read permission and the requested range, then obtains the first four [bytes](computer-science.md#byte) from its cached [file](file-system.md#computer-file). The [microkernel](#microkernel) transports the request; the service supplies its [file system](file-system.md) meaning.
- The service uses [reply capability](#reply-capability) authority to return `OK(7, 4, LIME)`. The client resumes, checks the request identifier and returned length, and copies those four [bytes](computer-science.md#byte) into its own local buffer. There were two logical [IPC](#inter-process-communication) messages: request and reply. The four arrows show delivery stages, not four separate requests.

This protocol is an illustrative design, not an actual [seL4](#sel4) [file system](file-system.md) interface. Its call/reply structure follows [seL4](#sel4)'s documented [IPC](#inter-process-communication): `seL4_Call` waits using reply authority, and small payloads can travel in [processor registers](computer-science.md#processor-register). [IPC tutorial, Background: System calls; IPC Buffer; Data transfer](computer-science-bibliography.md#ipc-tutorial-by-sel4-project)

An ordinary pointer in A refers to A's [address space](virtual-memory.md#address-space). Sending its numeric value does not make B's private [computer memory](computer-science.md#computer-memory) appear there. This example explicitly transfers [bytes](computer-science.md#byte). Sharing a mapped [memory page](virtual-memory.md#memory-page) instead would require intentional [memory protection](virtual-memory.md#memory-protection) permissions and a protocol for ownership and [synchronization](#synchronization-computing); passing a pointer alone establishes neither.

The same [IPC](#inter-process-communication) mechanism could carry `WRITE`, but this client could still be refused by the service's read-only handle policy. Conversely, possession of an [IPC endpoint](#ipc-endpoint) [security capability](#capability-computer-security) permits communication without automatically granting access to every [file](file-system.md#computer-file) the service manages. The [separation of mechanism and policy](#separation-of-mechanism-and-policy) appears twice: endpoint authority gates delivery, and the service's handle policy gates the requested operation.

#### Microkernel service failure isolation

↑ **Parent:** [Microkernel](#microkernel)

Suppose the [user-space service](#user-space-service) stops after receiving request `7`, before replying. Assume that its private [memory pages](virtual-memory.md#memory-page) are not writable mappings of the client's or an unrelated service's [computer memory](computer-science.md#computer-memory), and that it lacks [security capabilities](#capability-computer-security) to change their [software threads](#thread-computing). A failed store in the service cannot directly overwrite that private state through ordinary [CPU](computer-science.md#central-processing-unit) [address translation](virtual-memory.md#address-translation). Those assumptions establish a particular isolation boundary, not a successful read.

<a id="image-memory-protection-and-security-capabilities-limit-a-stopped-service-s-reach-recovery-needs-an-additional-design"></a>
![](microkernel-service-failure-authority-boundaries.png)

**[Figure 3](#image-memory-protection-and-security-capabilities-limit-a-stopped-service-s-reach-recovery-needs-an-additional-design). Memory protection and security capabilities limit a stopped service's reach; recovery needs an additional design**.

The client can remain blocked waiting for request `7`. An unrelated runnable service may continue if [process scheduling](#process-scheduling) and resources permit, but clients that depend on the stopped service still lose access to its service. A separately authorized recovery manager would need to detect the failure, rebuild the service's state and arrange communication with its replacement. The [microkernel](#microkernel) architecture by itself supplies none of those application-specific recovery decisions.

A missing reply also does not reveal whether a service crashed, is delayed by [process scheduling](#process-scheduling), or entered an infinite computation. For a read, retrying after recovery may be straightforward; for a modifying operation, absence of a reply does not prove that the modification never happened. Recovery must account for ambiguous completed operations and any required [file-system crash consistency](file-system.md#file-system-crash-consistency).

The boundary changes with authority. A deliberately shared writable [memory page](virtual-memory.md#memory-page) allows the service to change its shared contents; a [security capability](#capability-computer-security) controlling another [software thread](#thread-computing) permits the corresponding control operations. A [device driver](#device-driver) with uncontrolled [DMA](computer-science.md#direct-memory-access) can bypass ordinary [CPU](computer-science.md#central-processing-unit) [memory protection](virtual-memory.md#memory-protection). Thus service placement and actual permissions must be considered together. [What the Proofs Assume, The Assumptions: DMA and memory-mapped device registers](computer-science-bibliography.md#what-the-proofs-assume-by-sel4-project)

#### Microkernel communication cost

↑ **Parent:** [Microkernel](#microkernel)

For the [microkernel file-read example](#microkernel-file-read-example), distinguish [system call](#system-call) entry/exit, [security capability](#capability-computer-security) lookup, payload transfer, [process scheduling](#process-scheduling) and [context switches](#context-switch) from the service's actual [file](file-system.md#computer-file) lookup and read work. Entering a privileged [processor privilege level](#processor-privilege-level) and switching to a different [address space](virtual-memory.md#address-space) are different events. A change of [address space](virtual-memory.md#address-space) can affect the [translation lookaside buffer](virtual-memory.md#translation-lookaside-buffer); running different code and touching different [computer memory](computer-science.md#computer-memory) can cause [cache misses](computer-science.md#cache-miss). Neither event implies that every [translation lookaside buffer](virtual-memory.md#translation-lookaside-buffer) entry or [cache line](computer-science.md#cache-line) must be discarded.

A larger copied payload requires more transfer work; sharing [memory pages](virtual-memory.md#memory-page) can avoid copying that bulk data but introduces mapping and [synchronization](#synchronization-computing) work. A service that requests another service adds another [IPC](#inter-process-communication) exchange. If the cached [file](file-system.md#computer-file) data were absent, communication with a [device driver](#device-driver) and the [input-output](computer-science.md#input-output) wait would also matter. Blocking behind other requests affects observed response time even when the individual [IPC](#inter-process-communication) operations are cheap.

These are cost sources, not timings or a universal ranking against a [monolithic kernel](#monolithic-kernel). Implementation and [CPU](computer-science.md#central-processing-unit) details matter: the construction analysis separates protected entry costs, [address space](virtual-memory.md#address-space) switching, [translation lookaside buffer](virtual-memory.md#translation-lookaside-buffer) effects and [memory cache](computer-science.md#cache-computing) effects. [Liedtke, On micro-kernel construction, section 4.1, pp. 241–244: kernel-user switches, address-space switches, and discussion of hardware-dependent cache and TLB effects](computer-science-bibliography.md#on-micro-kernel-construction-by-jochen-liedtke)

#### seL4

↑ **Parent:** [Microkernel](#microkernel)

A [microkernel](#microkernel) using [security capabilities](#capability-computer-security) to control access to [operating-system kernel](#kernel-operating-system) objects, including [IPC endpoints](#ipc-endpoint) and [software threads](#thread-computing). An [IPC endpoint](#ipc-endpoint) connects cooperating [user-space services](#user-space-service); its [security capabilities](#capability-computer-security) are distinct from the service-defined handle `9` in the [microkernel file-read example](#microkernel-file-read-example). [Capabilities tutorial, Background: What is a capability?](computer-science-bibliography.md#capabilities-tutorial-by-sel4-project)

##### seL4 verification scope

↑ **Parent:** [seL4](#sel4)

[Formal verification](algorithm.md#formal-verification) uses machine-checked [formal proofs](mathematical-logic.md#formal-proof) to establish [functional correctness](algorithm.md#functional-correctness): the C implementation of verified [seL4](#sel4) configurations conforms to its [formal specification](algorithm.md#formal-specification). [Binary correctness](algorithm.md#binary-correctness) connects compiled machine code to that C behaviour where supported. Separate security [formal proofs](mathematical-logic.md#formal-proof) cover integrity, resource-access availability and confidentiality under their configuration requirements; these properties are not all available in every configuration. For example, the documented confidentiality theorem separates scheduler security domains rather than arbitrary pairs of [software threads](#thread-computing). [seL4 Proofs, High-level Proof Statements: Functional correctness; Binary correctness; Security; System initialisation; platform/configuration qualification](computer-science-bibliography.md#sel4-proofs-by-sel4-project)

The documented assumptions include correct hardware, selected handwritten machine-interface code, correct boot state, [translation lookaside buffer](virtual-memory.md#translation-lookaside-buffer) and [memory cache](computer-science.md#cache-computing) management, and noninterfering or trusted [DMA](computer-science.md#direct-memory-access). The confidentiality result covers information channels in its model; the assumptions page explicitly excludes timing channels from that coverage. [What the Proofs Assume, The Assumptions: Assembly, Hardware, Hardware management, Boot code, DMA, Information side-channels](computer-science-bibliography.md#what-the-proofs-assume-by-sel4-project)

Return to `READ(7, 9, 0, 4)`. Correct [IPC](#inter-process-communication) delivery does not establish that the service looked up the right [file](file-system.md#computer-file), returned `LIME`, or ever replied. A service can produce an incorrect payload while the [operating-system kernel](#kernel-operating-system) exactly follows its [formal specification](algorithm.md#formal-specification). The [formal proofs](mathematical-logic.md#formal-proof) therefore do not automatically prove all [user-space services](#user-space-service), nor turn the resource-access availability theorem into a guarantee that this [file](file-system.md#computer-file) read completes. The verified foundation supports further [algorithm correctness](algorithm.md#algorithm-correctness) and system reasoning; the service protocol and its recovery obligations still need their own justification.

// Destination: computer-science.bigb

### Kernel preemption

↑ **Parent:** [Kernel (operating system)](#kernel-operating-system)

Allows a running kernel execution to be involuntarily suspended for another schedulable context. Interrupt delivery and voluntary blocking are separate mechanisms.

// Target: computer-science.bigb

## Process scheduling

↑ **Parent:** [Operating system](operating-system.md)

[Process scheduling](#process-scheduling) chooses which runnable [operating-system process](#process-computing) or [software thread](#thread-computing) uses a [CPU](computer-science.md#central-processing-unit) next, and when it gives up that [CPU](computer-science.md#central-processing-unit). Runnable means able to execute now; work waiting for an [input-output](computer-science.md#input-output) operation is not eligible until that wait ends. A [ready queue](#ready-queue) records eligible work. The policy chooses a recipient; a [context switch](#context-switch) supplies the mechanism for transferring execution. Sharing a single [CPU](computer-science.md#central-processing-unit) lets a long calculation and an interactive program both make progress, although only one execution stream runs on that [CPU](computer-science.md#central-processing-unit) at an instant.

Consider three single-[software thread](#thread-computing) [operating-system processes](#process-computing) on one [CPU](computer-science.md#central-processing-unit), with abstract time units, zero [context switch](#context-switch) or scheduler overhead, and no [input-output](computer-science.md#input-output) blocking. Their arrival times and [CPU bursts](#cpu-burst) are $(a_A,b_A)=(0,5)$, $(a_B,b_B)=(1,3)$ and $(a_C,b_C)=(2,1)$. Each [CPU burst](#cpu-burst) is all the execution that its task needs. With [FCFS](queueing-theory.md#first-come-first-served), the current task runs to completion: A occupies $[0,5)$, B $[5,8)$ and C $[8,9)$. With [round-robin scheduling](#round-robin-scheduling) and [scheduling quantum](#scheduling-quantum) $q=2$, the intervals are A $[0,2)$, B $[2,4)$, C $[4,5)$, A $[5,7)$, B $[7,8)$ and A $[8,9)$. At a boundary, arrivals join the [ready queue](#ready-queue) before the unfinished task whose [scheduling quantum](#scheduling-quantum) has expired; this fixes the otherwise ambiguous ordering at time 2.

<a id="image-fcfs-and-round-robin-scheduling-share-the-same-nine-units-of-useful-cpu-work-differently"></a>
![](scheduling-fcfs-versus-round-robin.png)

**[Figure 4](#image-fcfs-and-round-robin-scheduling-share-the-same-nine-units-of-useful-cpu-work-differently). FCFS and round-robin scheduling share the same nine units of useful CPU work differently**.

The following triples always list A, B, C. Completion is an absolute time; [scheduling turnaround time](#scheduling-turnaround-time), [scheduling waiting time](#scheduling-waiting-time) and [scheduling response time](#scheduling-response-time) are durations measured from the relevant events.

| Policy | Completion times | [Scheduling turnaround times](#scheduling-turnaround-time) | [Scheduling waiting times](#scheduling-waiting-time) | [Scheduling response times](#scheduling-response-time) |
| --- | --- | --- | --- | --- |
| [FCFS](queueing-theory.md#first-come-first-served) | $(5,8,9)$ | $(5,7,7)$ | $(0,4,6)$ | $(0,4,6)$ |
| [Round-robin scheduling](#round-robin-scheduling), $q=2$ | $(9,8,5)$ | $(9,7,3)$ | $(4,4,2)$ | $(0,1,2)$ |

For example, B first runs at time 2 under [round-robin scheduling](#round-robin-scheduling), so its [scheduling response time](#scheduling-response-time) is $2-1=1$. It finishes at time 8, giving [scheduling turnaround time](#scheduling-turnaround-time) $8-1=7$ and [scheduling waiting time](#scheduling-waiting-time) $7-3=4$. Under [FCFS](queueing-theory.md#first-come-first-served), C waits $8-2=6$ before its sole execution interval. Under [round-robin scheduling](#round-robin-scheduling), A waits during $[2,5)$ and $[7,8)$, totaling $3+1=4$. Both timelines do exactly $5+3+1=9$ units of useful [CPU](computer-science.md#central-processing-unit) work; changing the order changes who benefits first.

The appeal is that shared progress can improve responsiveness: B and C get their first [CPU](computer-science.md#central-processing-unit) service sooner under [round-robin scheduling](#round-robin-scheduling), while A completes later. The [arithmetic mean](arithmetic.md#arithmetic-mean) of the [scheduling response times](#scheduling-response-time) falls from $10/3$ to $1$; the [arithmetic mean](arithmetic.md#arithmetic-mean) of the [scheduling turnaround times](#scheduling-turnaround-time) is $19/3$ for both policies in this particular example. These are different goals, and this workload establishes no universal ranking. Giving each continuously runnable task repeated turns is a practical form of fairness. A smaller [scheduling quantum](#scheduling-quantum) can shorten waits between turns, but makes [context switches](#context-switch) more frequent when competitors remain runnable. If each full slice performs $q$ units of useful work and incurs a fixed switching cost $s$, the overhead fraction in that simplified repeated cycle is $s/(q+s)$. Real costs and workloads determine the choice. [Remzi H. Arpaci-Dusseau and Andrea C. Arpaci-Dusseau, Operating Systems: Three Easy Pieces, chapter 7, sections 7.2–7.3 and 7.6–7.7: metrics, FCFS and round robin](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-sched.pdf)

### Ready queue

↑ **Parent:** [Process scheduling](#process-scheduling)

A collection of runnable [operating-system processes](#process-computing) or [software threads](#thread-computing) waiting for a [CPU](computer-science.md#central-processing-unit). A running task is not waiting in the [ready queue](#ready-queue), and a task waiting for [input-output](computer-science.md#input-output) is not runnable. [FCFS](queueing-theory.md#first-come-first-served) and [round-robin scheduling](#round-robin-scheduling) can use a [FIFO queue](data-structure.md#fifo-queue); other policies can organize eligible work differently, for example with a [priority queue](data-structure.md#priority-queue).

### CPU burst

↑ **Parent:** [Process scheduling](#process-scheduling)

An interval of useful [CPU](computer-science.md#central-processing-unit) execution needed before a task finishes or must wait, for example for [input-output](computer-science.md#input-output). A real [operating-system process](#process-computing) can need many [CPU bursts](#cpu-burst); the example under [process scheduling](#process-scheduling) assigns each task just one [CPU burst](#cpu-burst), possibly split across several turns by [round-robin scheduling](#round-robin-scheduling).

### Round-robin scheduling

↑ **Parent:** [Process scheduling](#process-scheduling)

Serve the front of a [FIFO queue](data-structure.md#fifo-queue) of runnable tasks for at most one [scheduling quantum](#scheduling-quantum). If the task finishes or must wait for [input-output](computer-science.md#input-output), it leaves the [CPU](computer-science.md#central-processing-unit) earlier; if it remains runnable after consuming its allowance, append it to the rear of the [ready queue](#ready-queue). In the example under [process scheduling](#process-scheduling), the [ready queue](#ready-queue) at time 2 is B, C, A: B arrived at time 1, C joins at the boundary, then A is requeued. That one convention determines the subsequent order.

#### Scheduling quantum

↑ **Parent:** [Round-robin scheduling](#round-robin-scheduling)

The maximum amount of [CPU](computer-science.md#central-processing-unit) execution allotted in one turn by [round-robin scheduling](#round-robin-scheduling). A task can finish before consuming its [scheduling quantum](#scheduling-quantum). When other tasks remain runnable, a shorter [scheduling quantum](#scheduling-quantum) provides more frequent turns at the cost of more frequent [context switches](#context-switch).

### Scheduling preemption

↑ **Parent:** [Process scheduling](#process-scheduling)

Taking the [CPU](computer-science.md#central-processing-unit) away from a still-runnable task before it voluntarily yields or finishes. [Round-robin scheduling](#round-robin-scheduling) uses [scheduling preemption](#scheduling-preemption) when a [scheduling quantum](#scheduling-quantum) expires, commonly using a timer [interrupt](#interrupt) to regain control. [Kernel preemption](#kernel-preemption) is the more specific question of whether an execution already within the [operating-system kernel](#kernel-operating-system) can be suspended for another runnable context.

### Scheduling response time

↑ **Parent:** [Process scheduling](#process-scheduling)

The delay from a task's arrival $a_i$ until its first execution $f_i$: $R_i=f_i-a_i$. This measures access to initial [CPU](computer-science.md#central-processing-unit) service, rather than completion of an entire user request. For C under [round-robin scheduling](#round-robin-scheduling) in [process scheduling](#process-scheduling), $R_C=4-2=2$; its [scheduling turnaround time](#scheduling-turnaround-time) is instead $5-2=3$.

### Scheduling turnaround time

↑ **Parent:** [Process scheduling](#process-scheduling)

The duration from a task's arrival $a_i$ until its completion $c_i$: $T_i=c_i-a_i$. It includes execution and all intervening waits. For A under [round-robin scheduling](#round-robin-scheduling) in [process scheduling](#process-scheduling), $T_A=9-0=9$, despite a [scheduling response time](#scheduling-response-time) of zero.

### Scheduling waiting time

↑ **Parent:** [Process scheduling](#process-scheduling)

The total duration a task spends runnable but waiting for a [CPU](computer-science.md#central-processing-unit), including later waits after [scheduling preemption](#scheduling-preemption). Under the zero-overhead, no-[input-output](computer-science.md#input-output)-blocking assumptions of [process scheduling](#process-scheduling), elapsed time partitions into useful execution and such waiting, so $W_i=T_i-b_i$, where $T_i$ is [scheduling turnaround time](#scheduling-turnaround-time) and $b_i$ is the total [CPU burst](#cpu-burst). Thus C under [round-robin scheduling](#round-robin-scheduling) has $W_C=3-1=2$. If a task also spends time blocked on [input-output](computer-science.md#input-output), that blocked duration belongs to [scheduling turnaround time](#scheduling-turnaround-time) but must not be counted as [scheduling waiting time](#scheduling-waiting-time).

// Target: computer-science.bigb

### Context switch

↑ **Parent:** [Process scheduling](#process-scheduling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Context_switch)

A [context switch](#context-switch) transfers [CPU](computer-science.md#central-processing-unit) execution from one [operating-system process](#process-computing) or [software thread](#thread-computing) to another while preserving enough [execution context](#execution-context) for the suspended task to resume. The [operating-system kernel](#kernel-operating-system) saves the outgoing task's [processor registers](computer-science.md#processor-register), including its resume [program counter](computer-science.md#instruction-pointer) and [stack pointer](computer-science.md#stack-pointer), and restores the incoming task's saved state. Hardware entry and software switching divide this work differently across architectures; the diagram groups them into logical save and load steps. During the transition the same [CPU](computer-science.md#central-processing-unit) executes the [operating-system kernel](#kernel-operating-system)'s scheduler and switching code. [Remzi H. Arpaci-Dusseau and Andrea C. Arpaci-Dusseau, Operating Systems: Three Easy Pieces, chapter 6, section 6.3: saving and restoring context](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-mechanisms.pdf)

For a schematic switch from A to B, let A's resume [program counter](computer-science.md#instruction-pointer) be $p_A$, its [stack pointer](computer-science.md#stack-pointer) $u_A$, and one illustrative data [processor register](computer-science.md#processor-register) contain 7. B's saved values are $p_B,u_B,42$. Saving A retains $(p_A,u_A,7)$ in A's [execution context](#execution-context); loading B establishes $(p_B,u_B,42)$ before B resumes. These are selected fields, not a complete architecture-specific [execution context](#execution-context). Later restoring A recovers its 7 even though B has used the same physical [processor register](computer-science.md#processor-register) for 42.

<a id="image-one-cpu-over-time-save-a-s-execution-context-run-the-scheduler-and-restore-b-s-execution-context"></a>
![](context-switch-state-transfer.png)

**[Figure 5](#image-one-cpu-over-time-save-a-s-execution-context-run-the-scheduler-and-restore-b-s-execution-context). One CPU over time: save A's execution context, run the scheduler, and restore B's execution context**.

The useful invariant is that each suspended task retains its own resume state, so another task's use of the [processor registers](computer-science.md#processor-register) does not erase it. This is what makes repeated turns under [round-robin scheduling](#round-robin-scheduling) possible. Saving an [execution context](#execution-context) does not copy the entire [address space](virtual-memory.md#address-space). Switching between [software threads](#thread-computing) of one [operating-system process](#process-computing) can retain the same [address space](virtual-memory.md#address-space); switching between [operating-system processes](#process-computing) with different [address spaces](virtual-memory.md#address-space) may also require changing the [memory management unit](virtual-memory.md#memory-management-unit)'s translation context, such as the active [page table](virtual-memory.md#page-table) and associated [address space identifier](virtual-memory.md#address-space-identifier), depending on the architecture. Their contents remain in [computer memory](computer-science.md#computer-memory). [Remzi H. Arpaci-Dusseau and Andrea C. Arpaci-Dusseau, Operating Systems: Three Easy Pieces, chapter 26, introduction: thread contexts and shared address spaces](https://pages.cs.wisc.edu/~remzi/OSTEP/threads-intro.pdf)

Entering the [operating-system kernel](#kernel-operating-system) through an [interrupt](#interrupt), [synchronous processor exception](#synchronous-processor-exception) or [system call](#system-call) does not automatically imply a [context switch](#context-switch) to another task. The handler may return to the same task; [process scheduling](#process-scheduling) determines whether another runnable task should take over. A [context switch](#context-switch) consumes time, and a changed [memory cache](computer-science.md#cache-computing) or [translation lookaside buffer](virtual-memory.md#translation-lookaside-buffer) working environment can add subsequent costs. Those costs are excluded from the toy [process scheduling](#process-scheduling) timelines, which are calculations rather than [operating system](operating-system.md) benchmarks. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 6, section 6.3: continue the current process or switch](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-mechanisms.pdf)[Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 7, section 7.7: direct and indirect switching costs](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-sched.pdf)

#### Execution context

↑ **Parent:** [Context switch](#context-switch)

State needed to resume a suspended execution stream, including saved [processor registers](computer-science.md#processor-register) and its position in a [call stack](data-structure.md#call-stack). An [operating-system kernel](#kernel-operating-system) can keep parts in a per-task record and parts on a kernel [call stack](data-structure.md#call-stack). An [execution context](#execution-context) identifies and preserves that stream's state; it is not a duplicate of all the [computer memory](computer-science.md#computer-memory) reachable through its [address space](virtual-memory.md#address-space).

// Target: computer-science.bigb

## Process (computing)

↑ **Parent:** [Operating system](operating-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Process_(computing))

An [operating-system process](#process-computing) is an execution instance of a program, with an [address space](virtual-memory.md#address-space), one or more [software threads](#thread-computing) carrying [execution contexts](#execution-context), and [operating system](operating-system.md) resources such as [file descriptors](#file-descriptor). A program describes instructions; an executable [file](file-system.md#computer-file) stores a form that can be loaded for execution. Starting the same executable twice can create two [operating-system processes](#process-computing), each with its own evolving state. A [operating-system process](#process-computing) can be waiting for [input-output](computer-science.md#input-output) or waiting for a turn on the [CPU](computer-science.md#central-processing-unit), rather than executing at every instant. [Remzi H. Arpaci-Dusseau and Andrea C. Arpaci-Dusseau, Operating Systems: Three Easy Pieces, chapter 4, sections 4.1, 4.3–4.4: program, process and execution states](https://pages.cs.wisc.edu/~remzi/OSTEP/cpu-intro.pdf)

For example, start the same counter program as [operating-system processes](#process-computing) A and B. In this toy mapping, both use [virtual address](virtual-memory.md#virtual-address) `0x1234` for a counter `x`, but A reads `x = 7` while B reads `x = 42`. The number `0x1234` is interpreted through the current [address space](virtual-memory.md#address-space), so it need not denote the same contents in both [operating-system processes](#process-computing). Writing A's ordinary private counter does not change B's counter. Compare [virtual memory](virtual-memory.md) for an explicit mapping to different [physical addresses](computer-science.md#physical-address).

<a id="image-separate-operating-system-processes-can-interpret-the-same-virtual-address-differently-software-threads-in-one-process-share-an-address-space"></a>
![](process-and-thread-address-spaces.png)

**[Figure 6](#image-separate-operating-system-processes-can-interpret-the-same-virtual-address-differently-software-threads-in-one-process-share-an-address-space). Separate operating-system processes can interpret the same virtual address differently; software threads in one process share an address space**.

Separate [virtual memory](virtual-memory.md) [address spaces](virtual-memory.md#address-space) provide a usual default isolation boundary, not a claim that all [computer memory](computer-science.md#computer-memory) is universally private. Deliberately shared mappings let [operating-system processes](#process-computing) communicate through the same stored data. Even logically private contents need not occupy distinct [page frames](virtual-memory.md#page-frame) at every moment: read-only program code can be shared, and [copy-on-write](virtual-memory.md#copy-on-write) can keep a common [memory page](virtual-memory.md#memory-page) until a write requires a private copy. The distinction is between which accesses and changes are permitted and which physical storage is currently reused. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 23, section 23.1, Other Neat Tricks: copy-on-write and shared mappings](https://pages.cs.wisc.edu/~remzi/OSTEP/vm-complete.pdf)[The Open Group, POSIX shared-memory object interface, shm\_open: multiple processes can refer to the same shared memory object](https://pubs.opengroup.org/onlinepubs/009695099/functions/shm_open.html)

This abstraction lets independent activities reuse the same executable while keeping their changing state separate. [Process scheduling](#process-scheduling) distributes [CPU](computer-science.md#central-processing-unit) time; [virtual memory](virtual-memory.md) interprets and protects addresses; [file descriptors](#file-descriptor) connect an execution to open resources. The useful design is controlled independence with explicit ways to share. Creating [operating-system processes](#process-computing), maintaining their mappings and performing [context switches](#context-switch) require time and [computer memory](computer-science.md#computer-memory); isolation alone gives no universal performance guarantee.

### File descriptor

↑ **Parent:** [Process (computing)](#process-computing)

A nonnegative [integer](integer.md) identifying an open access in one [operating-system process](#process-computing). The program passes its value to operations such as reading and closing; the [operating-system kernel](#kernel-operating-system) interprets it through that [operating-system process](#process-computing)'s descriptor table. In the toy example, table entry `3` refers to an [open file description](#open-file-description) for [inode](file-system.md#inode) 42. Another [operating-system process](#process-computing)'s entry `3` can reach a different [file](file-system.md#computer-file), and a closed [file descriptor](#file-descriptor) value can be reused. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 39, section 39.3: per-process file descriptors](https://pages.cs.wisc.edu/~remzi/OSTEP/file-intro.pdf)

#### Open file description

↑ **Parent:** [File descriptor](#file-descriptor)

A record of an open access to a [file](file-system.md#computer-file), including its current position and access mode. Each [file descriptor](#file-descriptor) reaches one [open file description](#open-file-description), but several [file descriptors](#file-descriptor) can share it. Separately opening the same ordinary [file](file-system.md#computer-file) creates separate [open file descriptions](#open-file-description) with independent positions while still reaching the same [inode](file-system.md#inode). Thus [file descriptors](#file-descriptor), [open file descriptions](#open-file-description) and [hard links](file-system.md#hard-link) have different counts. [The Open Group, POSIX.1-2017, section 3.258: open file description](https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_258)

// Target: computer-science.bigb

### Thread (computing)

↑ **Parent:** [Process (computing)](#process-computing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Thread_(computing))

A [software thread](#thread-computing) is an execution stream within a [operating-system process](#process-computing). Each [software thread](#thread-computing) has its own [execution context](#execution-context), including [processor registers](computer-science.md#processor-register), an [instruction pointer](computer-science.md#instruction-pointer), and a [call stack](data-structure.md#call-stack) selected by its [stack pointer](computer-science.md#stack-pointer). [Software threads](#thread-computing) in the same [operating-system process](#process-computing) share its [address space](virtual-memory.md#address-space), global variables, dynamically allocated storage (the memory heap), and resources such as [file descriptors](#file-descriptor). Separate register states let two [software threads](#thread-computing) pause at different instructions and later resume correctly. A [context switch](#context-switch) saves and restores those states; it does not copy the entire shared [address space](virtual-memory.md#address-space). [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 26, introduction and figure 26.1: thread contexts and shared address space](https://pages.cs.wisc.edu/~remzi/OSTEP/threads-intro.pdf)[The Open Group, POSIX.1-2024, sections 3.189–3.190: Live Process and Live Thread, shared resources and addressable storage](https://pubs.opengroup.org/onlinepubs/9799919799/basedefs/V1_chap03.html#tag_03_189)

In the right half of the diagram under [operating-system process](#process-computing), T1 and T2 access the same counter `x` at [virtual address](virtual-memory.md#virtual-address) `0x1234`. Their [call stacks](data-structure.md#call-stack) occupy separate regions of the same [address space](virtual-memory.md#address-space), and their saved [processor registers](computer-science.md#processor-register) can contain different values. A [software thread](#thread-computing)'s own [call stack](data-structure.md#call-stack) means the stack used for its calls, not a hardware protection boundary against another [software thread](#thread-computing). Another [software thread](#thread-computing) with a suitable address can access that stack's live data, subject to the program's lifetime and [synchronization](#synchronization-computing) rules. Sharing an [address space](virtual-memory.md#address-space) enables easy communication and makes accidental interference possible.

Concurrency means that several activities can make progress over overlapping intervals; parallel execution means that several activities execute at the same instant. On one [CPU](computer-science.md#central-processing-unit) execution slot, [process scheduling](#process-scheduling) can interleave [software threads](#thread-computing) without simultaneous execution. Multiple processor cores can run eligible [software threads](#thread-computing) in parallel, but merely creating [software threads](#thread-computing) does not ensure parallel execution or a speedup.

Consider an explicitly abstract interleaving model: shared `x` starts at $0$, and each of T1 and T2 performs three indivisible logical steps in its own order: load `x` into its own register `r`, add $1$ to `r`, then store `r` into `x`. Each load sees the latest preceding store in the displayed order. These model assumptions specify the example; they do not describe every programming language or every hardware memory model. In serial order T1 finishes all three steps before T2 starts, so T2 loads $1$ and stores $2$.

An overlapping order instead gives T1 load $0$, T2 load $0$, T1 add to get `r1 = 1`, T2 add to get `r2 = 1`, T1 store $1$, and T2 store $1$. The load/store subsequence is therefore T1 load $0$, T2 load $0$, T1 store $1$, T2 store $1$: final $x=1$, although each [software thread](#thread-computing) incremented its register correctly. The second store replaces the first with the same value, losing one intended update. This [race condition](#race-condition) is possible even with interleaving on a single [CPU](computer-science.md#central-processing-unit).

<a id="image-two-abstract-load-add-store-increments-retain-separate-registers-but-can-leave-the-shared-counter-at-1-instead-of-the-serial-result-2"></a>
![](thread-lost-update-interleaving.png)

**[Figure 7](#image-two-abstract-load-add-store-increments-retain-separate-registers-but-can-leave-the-shared-counter-at-1-instead-of-the-serial-result-2). Two abstract load/add/store increments retain separate registers but can leave the shared counter at $1$ instead of the serial result $2$**.

This is not an unprotected C implementation example. Conflicting unsynchronized accesses to an ordinary non-atomic C object from different [software threads](#thread-computing) can constitute a data race, which has undefined behavior; the abstract trace is not a prediction of that program's allowed outcomes. [ISO/IEC JTC1/SC22/WG14, committee draft N1570, 12 April 2011, section 5.1.2.4 paragraph 25: data races and undefined behavior](https://www.open-std.org/jtc1/sc22/wg14/www/docs/n1570.pdf)

The repair explains why [synchronization](#synchronization-computing) matters: [mutual exclusion](#mutual-exclusion) around the whole load/add/store sequence prevents the other [software thread](#thread-computing) from starting an increment halfway through it. Alternatively, an appropriate [atomic operation](#atomic-operation) can make the complete increment one indivisible read-modify-write. In the toy model, either repair makes the two increments take effect in an order, producing $0+1+1=2$. Making only each load and each store an [atomic operation](#atomic-operation) still permits the displayed lost update. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 28, sections 28.1–28.2 and 28.11: locks around updates and atomic fetch-and-add](https://pages.cs.wisc.edu/~remzi/OSTEP/threads-locks.pdf)

The attraction is independently progressing activities with direct access to shared data: a user-interface [software thread](#thread-computing) can handle input while another waits for [input-output](computer-science.md#input-output), and workers can divide independent pieces of a large calculation among available cores. The first benefit can exist on one [CPU](computer-science.md#central-processing-unit); the second requires suitable work and execution resources. [Context switches](#context-switch), [synchronization](#synchronization-computing), register-state records and extra [call stacks](data-structure.md#call-stack) consume time or [computer memory](computer-science.md#computer-memory), so the useful partition depends on the workload. [Arpaci-Dusseau and Arpaci-Dusseau, OSTEP chapter 26, section 26.1: parallel work and overlapping input-output with other activity](https://pages.cs.wisc.edu/~remzi/OSTEP/threads-intro.pdf)

#### Race condition

↑ **Parent:** [Thread (computing)](#thread-computing)

A dependence of behavior on the relative timing or ordering of concurrent activities. In the abstract example under [software thread](#thread-computing), two increments can leave $x=1$ or $x=2$ depending on their interleaving. A C data race is a language-defined conflict with undefined behavior, rather than a name for every [race condition](#race-condition).

#### Synchronization (computing)

↑ **Parent:** [Thread (computing)](#thread-computing)

Coordinating concurrent activities so that required ordering and visibility rules hold. [Mutual exclusion](#mutual-exclusion) is one form of [synchronization](#synchronization-computing); waiting for another [software thread](#thread-computing) to finish is another.

##### Mutual exclusion

↑ **Parent:** [Synchronization (computing)](#synchronization-computing)

[Mutual exclusion](#mutual-exclusion) allows at most one participating [software thread](#thread-computing) at a time to execute a protected [critical section](#critical-section). A [mutex](#mutex) is an object used to enforce that rule; the [critical section](#critical-section) is the region of the program that needs the rule. Several different [critical sections](#critical-section) can use the same [mutex](#mutex) to protect the same shared data. The benefit is reasoning about a complete update without another cooperating [software thread](#thread-computing) observing or changing its intermediate state.[pp. 1–2: lock ownership and critical sections](computer-science-bibliography.md#operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/locks)

For a small [lost update](#lost-update), shared `x` initially equals $0$. Each of two [software threads](#thread-computing), T1 and T2, uses its own local `r` and performs these three steps:
```
r = read(x)
r = r + 1
write(x, r)
```
Assume [sequential consistency](#sequential-consistency): each step is indivisible, each [software thread](#thread-computing) keeps the displayed order, and a read sees the latest preceding write to `x`. In the [thread interleaving](#thread-interleaving) T1 read, T2 read, T1 add, T2 add, T1 write, T2 write, both local values become $1$ and both writes store $1$. Final $x=1$ instead of $2$: a [lost update](#lost-update) despite two correctly executed local additions. Separate indivisible reads and writes are insufficient; the complete read, modify and write must be protected.

<a id="image-a-lost-update-and-its-repair-by-mutual-exclusion-around-the-complete-increment"></a>
![](mutual-exclusion-lost-update-timelines.png)

**[Figure 8](#image-a-lost-update-and-its-repair-by-mutual-exclusion-around-the-complete-increment). A lost update and its repair by mutual exclusion around the complete increment**.

The [binomial coefficient](binomial-coefficient.md) $\binom{6}{3}=20$ counts the [thread interleavings](#thread-interleaving) preserving the two three-step orders: choose T1's three positions, with the remaining positions belonging to T2. Exhaustive enumeration gives final $x=1$ in 18 orders and $x=2$ in the two serial orders. These counts are not probabilities: no random scheduler has been specified. With the same [mutex](#mutex) acquired before reading and released after writing, only the two complete increment orders remain, and both give $2$. Alternatively, an [atomic read-modify-write](#atomic-read-modify-write) increment updates `x` in one indivisible step. Protecting only the write still allows both [software threads](#thread-computing) to read $0$ beforehand.

[Mutual exclusion](#mutual-exclusion) is a [safety property](#safety-property): two participants must never be inside the protected [critical section](#critical-section) together. Eventual entry for every persistent requester is a [liveness property](#liveness-property), expressed here as [starvation freedom](#starvation-freedom). A protocol that never admits anyone satisfies the first requirement while failing the second. Nor does a [mutex](#mutex) alone promise which waiting [software thread](#thread-computing) enters next, or that a producer runs before a consumer. Such application ordering needs an additional [synchronization](#synchronization-computing) protocol.[pp. 181–182: mutual exclusion, finite witnesses to safety violations, and eventual service](computer-science-bibliography.md#defining-liveness-by-bowen-alpern-and-others)

The [sequential consistency](#sequential-consistency) assumptions delimit this calculation. In C++, unsynchronized conflicting accesses to an ordinary shared object can be a [data race](#data-race), which makes behavior undefined; the 20 schedules are not a prediction for that program. An [atomic operation](#atomic-operation) with relaxed ordering also supplies no [acquire-release synchronization](#acquire-release-synchronization) for other data. A real [mutex](#mutex) must supply both exclusive entry and the required [happens-before](#happens-before) ordering between its users.[Working Draft, Standard for Programming Language C++ (N4861)](computer-science-bibliography.md#working-draft-standard-for-programming-language-c-plus-plus-n4861)

###### Critical section

↑ **Parent:** [Mutual exclusion](#mutual-exclusion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Critical_section)

A region whose accesses must obey a shared [synchronization](#synchronization-computing) protocol. For the [lost update](#lost-update) in [mutual exclusion](#mutual-exclusion), the [critical section](#critical-section) includes the read and the local addition as well as the write. Choosing its boundary means identifying the complete operation whose intermediate state must be protected. Every conflicting access must participate in a compatible protocol; merely declaring a [mutex](#mutex) does not protect accesses that bypass it.

###### Mutex

↑ **Parent:** [Mutual exclusion](#mutual-exclusion)

An object with acquire and release operations that provides exclusive ownership to a participating [software thread](#thread-computing). Several source-code regions can acquire the same [mutex](#mutex); two different [mutex](#mutex) objects do not exclude each other's users. The caller should enter its [critical section](#critical-section) only after successful acquisition and release ownership on every exit path. A [mutex](#mutex) may make a waiting [software thread](#thread-computing) sleep or use a [spinlock](#spinlock); the interface and the waiting mechanism are distinct.[Locks](computer-science-bibliography.md#operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/locks)

###### Spinlock

↑ **Parent:** [Mutex](#mutex)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Spinlock)

A mechanism that waits for ownership by repeatedly trying while consuming [CPU](computer-science.md#central-processing-unit) execution time. A [spinlock](#spinlock) built from [test-and-set](#test-and-set) can enforce [mutual exclusion](#mutual-exclusion) without guaranteeing [starvation freedom](#starvation-freedom). Progress also requires the owner to run and release: if a waiting [software thread](#thread-computing) monopolizes the only [CPU](computer-science.md#central-processing-unit) while the owner is suspended, exclusive entry alone cannot help.[pp. 8–9: preemption requirement and lack of fairness guarantees](computer-science-bibliography.md#operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/locks)

###### Test-and-set

↑ **Parent:** [Spinlock](#spinlock)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Test-and-set)

An [atomic read-modify-write](#atomic-read-modify-write) that returns a flag's old value while setting it. In a [sequential consistency](#sequential-consistency) model with the flag initially $0$, `exchange(flag, 1)` permits entry only when it returns $0$; an owner resets the flag to $0$ on release. Between releases only one exchange can observe $0$. By contrast, separate `read(flag)` and `write(flag, 1)` steps allow both contenders to read $0$ before either writes $1$. The indivisibility of the exchange is an assumed primitive, not something proved by writing its steps as ordinary assignments.[Locks](computer-science-bibliography.md#operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/locks)

###### Thread interleaving

↑ **Parent:** [Mutual exclusion](#mutual-exclusion)

An ordered execution obtained by mixing steps of several [software threads](#thread-computing) while retaining each one's own step order. In the [sequential consistency](#sequential-consistency) model of [mutual exclusion](#mutual-exclusion), an indivisible step finishes before the next begins. Selecting the step boundaries is part of the model: an [atomic read-modify-write](#atomic-read-modify-write) increment has one boundary, whereas a separate read, local addition and write have three. Enumerating all such orders checks this specified model, not an arbitrary [memory model](#memory-model) or a real [mutex](#mutex) implementation.

###### Lost update

↑ **Parent:** [Thread interleaving](#thread-interleaving)

A change that is overwritten by another update based on an older value. In [mutual exclusion](#mutual-exclusion), both [software threads](#thread-computing) read $0$ and later write $1$, so one intended increment is lost. This [race condition](#race-condition) can occur with individually atomic reads and writes and therefore need not involve a [data race](#data-race). Its repair must cover the complete update, using a [critical section](#critical-section) or an appropriate [atomic read-modify-write](#atomic-read-modify-write).

##### Safety property

↑ **Parent:** [Synchronization (computing)](#synchronization-computing)

A requirement whose violation has a finite execution prefix that no continuation can repair. Two [software threads](#thread-computing) simultaneously inside a protected [critical section](#critical-section) already violate [mutual exclusion](#mutual-exclusion); later leaving does not erase that violation. This contrasts with a [liveness property](#liveness-property), for which a long finite wait alone does not establish failure.[pp. 181–182: finite irremediable prefixes](computer-science-bibliography.md#defining-liveness-by-bowen-alpern-and-others)

##### Liveness property

↑ **Parent:** [Synchronization (computing)](#synchronization-computing)

A requirement of eventual progress, with no finite prefix ruling out its eventual satisfaction. For [starvation freedom](#starvation-freedom), a persistent requester must eventually enter its [critical section](#critical-section). Establishing such a [liveness property](#liveness-property) requires explicit scheduling and protocol assumptions in addition to [mutual exclusion](#mutual-exclusion). Exhaustive finite [thread interleaving](#thread-interleaving) checks alone do not establish eventual service for repeatedly competing [software threads](#thread-computing).[p. 182: every finite prefix can still be extended to satisfy a liveness property](computer-science-bibliography.md#defining-liveness-by-bowen-alpern-and-others)

###### Starvation freedom

↑ **Parent:** [Liveness property](#liveness-property)

For acquisition of a [mutex](#mutex), the guarantee that every persistent requester eventually succeeds, under specified scheduling assumptions and with owners eventually releasing. Some [software threads](#thread-computing) repeatedly succeeding while another waits forever violates [starvation freedom](#starvation-freedom) without violating [mutual exclusion](#mutual-exclusion). A finite bound on the wait, and service in arrival order, are additional requirements.

##### Deadlock

↑ **Parent:** [Synchronization (computing)](#synchronization-computing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Deadlock)

A group of participants cannot proceed because each waits for a resource whose release depends on another participant in the group. Consider two initially free [mutex](#mutex) objects A and B. T1 acquires A then tries B; T2 acquires B then tries A. If each obtains its first [mutex](#mutex), both wait permanently for the other, with release reachable only after the second acquisition. Each [mutex](#mutex) still enforces [mutual exclusion](#mutual-exclusion).[pp. 5–7, figures 32.6–32.7: opposing acquisition orders and circular wait](computer-science-bibliography.md#operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/common-concurrency-problems)

<a id="image-reachable-states-for-opposite-mutex-acquisition-orders-and-for-one-shared-lock-ordering"></a>
![](mutual-exclusion-lock-order-state-space.png)

**[Figure 9](#image-reachable-states-for-opposite-mutex-acquisition-orders-and-for-one-shared-lock-ordering). Reachable states for opposite mutex acquisition orders and for one shared lock ordering**.

Each [software thread](#thread-computing) performs four indivisible operations: acquire its first [mutex](#mutex), acquire its second, release the second, release the first. An unavailable acquisition blocks; neither participant releases early. A state records each participant's completed-operation count and both owners. Exhaustive exploration finds 19 reachable states with opposite orders, including exactly one nonterminal state with no enabled operation: both counts are $1$, T1 owns A, and T2 owns B. Giving both participants the order A then B leaves 16 reachable states and no such blocked state. Unshown grid positions are unreachable. These are tiny [sequential consistency](#sequential-consistency) models, without timeouts, cancellation, recursive acquisition or other resources.

###### Deadlock freedom

↑ **Parent:** [Deadlock](#deadlock)

Absence of a reachable [deadlock](#deadlock). In the finite acquisition model under [deadlock](#deadlock), reaching a nonterminal state with no enabled operation is a finite witness to failure, so this formulation is a [safety property](#safety-property). Sometimes the phrase is used for eventual acquisition by some requester, a [liveness property](#liveness-property); the intended requirement must be stated. Neither formulation by itself promises [starvation freedom](#starvation-freedom) for every requester.

###### Lock ordering

↑ **Parent:** [Deadlock](#deadlock)

A shared order governing acquisition of distinct [mutex](#mutex) objects. To prevent circular waiting, choose a strict [total order](set.md#total-order) and acquire only a higher-ranked [mutex](#mutex) while retaining lower-ranked ones. In the two-object [deadlock](#deadlock) example, every participant acquires A before B. An outline of the argument is that ranks would strictly increase around any alleged waiting cycle, yet return to the starting rank, a contradiction. The rule must include acquisitions hidden inside called routines. It excludes this kind of [deadlock](#deadlock), not arbitrary waiting on other resources or failure to schedule an owner.[pp. 7–8: consistent acquisition ordering and hidden calls](computer-science-bibliography.md#operating-systems-three-easy-pieces-by-remzi-h-arpaci-dusseau-and-others/common-concurrency-problems)

##### Memory model

↑ **Parent:** [Synchronization (computing)](#synchronization-computing)

Rules specifying which shared-data observations and operation orders are allowed. [Sequential consistency](#sequential-consistency) is the model used in the two diagrams. A language [memory model](#memory-model) can permit weaker ordering and impose additional conditions on conflicting accesses. Correct use of an indivisible flag must therefore be checked against that [memory model](#memory-model), including [happens-before](#happens-before) relationships for the data guarded by the flag.

###### Sequential consistency

↑ **Parent:** [Memory model](#memory-model)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sequential_consistency)

Execution behaves as if steps occurred in one [total order](set.md#total-order) preserving each participant's program order; reads observe the latest preceding writes in that order. This is the definition given in the 1979 paper [How to Make a Multiprocessor Computer That Correctly Executes Multiprocess Programs](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/12/How-to-Make-a-Multiprocessor-Computer-That-Correctly-Executes-Multiprocess-Programs.pdf), printed p. 690. It permits many [thread interleavings](#thread-interleaving), including the [lost update](#lost-update) under [mutual exclusion](#mutual-exclusion); ordering individual accesses does not combine them into one [atomic operation](#atomic-operation).

###### Data race

↑ **Parent:** [Memory model](#memory-model)

For the C++ case used here, conflicting accesses by different [software threads](#thread-computing), at least one non-atomic, with neither ordered before the other by [happens-before](#happens-before). Such a [data race](#data-race) has undefined behavior. A [race condition](#race-condition) is broader: the [lost update](#lost-update) with separate atomic reads and writes depends on their order while avoiding a [data race](#data-race).[pp. 79–80: conflicting actions and undefined behavior](computer-science-bibliography.md#working-draft-standard-for-programming-language-c-plus-plus-n4861)

###### Happens-before

↑ **Parent:** [Memory model](#memory-model)

An ordering [binary relation](set-theory.md#binary-relation) used by a [memory model](#memory-model) to constrain observation of shared data. For the [mutex](#mutex) example, T1's write precedes its release, that release synchronizes with T2's successful acquisition, and that acquisition precedes T2's read. Together these steps order the write before the read. Wall-clock timing alone does not establish [happens-before](#happens-before).[Working Draft, Standard for Programming Language C++ (N4861)](computer-science-bibliography.md#working-draft-standard-for-programming-language-c-plus-plus-n4861)

###### Acquire-release synchronization

↑ **Parent:** [Happens-before](#happens-before)

A release on an atomic object can synchronize with an acquire that reads the released value, establishing [happens-before](#happens-before) for surrounding accesses. A [test-and-set](#test-and-set) [spinlock](#spinlock) needs suitable acquisition and release semantics for its guarded data; relaxed flag operations alone do not supply that relationship. This is a separate question from the flag's indivisibility.[pp. 1524–1525: relaxed ordering and release/acquire synchronization](computer-science-bibliography.md#working-draft-standard-for-programming-language-c-plus-plus-n4861)

##### Atomic operation

↑ **Parent:** [Synchronization (computing)](#synchronization-computing)

An operation that takes effect indivisibly relative to the specified competing accesses. An atomic increment protects the whole read-modify-write; separate atomic loads and stores do not make their combined sequence an [atomic operation](#atomic-operation).

// Target: computer-science.bigb

###### Atomic read-modify-write

↑ **Parent:** [Atomic operation](#atomic-operation)

An [atomic operation](#atomic-operation) that reads a shared object's value and changes it as one indivisible action. For an increment from $0$, the two operations under [mutual exclusion](#mutual-exclusion) produce $1$ then $2$ in either [software thread](#thread-computing) order. A [test-and-set](#test-and-set) is another example. The operation's ordering guarantees for other data still depend on the [memory model](#memory-model) and its selected [acquire-release synchronization](#acquire-release-synchronization) semantics.

## ↑ Ancestors (2)

1. [Computer science](computer-science.md)
2. [Codex Wiki](README.md)

## ← Incoming links (33)

- [Address translation](virtual-memory.md#address-translation)
- [Computer file](file-system.md#computer-file)
- [Context switch](#context-switch)
- [Copy-on-write](virtual-memory.md#copy-on-write)
- [Copy-on-write fault handling](virtual-memory.md#copy-on-write-fault-handling)
- [Device driver](#device-driver)
- [Interrupt](#interrupt)
- [Interrupt-driven input-output](#interrupt-driven-input-output)
- [Kernel (operating system)](#kernel-operating-system)
- [Linux kernel](#linux-kernel)
- [Memory management unit](virtual-memory.md#memory-management-unit)
- [Memory-mapped file](virtual-memory.md#memory-mapped-file)
- [Operating system](operating-system.md)
- [Optimal page replacement](virtual-memory.md#optimal-page-replacement)
- [Page cache](file-system.md#page-cache)
- [Page fault](virtual-memory.md#page-fault)
- [Page-replacement cost accounting](virtual-memory.md#page-replacement-cost-accounting)
- [Page table](virtual-memory.md#page-table)
- [Page table walk](virtual-memory.md#page-table-walk)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5.md#7/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5.md#7/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5.md#8/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5.md#7/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-5.md#8/c/ii/solution)
- [Process (computing)](#process-computing)
- [Sv39 page table](virtual-memory.md#sv39-page-table)
- [System call](#system-call)
- [Translation lookaside buffer](virtual-memory.md#translation-lookaside-buffer)
- [Two-level address translation](virtual-memory.md#two-level-address-translation)
- [User-space service](#user-space-service)
- [Virtual memory](virtual-memory.md)
- [Working set](virtual-memory.md#working-set)
