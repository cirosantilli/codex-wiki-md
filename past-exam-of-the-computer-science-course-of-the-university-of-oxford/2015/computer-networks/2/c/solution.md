<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Dynamic [network address and port translation](../../../../../network-address-and-port-translation.md) has an important [soft state](../../../../../soft-state.md) aspect: activity refreshes a binding's lifetime, and inactivity eventually expires it without a reliably delivered close message. This is especially useful for [UDP](../../../../../user-datagram-protocol.md), which supplies no connection-closing exchange. Even for [TCP](../../../../../transmission-control-protocol.md), the [router](../../../../../router.md) cannot assume that it will observe every closing [packet](../../../../../network-packet.md).

However, an expiring entry is not necessarily harmlessly disposable. Suppose the binding `10.0.0.2:49152` to `198.51.100.7:62001` disappears while the remote [endpoint](../../../../../communication-endpoint.md) is still using it. A reply to port 62001 no longer reveals the private destination. New outbound traffic might obtain a different public [transport port](../../../../../transport-port.md), which does not reconstruct the old connection as viewed by the remote [endpoint](../../../../../communication-endpoint.md). Losing the binding can therefore break the exchange even though both [endpoints](../../../../../communication-endpoint.md) remain alive. This conflicts with [fate-sharing](../../../../../fate-sharing.md) when indispensable connection information resides in a separate [router](../../../../../router.md).

Static address mappings and configured [port forwarding](../../../../../port-forwarding.md) are [hard state](../../../../../hard-state.md); a fixed translation rule need not even require a dynamic per-exchange table. Thus

$$
\boxed{\text{dynamic bindings use soft-state expiry, but may hold essential connection state}.}
$$

Describing all [network address translation](../../../../../network-address-translation.md) information as fully reconstructible [soft state](../../../../../soft-state.md) would overlook both this recovery limitation and the static configuration.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Computer networks](../../../computer-networks-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
