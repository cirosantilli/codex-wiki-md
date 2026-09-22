<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[UDP](../../../../../user-datagram-protocol.md) fits [IP multicast](../../../../../ip-multicast.md) because each independent datagram can be delivered to a group without establishing a separate transport connection with every receiver. Ordinary [TCP](../../../../../transmission-control-protocol.md) defines a reliable ordered byte stream between two [endpoints](../../../../../communication-endpoint.md), with one peer's [acknowledgements](../../../../../acknowledgement.md), [receive window](../../../../../receive-window.md) and connection state. A group has many receivers with different losses and capacities, so that interface cannot simply be assigned to one group address. A reliable group service can be designed, but ordinary [TCP](../../../../../transmission-control-protocol.md) does not provide it. [UDP](../../../../../user-datagram-protocol.md) itself adds neither group reliability nor [congestion control](../../../../../congestion-control.md); applications must provide whatever additional behaviour they require.

A virtual [multicast distribution tree](../../../../../multicast-distribution-tree.md) lets one [packet](../../../../../network-packet.md) traverse a shared upstream link and be copied only where branches diverge. Compared with a separate [unicast](../../../../../unicast.md) copy per receiver, this saves repeated transmission over the common links. A [tree](../../../../../tree-graph-theory-split.md) also supplies a unique parent route and avoids forwarding loops when the routing information is consistent. Branches with no interested receivers can be pruned.

For a source-specific [multicast distribution tree](../../../../../multicast-distribution-tree.md), a [router](../../../../../router.md) needs the group identifier and source identifier, the expected incoming interface, the set of outgoing interfaces leading to interested receivers, and information about local group membership. Timers and join/prune information maintain those decisions. This is naturally keyed by $(S,G)$ for source $S$ and group $G$; other [multicast routing](../../../../../multicast-routing.md) designs can use a shared group tree. A [router](../../../../../router.md) needs the relevant local forwarding entries, rather than a complete list of all group members everywhere. The result is

$$
\boxed{\text{one upstream copy; replication at branches; per-tree input/output interface state}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
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
