# Circular buffer

↑ **Parent:** [Data structure](data-structure-split.md)

A [circular buffer](circular-buffer.md) stores a changing [sequence](sequence.md) in a fixed-capacity [array](array-data-structure.md), reusing slots by wrapping [array indices](array-index.md) through [modular arithmetic](modular-arithmetic-split.md). A front [array index](array-index.md) and an occupied count can represent a [FIFO queue](fifo-queue.md) without shifting entries after removal. The physical [array](array-data-structure.md) stays in place; the position at which its logical [sequence](sequence.md) begins moves. This makes a [circular buffer](circular-buffer.md) useful when storage must remain bounded while successive items arrive and leave.

Capacity and overflow behavior are separate choices. A rejecting [FIFO queue](fifo-queue.md) preserves all accepted items until removal and reports failure on a full insertion. An overwriting [circular buffer](circular-buffer.md) deliberately discards its oldest item to retain the newest arrivals. These are different [application programming interfaces](application-programming-interface.md). The existing [representation independence](representation-independence.md) example specifies the rejecting policy and gives its [abstraction function](abstraction-function.md) and correctness argument against a shifting [array](array-data-structure.md) implementation.

**Table of contents**

- [Circular buffer indices](circular-buffer-indices.md)
- [Circular buffer full and empty states](circular-buffer-full-and-empty-states.md)
- [Circular buffer operation trace](circular-buffer-operation-trace.md)
- [Circular buffer overflow policy](circular-buffer-overflow-policy.md)
- [Circular buffer operation costs](circular-buffer-operation-costs.md)

## ↑ Ancestors (3)

1. [Data structure](data-structure-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Circular buffer](circular-buffer.md)
- [Circular buffer full and empty states](circular-buffer-full-and-empty-states.md)
- [Circular buffer indices](circular-buffer-indices.md)
- [Circular buffer operation costs](circular-buffer-operation-costs.md)
- [Circular buffer overflow policy](circular-buffer-overflow-policy.md)
- [Representation independence](representation-independence.md)
