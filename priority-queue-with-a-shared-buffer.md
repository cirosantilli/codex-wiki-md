# Priority queue with a shared buffer

↑ **Parent:** [Multiclass single-server queue](multiclass-single-server-queue.md)

A two-class [queue](queue-queueing-theory.md) has one total buffer but serves the high-priority class before the other. A preemptive-resume [service discipline](service-discipline.md) interrupts low-priority work immediately and later resumes it without wasting completed work. Under [first come first served](first-come-first-served.md) within the high-priority class, a new high-priority packet waits $V/C$ when $V$ is the high-priority workload immediately before its arrival. The total workload determines shared-buffer overflow, while $V$ determines the high-priority waiting time. An additional admission gate rejects high-priority packets when $V/C$ exceeds a prescribed delay limit. Finite packets require a fit test against the remaining buffer space, and nonpreemptive service adds residual low-priority service time.

**Table of contents**

- [Effective-bandwidth admission region with a voice delay gate](effective-bandwidth-admission-region-with-a-voice-delay-gate.md)

## ↑ Ancestors (7)

1. [Multiclass single-server queue](multiclass-single-server-queue.md)
2. [Queueing theory](queueing-theory-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/4/b/solution.md)
- [Queueing delay](queueing-delay.md)
