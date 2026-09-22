# Bus arbitration

↑ **Parent:** [Computer bus](computer-bus.md)

Selecting among initiators requesting a shared resource. An arbiter grants permission before an initiator starts its [bus transaction](bus-transaction.md). Fixed priority can indefinitely postpone a lower-priority requester under continuing higher-priority demand. Rotating priority can provide [starvation freedom](starvation-freedom.md) when every owner releases the resource after bounded work. Neither policy alone determines [bus throughput](bus-throughput.md): waiting, setup and target readiness also matter.[CS152 lecture 21, slides 35–36: reservation, priority and fairness](cs152-computer-architecture-and-engineering-fall-1999/lecture-21-buses-and-i-and-o.md)

**Table of contents**

- [Bus ownership](bus-ownership.md)
- [Bus contention](bus-contention.md)

## ↑ Ancestors (3)

1. [Computer bus](computer-bus.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Bus burst](bus-burst.md)
- [Bus contention](bus-contention.md)
- [Computer bus](computer-bus.md)
- [Control bus](control-bus.md)
- [Shared-bus timing example](shared-bus-timing-example.md)
