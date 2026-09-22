# Synchronous send-and-receive

↑ **Parent:** [Synchronous message passing](synchronous-message-passing.md)

A [system call](system-call.md) that sends a request and commits the caller to receiving the matching reply as one coordinated operation, often named `sendrec`. It avoids the gap in which a client has completed a send but has not yet entered a receive. It does not make the service nonblocking or eliminate [deadlock](deadlock.md) caused by other circular dependencies.

## ↑ Ancestors (8)

1. [Synchronous message passing](synchronous-message-passing.md)
2. [Message passing](message-passing.md)
3. [Synchronization (computing)](synchronization-computing.md)
4. [Thread (computing)](thread-computing.md)
5. [Process (computing)](process-computing.md)
6. [Operating system](operating-system-split.md)
7. [Computer science](computer-science-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof-resit/2/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/3/c/solution.md)
- [Synchronous message passing](synchronous-message-passing.md)
