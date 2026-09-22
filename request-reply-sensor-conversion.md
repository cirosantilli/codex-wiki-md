# Request-reply sensor conversion

↑ **Parent:** [Device driver](device-driver.md)

A [device driver](device-driver.md) protocol giving each accepted client request its own fresh hardware conversion. A single driver owns the device registers, queues requests, starts one conversion, waits for its completion, reads the result and replies to the identified requester before starting the next conversion. Sender identity and a per-call token prevent reply confusion. A [FIFO queue](fifo-queue.md) prevents later accepted requests from overtaking earlier ones.

Safety follows from at most one active conversion and exclusive register ownership. [Starvation freedom](starvation-freedom.md) additionally needs finite conversion time, eventual interrupt delivery, fair request acceptance and scheduling, and clients ready to receive their replies. These are progress assumptions, not consequences of [mutual exclusion](mutual-exclusion.md) alone.

## ↑ Ancestors (4)

1. [Device driver](device-driver.md)
2. [Operating system](operating-system-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof-resit/2/b/solution.md)
