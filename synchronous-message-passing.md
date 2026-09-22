# Synchronous message passing

↑ **Parent:** [Message passing](message-passing.md)

A [message passing](message-passing.md) discipline in which a send completes only when a matching receive accepts the message. This rendezvous transfers both data and control dependencies: an unready recipient can block a service and thereby delay its other clients. A reply is a separate send unless the interface supplies [synchronous send-and-receive](synchronous-send-and-receive.md).

**Table of contents**

- [Synchronous send-and-receive](synchronous-send-and-receive.md)

## ↑ Ancestors (7)

1. [Message passing](message-passing.md)
2. [Synchronization (computing)](synchronization-computing.md)
3. [Thread (computing)](thread-computing.md)
4. [Process (computing)](process-computing.md)
5. [Operating system](operating-system-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Backpressure](backpressure.md)
- [Head-of-line blocking](head-of-line-blocking.md)
- [Message-passing channel](message-passing-channel.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/concurrent-programming/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/3/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/3/b/solution.md)
