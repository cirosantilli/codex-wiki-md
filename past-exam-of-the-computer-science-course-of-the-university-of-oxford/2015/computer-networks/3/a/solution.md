<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Transport sequence numbers](../../../../../transport-sequence-number.md) identify the position of data within an exchange. They let a receiver restore order, recognize duplicates, identify missing data and state precisely what has been received in an [acknowledgement](../../../../../acknowledgement.md). In [TCP](../../../../../transmission-control-protocol.md) they count [bytes](../../../../../byte.md), so one [packet](../../../../../network-packet.md) can contain several consecutively numbered [bytes](../../../../../byte.md).

A [send window](../../../../../send-window.md) is the range of numbered data the sender is currently allowed to have outstanding. It permits several transmissions before their [acknowledgements](../../../../../acknowledgement.md) return, which keeps the path busy despite [network latency](../../../../../network-latency.md), while bounding unacknowledged data and the information needed for [data retransmission](../../../../../retransmission-data-networks.md). A [receive window](../../../../../receive-window.md) specifies the range the receiver is prepared to accept, limiting buffer use and rejecting data outside the current range; an implementation may retain acceptable out-of-order data until earlier data arrive. As [acknowledgements](../../../../../acknowledgement.md) and consumption advance, these ranges slide, giving a [sliding window protocol](../../../../../sliding-window-protocol.md). Thus

$$
\boxed{\text{numbers identify data; send/receive windows bound outstanding/acceptable data}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
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
