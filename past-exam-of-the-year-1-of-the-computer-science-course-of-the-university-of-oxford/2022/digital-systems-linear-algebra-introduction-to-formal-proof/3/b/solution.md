<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With [synchronous message passing](../../../../../synchronous-message-passing.md), the smoothing [operating-system process](../../../../../process-computing.md) can still be waiting for `TEMP` when its next `PING` is due. If the timer service sends to subscribers serially, it blocks on this unready recipient and cannot deliver the other subscribers' ticks: **one slow sensor can delay every timer client through [head-of-line blocking](../../../../../head-of-line-blocking.md)**. Once it resumes, implementations may deliver late ticks, drift from their schedule, or accumulate overdue work.

The consequence depends on the delivery model. With buffered sends the timer need not block immediately, but its [queue](../../../../../queue-queueing-theory.md) can grow or overflow; the smoothing [operating-system process](../../../../../process-computing.md) still cannot process readings at a sustained rate faster than the [sensor](../../../../../sensor.md). A nonblocking notification mechanism or separate timer-delivery workers can isolate other subscribers, while coalescing missed ticks prevents an unlimited backlog. These changes do not make an over-slow [sensor](../../../../../sensor.md) meet the original sampling rate.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
