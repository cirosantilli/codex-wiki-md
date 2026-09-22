<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For two competing [TCP](../../../../../transmission-control-protocol.md) connections, each sender's [congestion control](../../../../../congestion-control.md) aims to obtain useful throughput while adapting to shared capacity and avoiding persistent overload. For two comparable, continuously backlogged connections at one bottleneck, the usual fairness objective is approximately half the available capacity each, while keeping the bottleneck productively used. The goal is not for both senders independently to seize the whole link. Unequal delays, implementations, application demands and other bottlenecks mean that equal throughput is not guaranteed.

For two [UDP](../../../../../user-datagram-protocol.md) exchanges, there is no corresponding built-in transport [congestion control](../../../../../congestion-control.md) objective: [UDP](../../../../../user-datagram-protocol.md) sends datagrams without specifying a congestion response. The applications might implement well-behaved [congestion control](../../../../../congestion-control.md), rate limiting or no adaptation at all. Consequently two [UDP](../../../../../user-datagram-protocol.md) labels alone do not determine either a target share or the resulting allocation. Applications should still manage overload; that responsibility is outside the base [UDP](../../../../../user-datagram-protocol.md) service.

For a competing [TCP](../../../../../transmission-control-protocol.md) connection and an unresponsive high-rate [UDP](../../../../../user-datagram-protocol.md) application sharing an ordinary queue, losses cause the [TCP](../../../../../transmission-control-protocol.md) sender to reduce its offered load while the [UDP](../../../../../user-datagram-protocol.md) sender continues. The [UDP](../../../../../user-datagram-protocol.md) traffic can take much of the bottleneck capacity and severely reduce [TCP](../../../../../transmission-control-protocol.md) throughput. If the [UDP](../../../../../user-datagram-protocol.md) rate exceeds capacity, it too loses [packets](../../../../../network-packet.md); sending more does not guarantee useful delivery. A modest-rate or adaptive [UDP](../../../../../user-datagram-protocol.md) application, or a [router](../../../../../router.md) enforcing [fair queueing](../../../../../fair-queueing.md), gives a different outcome. Thus

$$
\boxed{\text{TCP seeks an adaptive fair share; UDP alone supplies no competing control law}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
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
