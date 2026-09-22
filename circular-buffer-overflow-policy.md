# Circular buffer overflow policy

↑ **Parent:** [Circular buffer](circular-buffer.md)

Continue from step 9 with a proposed insertion of $H$. A rejecting operation `try_enqueue(H)` returns `full`, writes nothing and leaves $(C,D,E,F,G)$ with $h=2,n=5,w=2$. The next `dequeue()` returns $C$, leaving $(D,E,F,G)$ with $h=3,n=4,w=2$. Rejection requires the caller to decide whether to retry or abandon $H$.

An overwriting operation `append_latest(H)` instead writes $B_h\leftarrow H$, advances $h\leftarrow(h+1)\bmod C$, and keeps $n=C$. It can report the discarded label $C$ as part of its specified result. At step 10 this gives $(D,E,F,G,H)$ with $h=3,n=5,w=3$. The next `dequeue()` returns $D$, leaving $(E,F,G,H)$ with $h=4,n=4,w=3$. Below full capacity, `append_latest` follows the ordinary insertion rule without discarding anything.

The lower bars in the trace diagram expose the consequence: $C$ entered at step 4 and remains a member until step 11 under rejection, but only until step 10 under overwrite. $H$ never becomes a member in the rejecting branch; it does in the overwriting branch. The same physical slot can therefore hold different logical items over time. These interfaces are observably different, so [representation independence](representation-independence.md) cannot justify exchanging them while retaining the same promised results.

Boost's documented `push_back` behavior chooses overwrite when full, implemented by assignment to the old element. Its discussion of iterator invalidation illustrates why a reused address need not still identify the original item. Assignment, object destruction, and release of an owned resource are separate language-level concerns; the membership bars make no claim about those lifetimes.[Jan Gaspar, Boost.Circular Buffer, Implementation: Overwrite Operation; Writing to a Full Buffer; Iterator Invalidation; Caveats](boost-circular-buffer-by-jan-gaspar/implementation.md)

A rejecting [FIFO queue](fifo-queue.md) suits work that must remain pending until explicitly removed. An overwriting [circular buffer](circular-buffer.md) suits a bounded recent history where losing the oldest retained item is the stated policy. Neither storage wrap nor bounded capacity chooses between those requirements.

## ↑ Ancestors (4)

1. [Circular buffer](circular-buffer.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
