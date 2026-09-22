# Round-robin scheduling

↑ **Parent:** [Process scheduling](process-scheduling.md)

Serve the front of a [FIFO queue](fifo-queue.md) of runnable tasks for at most one [scheduling quantum](scheduling-quantum.md). If the task finishes or must wait for [input-output](input-output.md), it leaves the [CPU](central-processing-unit.md) earlier; if it remains runnable after consuming its allowance, append it to the rear of the [ready queue](ready-queue.md). In the example under [process scheduling](process-scheduling.md), the [ready queue](ready-queue.md) at time 2 is B, C, A: B arrived at time 1, C joins at the boundary, then A is requeued. That one convention determines the subsequent order.

**Table of contents**

- [Scheduling quantum](scheduling-quantum.md)

## ↑ Ancestors (4)

1. [Process scheduling](process-scheduling.md)
2. [Operating system](operating-system-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Context switch](context-switch.md)
- [CPU burst](cpu-burst.md)
- [Process scheduling](process-scheduling.md)
- [Ready queue](ready-queue.md)
- [Scheduling preemption](scheduling-preemption.md)
- [Scheduling quantum](scheduling-quantum.md)
- [Scheduling response time](scheduling-response-time.md)
- [Scheduling turnaround time](scheduling-turnaround-time.md)
- [Scheduling waiting time](scheduling-waiting-time.md)
