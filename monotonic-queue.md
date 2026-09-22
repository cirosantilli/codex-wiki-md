# Monotonic queue

↑ **Parent:** [Double-ended queue](double-ended-queue.md)

A monotonic queue keeps candidate values in sorted order while a window moves through a sequence. For window maxima, discard smaller or equal values from the back before appending a new value, and remove expired indices from the front. The maximum is always at the front. Each index enters and leaves at most once, so all windows can be processed in linear time.

## ↑ Ancestors (4)

1. [Double-ended queue](double-ended-queue.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
