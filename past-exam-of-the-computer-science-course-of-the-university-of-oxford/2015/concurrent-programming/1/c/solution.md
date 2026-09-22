<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a [tagged union](../../../../../tagged-union.md) so that an idle indication cannot be confused with an actual value of type `T`. [Heartbeat messages](../../../../../heartbeat-message.md) are transport messages only and never reach the consumer.

```
sealed trait InterPeer[+T]
final case class Data[T](value: T) extends InterPeer[T]
case object Idle extends InterPeer[Nothing]
case object EndPeer extends RuntimeException
case object PeerTimeout extends RuntimeException
```

Here are two small [Communicating Scala Objects](../../../../../communicating-scala-objects.md) helpers. A timer expiring after a port has closed denotes orderly end-of-stream, rather than evidence of a silent peer. Closure can instead make the [alternation](../../../../../guarded-alternation.md) throw `Stopped` directly. `sendWithin` completes exactly one send, or throws; `receiveWithin` completes exactly one receive, or throws. Time arguments are positive nanosecond intervals.

```
def sendWithin[A](p: ![A], value: A, t: Long): Unit = {
  if (!p.canOutput) throw EndPeer
  alt(
    p =!=> { value }
    | after(t) ==> {
        if (!p.canOutput) throw EndPeer else throw PeerTimeout
      }
  )
}
def receiveWithin[A](p: ?[A], t: Long): A = {
  if (!p.canInput) throw EndPeer
  var result: Option[A] = None
  alt(
    p =?=> { x => result = Some(x) }
    | after(t) ==> {
        if (!p.canInput) throw EndPeer else throw PeerTimeout
      }
  )
  result.get
}
```

The sender waits only half the agreed interval before preparing an idle indication, leaving some scheduling allowance before the receiver's deadline. A pending data or idle send has its own deadline, so a failed receiver cannot strand the sender forever. An application with a guaranteed network-delay bound should subtract that bound, plus scheduling allowance, when choosing the heartbeat period.

```
def iPr[T](timeout: Long, in: ?[T], out: ![InterPeer[T]],
           fail: ![Unit]): PROC = proc {
  require(timeout >= 2)
  var failed = false
  try {
    while (in.canInput && out.canOutput) {
      var packet: InterPeer[T] = Idle
      alt(
        in =?=> { x => packet = Data(x) }
        | after(timeout / 2) ==> { () }
      )
      // A just-accepted Data must survive a simultaneous upstream close.
      if (packet != Idle || in.canInput) sendWithin(out, packet, timeout)
    }
  } catch {
    case PeerTimeout => failed = out.canOutput
    case EndPeer => ()
    case _: io.threadcso.process.Stopped => ()
  } finally { in.closeIn; out.closeOut }
  try { if (failed) fail ! (()) }
  catch { case _: io.threadcso.process.Stopped => () }
  finally { fail.closeOut }
}

def iCon[T](timeout: Long, in: ?[InterPeer[T]], out: ![T],
            fail: ![Unit]): PROC = proc {
  require(timeout > 0)
  var failed = false
  try {
    while (out.canOutput) {
      receiveWithin(in, timeout) match {
        case Idle => ()
        case Data(x) => sendWithin(out, x, timeout)
      }
    }
  } catch {
    case PeerTimeout => failed = out.canOutput
    case EndPeer => ()
    case _: io.threadcso.process.Stopped => ()
  } finally { in.closeIn; out.closeOut }
  try { if (failed) fail ! (()) }
  catch { case _: io.threadcso.process.Stopped => () }
  finally { fail.closeOut }
}
```

Each failure port has a supervising receiver that accepts its single notification; data-port cleanup occurs before that potentially blocking notification. The sender reports an interpeer send taking too long. The receiver reports an excessive interpeer receive delay or an excessive delay delivering a value to the consumer. Producer idleness alone is healthy and causes [heartbeat messages](../../../../../heartbeat-message.md), not a failure. A sufficiently slow consumer can ultimately cause both detectors to fire, since its [backpressure](../../../../../backpressure.md) reaches the sender.

Ignoring [heartbeat messages](../../../../../heartbeat-message.md), at most one genuine value is held by each intermediary with a synchronous interpeer [message-passing channel](../../../../../message-passing-channel.md); no value overtakes another. Normal upstream closure propagates after the last accepted genuine value is delivered, provided its delivery meets the deadline. The pair is not ready for another input while its sender is blocked sending, so it has the specified prefix and bounded-storage properties without every readiness property of an ideal [strict buffer](../../../../../strict-buffer.md). Its useful guarantee is

$$
\boxed{\text{ordered genuine data, at most two pending values, and timed failure indications}.}
$$

A timeout establishes suspicion, not proof of a crash: a live but delayed peer or an excessive network delay gives the same observation. There is no promise of bounded detection when the detector itself is never scheduled, nor of exact agreement between the two failure indications. A sender-side deadline measures completion of its own send: a network adapter that merely accepts values into local storage cannot confirm remote receipt. Detecting that remote failure at the sender would require confirmations over a return [message-passing channel](../../../../../message-passing-channel.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
