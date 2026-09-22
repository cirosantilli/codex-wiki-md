# Interrupt-safe ring-buffer snapshot

↑ **Parent:** [Circular buffer](circular-buffer.md)

When an [interrupt handler](interrupt-handler.md) is the sole writer of a fixed [ring buffer](circular-buffer.md), foreground code can obtain a coherent view by saving and masking the relevant interrupt, copying the count and valid entries, and restoring the earlier mask. Perform expensive calculations on the copy after leaving the [critical section](critical-section.md). Exclusion prevents the writer from changing the logical version during the copy; individually atomic loads alone do not give this guarantee. Correctness also requires compiler ordering at the boundaries, no unmasked competing writer, and a short enough mask interval that the peripheral does not lose events. Restoring the previous mask avoids accidentally enabling an interrupt disabled by an outer caller.

## ↑ Ancestors (4)

1. [Circular buffer](circular-buffer.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/2/b/solution.md)
