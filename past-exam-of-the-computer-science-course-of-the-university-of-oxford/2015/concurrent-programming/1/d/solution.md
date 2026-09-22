<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [channel multiplexer](../../../../../channel-multiplexer.md) adds a stream identity; a [channel demultiplexer](../../../../../channel-demultiplexer.md) removes it and selects the corresponding output. Add an explicit per-stream end marker, since closing the shared [message-passing channel](../../../../../message-passing-channel.md) cannot identify which producer has finished. `End(i)` is represented by `None`; `Some(x)` represents a genuine value, including a `null` value if the application permits one.

```
final case class MUX[T](stream: Int, item: Option[T])
```

The following [Communicating Scala Objects](../../../../../communicating-scala-objects.md) implementation uses a synchronous one-to-one `mid`. As in part (a), a short timer detects closure even when no communication is enabled. Only the [channel multiplexer](../../../../../channel-multiplexer.md) owns the input ports, and only the [channel demultiplexer](../../../../../channel-demultiplexer.md) owns the output ports. The [channel multiplexer](../../../../../channel-multiplexer.md) takes at most one input value before its corresponding `mid` write; it never accepts a second input while that write is pending.

```
def iMux[T](ins: Seq[?[T]], mid: ![MUX[T]]): PROC = proc {
  val ended = Array.fill(ins.length)(false)
  val poll = 1000000L
  try {
    while (mid.canOutput && ended.contains(false)) {
      for (i <- ins.indices if !ended(i) && !ins(i).canInput) {
        mid ! MUX[T](i, None)
        ended(i) = true
      }
      if (ended.contains(false)) {
        alt(
          (| (for (i <- ins.indices) yield
            (!ended(i) && ins(i)) =?=> { x => mid ! MUX(i, Some(x)) }))
          | after(poll) ==> { () }
        )
      }
    }
  } catch { case _: io.threadcso.process.Stopped => () }
  finally { ins.foreach(_.closeIn); mid.closeOut }
}

def iDemux[T](mid: ?[MUX[T]], outs: Seq[![T]]): PROC = proc {
  val ended = Array.fill(outs.length)(false)
  val poll = 1000000L
  try {
    while (mid.canInput && ended.contains(false) &&
           outs.indices.forall(i => ended(i) || outs(i).canOutput)) {
      alt(
        mid =?=> { packet =>
          val i = packet.stream
          require(i >= 0 && i < outs.length && !ended(i))
          packet.item match {
            case Some(x) => outs(i) ! x
            case None => ended(i) = true; outs(i).closeOut
          }
        }
        | after(poll) ==> { () }
      )
    }
  } catch { case _: io.threadcso.process.Stopped => () }
  finally { mid.closeIn; outs.foreach(_.closeOut) }
}
```

For each stream, the output [sequence](../../../../../sequence.md) remains a prefix of its accepted input [sequence](../../../../../sequence.md). One value can be pending in the [channel demultiplexer](../../../../../channel-demultiplexer.md), and one in the [channel multiplexer](../../../../../channel-multiplexer.md), possibly from the same stream. Hence its discrepancy is at most two:

$$
\boxed{N=2\text{ is a valid per-stream storage bound for this implementation}.}
$$

There is a shared total of two pending values, so these processes do not supply the independent readiness of a parallel collection of capacity-two [strict buffers](../../../../../strict-buffer.md). An unready consumer blocks the [channel demultiplexer](../../../../../channel-demultiplexer.md)'s ordinary send; the [channel multiplexer](../../../../../channel-multiplexer.md) can accept one further value and then blocks too. This is [head-of-line blocking](../../../../../head-of-line-blocking.md).

The [alternation](../../../../../guarded-alternation.md) may choose an input unfairly; replacing its selection policy by round-robin selection helps among simultaneously ready producers. Even fair input choice cannot compensate for a consumer that blocks the entire [channel demultiplexer](../../../../../channel-demultiplexer.md). Closed-input scanning does allow a producer's end marker eventually to reach its consumer, but only after the shared transport and any earlier delivery become serviceable. Its own accepted values precede its end marker, so that consumer drains cleanly.

Consumer-driven closure is more restrictive. With no return [message-passing channel](../../../../../message-passing-channel.md), the sender cannot promptly learn which producer should stop. This implementation deliberately shuts down the whole [multiplexed channel](../../../../../multiplexed-channel.md) when it detects any unfinished consumer closing, thereby cancelling the other pairs too. If the [channel demultiplexer](../../../../../channel-demultiplexer.md) is already blocked on some other consumer, even that detection waits for the blocked send. Thus producer-driven ends can be represented separately but need not be delivered promptly; consumer-driven cancellation is global and need not be detected promptly. Merely adding an end marker does not solve either delay.

## ↑ Ancestors (11)

1. [D](../d.md)
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
