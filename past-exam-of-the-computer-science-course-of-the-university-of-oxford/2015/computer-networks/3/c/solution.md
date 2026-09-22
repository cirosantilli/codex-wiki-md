<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[TCP](../../../../../transmission-control-protocol.md) implements both restrictions at the sending [endpoint](../../../../../communication-endpoint.md), using information from different places. For [flow control](../../../../../flow-control.md), the receiving [TCP](../../../../../transmission-control-protocol.md) advertises its available [receive window](../../../../../receive-window.md) $\mathrm{rwnd}$ in [TCP](../../../../../transmission-control-protocol.md) headers. The sending [TCP](../../../../../transmission-control-protocol.md) tracks that advertised range together with the [acknowledgement](../../../../../acknowledgement.md) number, and must not send ordinary new data beyond its right edge. As the receiving application consumes data, the receiver can advertise more space. A zero [receive window](../../../../../receive-window.md) stops ordinary new data and invokes the separate probing mechanism.

For [congestion control](../../../../../congestion-control.md), the sender maintains a [congestion window](../../../../../congestion-window.md) $\mathrm{cwnd}$ representing its permitted amount of outstanding data given the path's condition. [Acknowledgements](../../../../../acknowledgement.md), duplicate [acknowledgements](../../../../../acknowledgement.md) and [data retransmission](../../../../../retransmission-data-networks.md) timeouts supply feedback; explicit congestion notifications can also contribute when negotiated. [Routers](../../../../../router.md) supply the underlying evidence through queuing, drops or marks, but ordinary [TCP](../../../../../transmission-control-protocol.md) [congestion window](../../../../../congestion-window.md) management takes place at the [endpoints](../../../../../communication-endpoint.md), rather than through a per-connection capacity reservation at each [router](../../../../../router.md).[§§2–3: cwnd, rwnd, flight size and sender mechanisms](../../../../../tcp-congestion-control-rfc-5681.md)

Ignoring exceptional probe behaviour, let $F$ be the number of sent but not yet acknowledged [bytes](../../../../../byte.md). The two controls combine approximately as

$$
\boxed{F\leq\min(\mathrm{rwnd},\mathrm{cwnd}),\qquad
\text{new-data allowance}=\max\{0,\min(\mathrm{rwnd},\mathrm{cwnd})-F\}.}
$$

The [send window](../../../../../send-window.md) is anchored by the acknowledged sequence position, rather than authorizing a fresh windowful on every send. [Acknowledgements](../../../../../acknowledgement.md) release room as old data leave flight. A sudden reduction of a limit can leave already transmitted data above it; the sender then waits instead of recalling those [bytes](../../../../../byte.md). The [receive window](../../../../../receive-window.md) is explicit receiver feedback, whereas the [congestion window](../../../../../congestion-window.md) is a local sender variable. No details of their parameter-adjustment algorithms are needed for this distinction.

## ↑ Ancestors (11)

1. [C](../c.md)
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
