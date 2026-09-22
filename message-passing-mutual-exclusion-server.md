# Message-passing mutual exclusion server

↑ **Parent:** [Mutual exclusion](mutual-exclusion.md)

Maintain an owner identity, initially empty, and a [FIFO queue](fifo-queue.md) of accepted client requests. A request appends its sender to the [FIFO queue](fifo-queue.md). A release from the owner clears the owner. Whenever there is no owner and the [FIFO queue](fifo-queue.md) is nonempty, remove its oldest request, record that client as owner, and send a grant. The server processes these state changes sequentially.

**Safety proof.** At most one grant is outstanding: a new grant requires an empty owner field, and a valid release clears precisely the preceding ownership. Compliant clients access the resource only while holding their grant, so [mutual exclusion](mutual-exclusion.md) follows. With reliable eventual [message passing](message-passing.md), continued server execution and finite resource-use durations, the [FIFO queue](fifo-queue.md) also gives [starvation freedom](starvation-freedom.md) for accepted requests, since later requests cannot overtake them.

## ↑ Ancestors (7)

1. [Mutual exclusion](mutual-exclusion.md)
2. [Synchronization (computing)](synchronization-computing.md)
3. [Thread (computing)](thread-computing.md)
4. [Process (computing)](process-computing.md)
5. [Operating system](operating-system-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Message passing](message-passing.md)
- [Nonpreemptive strict-priority arbitration](nonpreemptive-strict-priority-arbitration.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/2/a/solution.md)
