<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The decisive difficulty is that a [TCP](../../../../../transmission-control-protocol.md) [receive window](../../../../../receive-window.md) update is not itself delivered by a reliable notification channel. The receiver can advertise a newly nonzero [receive window](../../../../../receive-window.md), but the [packet](../../../../../network-packet.md) carrying that advertisement can be lost. With the sender stopped and the receiver expecting more data, neither side need send anything else. The sender can then wait forever despite available receiver space.

A [TCP](../../../../../transmission-control-protocol.md) [acknowledgement](../../../../../acknowledgement.md) containing only an updated [receive window](../../../../../receive-window.md) does not occupy new sequence space that would make its loss trigger normal [data retransmission](../../../../../retransmission-data-networks.md). Requiring an [acknowledgement](../../../../../acknowledgement.md) of every such notification would introduce a separate reliability rule; that new [acknowledgement](../../../../../acknowledgement.md) can itself be lost. Some participant still needs a timer and retry rule. Reordering can also deliver stale advertisements, so [transport sequence number](../../../../../transport-sequence-number.md) and [acknowledgement](../../../../../acknowledgement.md) checks are needed in addition to merely sending a notification.

The [persist timer](../../../../../persist-timer.md) assigns the repeated enquiry to the side that has data waiting: the sender periodically sends a [zero-window probe](../../../../../zero-window-probe.md), eliciting an [acknowledgement](../../../../../acknowledgement.md) with the receiver's current [receive window](../../../../../receive-window.md). If one enquiry or response is lost, a later attempt can succeed. Receiver window updates remain useful for prompt resumption; probes provide recovery when those updates disappear.[§4.2.2.17: zero-window probing prevents indefinite hangs when a reopening ACK is lost](../../../../../requirements-for-internet-hosts-communication-layers-rfc-1122.md)

One could instead specify repeated receiver notifications, a response and suitable timers, but that replaces the recovery mechanism rather than eliminating its purpose. Therefore

$$
\boxed{\text{a lost reopening notification can deadlock the exchange; timed retries are needed}.}
$$

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Computer networks](../../../computer-networks-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
