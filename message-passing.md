# Message passing

↑ **Parent:** [Synchronization (computing)](synchronization-computing.md)

[Operating-system processes](process-computing.md) communicate by sending and receiving messages. A [message-passing mutual exclusion server](message-passing-mutual-exclusion-server.md) can centralize ownership of a shared resource: clients request permission, wait for a grant, and release the resource when finished. Correctness depends on an explicit delivery and failure model; reliable delivery and compliant clients suffice for the basic ownership protocol.

**Table of contents**

- [Control channel](control-channel.md)
- [Channel multiplexing](channel-multiplexing.md)
  - [Multiplexed channel](multiplexed-channel.md)
  - [Channel demultiplexer](channel-demultiplexer.md)
  - [Channel multiplexer](channel-multiplexer.md)
- [Heartbeat message](heartbeat-message.md)
- [Message-passing channel](message-passing-channel.md)
  - [Strict buffer](strict-buffer.md)
- [Head-of-line blocking](head-of-line-blocking.md)
- [Synchronous message passing](synchronous-message-passing.md)
  - [Synchronous send-and-receive](synchronous-send-and-receive.md)

## ↑ Ancestors (6)

1. [Synchronization (computing)](synchronization-computing.md)
2. [Thread (computing)](thread-computing.md)
3. [Process (computing)](process-computing.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Message-passing mutual exclusion server](message-passing-mutual-exclusion-server.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof-resit/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/3/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/3/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/3/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/2/a/solution.md)
- [Synchronous message passing](synchronous-message-passing.md)
