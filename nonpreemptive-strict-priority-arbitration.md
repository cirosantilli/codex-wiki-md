# Nonpreemptive strict-priority arbitration

↑ **Parent:** [Process scheduling](process-scheduling.md)

At each service decision, choose the highest-priority pending request, preserving [FIFO queue](fifo-queue.md) order within a priority class. A running owner retains the resource until it releases it; a higher-priority arrival changes the next choice rather than interrupting current work. Two priority classes can be represented by two [FIFO queues](fifo-queue.md), consulting the urgent one first.

This policy preserves the ownership safety argument of a [message-passing mutual exclusion server](message-passing-mutual-exclusion-server.md). It does not by itself give [starvation freedom](starvation-freedom.md) to lower-priority requests when higher-priority traffic can continue indefinitely. Priority is evaluated on requests known to the arbiter at the decision point; a message not yet received cannot influence that decision.

## ↑ Ancestors (4)

1. [Process scheduling](process-scheduling.md)
2. [Operating system](operating-system-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [LIFO starvation](lifo-starvation.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/2/b/solution.md)
