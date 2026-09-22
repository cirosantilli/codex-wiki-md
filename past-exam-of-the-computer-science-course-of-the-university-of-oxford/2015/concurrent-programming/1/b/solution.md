<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A cyclic [Communicating Scala Objects](../../../../../communicating-scala-objects.md) component has a communication loop followed by a close-down phase. `repeat { ... }` catches the library's normal `Stopped` family of exceptions, including closure, and leaves the loop; ordinary `while` code instead needs the explicit handler used above. In either case, cleanup closes every owned input port with `closeIn` and every owned output port with `closeOut`, preferably in `finally`. Reclosing a one-to-one port is harmless. A parallel composition completes only when every component has completed; one component returning does not automatically cancel all the others.

The producer closes `left` on return. The [strict buffer](../../../../../strict-buffer.md) observes this, drains its [FIFO queue](../../../../../fifo-queue.md) into a cooperating consumer, and closes `right`; the consumer's next read detects closure and enters its own cleanup. Conversely, the consumer closes `right` on return; the [strict buffer](../../../../../strict-buffer.md) then closes `left`, releasing a blocked producer write or causing its next write to stop. Thus,

$$
\boxed{\text{upstream closure drains forward; downstream closure cancels backward}.}
$$

Eventual termination assumes that surviving components reach their next communication or closure check, and that the consumer keeps accepting a finite outstanding backlog after producer termination. A component stuck forever in unrelated computation cannot be stopped by closing a port alone.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Concurrent programming](../../../concurrent-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
