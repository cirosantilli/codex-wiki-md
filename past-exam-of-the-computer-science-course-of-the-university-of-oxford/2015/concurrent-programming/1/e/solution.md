<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use a return [control channel](../../../../../control-channel.md) to carry both cancellation and one-slot [flow control](../../../../../flow-control.md). The latter is what prevents a silent consumer from obstructing other streams. Keep the preceding `MUX` type and add

```
sealed trait CTRL
final case class Grant(stream: Int) extends CTRL
final case class Cancel(stream: Int) extends CTRL
```

Here is a precise event-loop specification of the modified generators. `choose` means a fair [Communicating Scala Objects](../../../../../communicating-scala-objects.md) [guarded alternation](../../../../../guarded-alternation.md) over the listed input events, output events and a short closure-poll timer; every selected transition below is finite and contains no further blocking communication. An output transition commits its state change only after its selected send succeeds. The notation is operational pseudocode, with the requested signatures; it does not introduce an assumed nonblocking send primitive.

```
def iMux[T](ins: Seq[?[T]], ctrl: ?[CTRL], mid: ![MUX[T]]): PROC
  for each stream i:
    credit[i] = true; inputOpen[i] = true; terminal[i] = false
    pending[i] = None                     // Option[MUX[T]]
  until every terminal[i]:
    poll closures:
      if !ins[i].canInput: inputOpen[i] = false
      if !terminal[i] && !inputOpen[i] && pending[i].isEmpty:
        pending[i] = Some(MUX(i, None))   // end follows earlier data
    choose:
      ctrl ? Grant(i):
        if !terminal[i]: credit[i] = true
      ctrl ? Cancel(i):
        terminal[i] = true; pending[i] = None; ins[i].closeIn
      ins[i] ? x, enabled when inputOpen[i] && !terminal[i]
                              && credit[i] && pending[i].isEmpty:
        credit[i] = false; pending[i] = Some(MUX(i, Some(x)))
      mid ! pending[i].get, enabled when pending[i].nonEmpty:
        if pending[i].get.item.isEmpty: terminal[i] = true
        pending[i] = None
      poll timer: no action
  finally: close every ins[i] input; close mid output and ctrl input

def iDemux[T](ctrl: ![CTRL], mid: ?[MUX[T]], outs: Seq[![T]]): PROC
  for each stream i:
    slot[i] = None; ended[i] = false; cancelled[i] = false
  replies = empty FIFO queue of CTRL
  until every (cancelled[i] || (ended[i] && slot[i].isEmpty)):
    poll closures:
      if !cancelled[i] && !ended[i] && !outs[i].canOutput:
        cancelled[i] = true; slot[i] = None
        delete any queued Grant(i); append Cancel(i) to replies
      if !cancelled[i] && ended[i] && slot[i].nonEmpty
                                      && !outs[i].canOutput:
        cancelled[i] = true; slot[i] = None
      if ended[i] && slot[i].isEmpty: outs[i].closeOut
    choose:
      mid ? MUX(i, Some(x)):
        if !cancelled[i]: assert slot[i].isEmpty; slot[i] = Some(x)
      mid ? MUX(i, None):
        ended[i] = true
      outs[i] ! slot[i].get, enabled when !cancelled[i] && slot[i].nonEmpty:
        slot[i] = None
        if !ended[i]: append Grant(i) to replies
      ctrl ! replies.front, enabled when replies.nonEmpty:
        remove replies.front
      poll timer: no action
  finally: close mid input, every output, and ctrl output
```

There is one receive event on `mid`, with the two packet forms dispatched in its body, and one send event on `mid`, offering a fairly chosen pending stream. There is likewise one send event on `ctrl`. If `mid` becomes exhausted, the [channel demultiplexer](../../../../../channel-demultiplexer.md) marks any remaining streams ended, discards queued replies, and drains or cancels their slots; the sender has then finished and needs no more grants. If the control input closes, the [channel multiplexer](../../../../../channel-multiplexer.md) enters cleanup. If the receiver finds its control output closed, it discards queued replies and disables further control sends, but continues receiving end markers and draining its slots; sender completion must not discard already accepted values. A channel closing during an individual guarded operation is handled locally: a failed `outs(i)` send cancels that stream and queues `Cancel(i)` unless it had already ended; exhaustion of a shared port uses the cleanup rules just stated. Ports that closed while their data events were disabled are found by the poll. These rules specify closure handling as well as normal transitions.

The credit starts at one and is consumed when an input is accepted. It is returned only after the corresponding output finishes. Thus the one permitted outstanding value for stream $i$ is either pending at the sender or stored at the receiver, never both. An end marker needs no credit and follows that stream's last data packet on the ordered shared [message-passing channel](../../../../../message-passing-channel.md). It can arrive while that value is still waiting for its consumer; the receiver then delays closing the output until its slot empties. The invariant is

$$
\boxed{0\leq |I_i|-|O_i|\leq 1\quad\text{until stream }i\text{ is cancelled}.}
$$

As in a [strict buffer](../../../../../strict-buffer.md), cancellation can discard the last outstanding value. A cancelled receiver ignores a data packet already in flight; a later grant cannot resurrect a cancelled sender. No selected data delivery blocks the event loop, and control replies are queued rather than sent inside a receive handler. In particular, there is no cycle in which the sender blocks sending data while the receiver blocks sending cancellation. Closing the control output at final receiver termination also releases the sender if a last cancellation was still queued.

Under fair event selection and eventual scheduling, an individual cancellation reaches its producer without waiting for any unrelated consumer. Producer closure similarly delivers its own end marker without waiting for another stream to drain. This gives finite [flow control](../../../../../flow-control.md) equivalent in ordering and termination to capacity-one [strict buffers](../../../../../strict-buffer.md), with finite protocol delays. A physical shared [message-passing channel](../../../../../message-passing-channel.md) necessarily serializes transfers, so instantaneous readiness and absolute real-time delay bounds are not identical to physically separate buffers.

## ↑ Ancestors (11)

1. [E](../e.md)
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
