# Channel multiplexing

↑ **Parent:** [Message passing](message-passing.md)

Sharing one [message-passing channel](message-passing-channel.md) among multiple logical streams by attaching a stream identity to each transferred value. Independent cancellation requires a protocol that conveys which stream is ending; bounded per-stream [flow control](flow-control.md) can prevent [head-of-line blocking](head-of-line-blocking.md) from a single unready consumer.

**Table of contents**

- [Multiplexed channel](multiplexed-channel.md)
- [Channel demultiplexer](channel-demultiplexer.md)
- [Channel multiplexer](channel-multiplexer.md)

## ↑ Ancestors (7)

1. [Message passing](message-passing.md)
2. [Synchronization (computing)](synchronization-computing.md)
3. [Thread (computing)](thread-computing.md)
4. [Process (computing)](process-computing.md)
5. [Operating system](operating-system-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)
