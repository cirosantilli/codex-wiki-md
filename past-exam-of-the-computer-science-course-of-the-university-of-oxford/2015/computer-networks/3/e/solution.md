<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

[Nagle's algorithm](../../../../../nagle-s-algorithm.md) prevents the small-packet problem: an application that writes one or a few [bytes](../../../../../byte.md) at a time could generate a separate [TCP](../../../../../transmission-control-protocol.md) [TCP segment](../../../../../tcp-segment.md) for each write, with transport/link overhead and [router](../../../../../router.md) work far larger than the useful data. This is a sender-side cause of the [silly window syndrome](../../../../../silly-window-syndrome.md) family of inefficient tiny transmissions.

When no data are outstanding, send the first small [TCP segment](../../../../../tcp-segment.md) promptly. While data remain unacknowledged, accumulate further small writes instead of emitting another short [TCP segment](../../../../../tcp-segment.md). Release the accumulated data when either enough are available for a full-sized [TCP segment](../../../../../tcp-segment.md), subject to the allowed [send window](../../../../../send-window.md), or the outstanding data have been acknowledged. This makes the waiting adapt to the [round-trip time](../../../../../round-trip-time.md), rather than imposing one fixed batching interval.[The small-packet problem and the proposed unacknowledged-data rule](../../../../../congestion-control-in-ip-tcp-internetworks-rfc-896.md)

The penalty is extra [network latency](../../../../../network-latency.md) for later small writes. A short application message split across writes may have its second piece delayed awaiting the [acknowledgement](../../../../../acknowledgement.md) of the first. If the receiver uses a [delayed acknowledgement](../../../../../delayed-acknowledgement.md) while its application awaits that second piece, progress can wait for the acknowledgement timer. It is a delay interaction, not a permanent deadlock while that timer works. Latency-sensitive applications can request that [Nagle's algorithm](../../../../../nagle-s-algorithm.md) be disabled, accepting the possible extra [packets](../../../../../network-packet.md). The tradeoff is

$$
\boxed{\text{fewer tiny segments, at the cost of waiting to coalesce subsequent small writes}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
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
