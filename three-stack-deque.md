# Three-stack deque

↑ **Parent:** [Double-ended queue](double-ended-queue.md)

A [deque](double-ended-queue.md) can use two permanent [stacks](stack-data-structure.md) holding the front and back portions, plus an empty temporary [stack](stack-data-structure.md). When removal encounters an empty side, park the top half of the other side in the temporary [stack](stack-data-structure.md), reverse its remaining half into the empty side, and restore the parked half. This preserves order and balances the permanent [stacks](stack-data-structure.md). The [potential method](potential-method.md) with $\Phi=3\bigl||F|-|B|\bigr|$ pays for the [linear time](linear-time.md) transfer from the previous size imbalance, giving constant [amortized cost](amortized-cost.md) for all four endpoint operations with only a fixed number of size counters.

## ↑ Ancestors (4)

1. [Double-ended queue](double-ended-queue.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
