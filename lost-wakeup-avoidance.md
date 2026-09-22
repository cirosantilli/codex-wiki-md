# Lost-wakeup avoidance

↑ **Parent:** [Interrupt-driven input-output](interrupt-driven-input-output.md)

A completion can occur after a device is started but before its driver begins waiting. Preserve that completion in a pending notification or use an atomic condition-check-and-wait operation. Establish the interrupt route before starting the device, and clear stale status before the new start, not afterwards. Otherwise a fast completion can be erased and a completed request can wait indefinitely.

## ↑ Ancestors (5)

1. [Interrupt-driven input-output](interrupt-driven-input-output.md)
2. [Interrupt](interrupt.md)
3. [Operating system](operating-system-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof-resit/2/a/solution.md)
