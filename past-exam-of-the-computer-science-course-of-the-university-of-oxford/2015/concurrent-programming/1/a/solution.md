<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Store the accepted but undelivered values in an ordinary [FIFO queue](../../../../../fifo-queue.md), owned exclusively by the [Communicating Scala Objects](../../../../../communicating-scala-objects.md) process. An input event is enabled precisely when the [FIFO queue](../../../../../fifo-queue.md) is not full, and an output event precisely when it is not empty. An output event's expression is evaluated only after that event is selected; its epilogue runs after the output completes. The following uses no buffered communication [message-passing channels](../../../../../message-passing-channel.md).

```
def strictBuffer[T](capacity: Int, in: ?[T], out: ![T]): PROC = proc {
  require(capacity > 0)
  val q = scala.collection.mutable.Queue[T]()
  val poll = 1000000L                     // nanoseconds
  try {
    while (out.canOutput && (in.canInput || q.nonEmpty)) {
      alt(
        (q.size < capacity && in) =?=> { x => q.enqueue(x) }
        | (q.nonEmpty && out) =!=> { q.front } ==> { q.dequeue(); () }
        | after(poll) ==> { () }
      )
    }
  } catch { case _: io.threadcso.process.Stopped => () }
  finally { in.closeIn; out.closeOut }
}
```

Here `canInput` and `canOutput` mean that the port has not become permanently unable to communicate; they are not instantaneous readiness tests. A closed input event is disabled by the [Communicating Scala Objects](../../../../../communicating-scala-objects.md) [guarded alternation](../../../../../guarded-alternation.md). The timer periodically rechecks closure even when the affected port's data event is disabled, for example when the [FIFO queue](../../../../../fifo-queue.md) is empty and the downstream port closes. It neither transfers data nor imposes a deadline on a healthy producer. This avoids silently assuming that closure of a disabled event wakes an [alternation](../../../../../guarded-alternation.md). The relevant output-event and closure conventions are documented in [2017 revision, §§4 and 5.2](../../../../../communicating-scala-objects-by-bernard-sufrin.md).

Write $I$ and $O$ for the input and output [sequences](../../../../../sequence.md). The [loop invariant](../../../../../loop-invariant.md) is that $I$ is $O$ followed by the contents of the [FIFO queue](../../../../../fifo-queue.md). An input appends one value to its rear; an output removes exactly its front. Consequently,

$$
\boxed{O\text{ is a prefix of }I,\qquad 0\leq |I|-|O|=|q|\leq\mathrm{capacity}.}
$$

The two data events remain offered whenever their respective size conditions hold. Under a fair choice policy, an endlessly ready event is eventually selected. The timer requires the usual assumption that expiry cannot starve a ready communication forever.

When the input closes, no more values are accepted, but all remaining values stay eligible for output. Once the [FIFO queue](../../../../../fifo-queue.md) empties, the process closes its output and terminates. If the output closes first, there is no recipient for those remaining values: the process abandons them, closes the input to release the producer, and terminates. Draining after upstream closure requires a consumer that continues receiving. The positive-capacity precondition is deliberate: two separate [synchronous message passing](../../../../../synchronous-message-passing.md) events cannot provide a capacity-zero buffer with zero discrepancy after every event; that would require a simultaneous three-party transfer.

## ↑ Ancestors (11)

1. [A](../a.md)
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
