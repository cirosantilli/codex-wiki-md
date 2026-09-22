# Shared interrupt demultiplexing

↑ **Parent:** [Interrupt handler](interrupt-handler.md)

When several devices share an [interrupt](interrupt.md), the handler examines each device's pending status and acknowledges every active source. Separate tests allow simultaneous requests to be serviced. A source becoming pending during the scan must cause another [interrupt](interrupt.md) or be found by a justified rescan; the necessary behaviour depends on the [interrupt controller](interrupt-controller.md) and device protocol.

## ↑ Ancestors (5)

1. [Interrupt handler](interrupt-handler.md)
2. [Interrupt](interrupt.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/2/b/solution.md)
