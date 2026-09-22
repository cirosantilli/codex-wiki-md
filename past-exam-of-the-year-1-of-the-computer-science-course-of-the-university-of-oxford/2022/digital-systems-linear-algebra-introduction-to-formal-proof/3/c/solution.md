<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With a synchronous reply, `send(client,&answer)` blocks until the client receives. An indefinitely unready client therefore stalls the smoothing [operating-system process](../../../../../process-computing.md), which may in turn stall the timer service and its other clients as in the preceding part. If the client is merely delayed, this is blocking and delayed service; a [deadlock](../../../../../deadlock.md) requires a circular wait or a client that will never receive.

**Requiring correctly used [synchronous send-and-receive](../../../../../synchronous-send-and-receive.md) helps.** A client calling `sendrec(SMOOTH,&m)` is committed to waiting for the matching reply as soon as its request has been accepted. This closes the scheduling window between a separate send and receive and prevents unrelated client computation from postponing that receive. It does not by itself fix slow measurements, arbitrary failures, circular dependencies between other services, or lack of CPU scheduling. With buffered replies the initial effect may instead be queue growth, depending on the [message passing](../../../../../message-passing.md) contract.

## ↑ Ancestors (12)

1. [C](../c.md)
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
