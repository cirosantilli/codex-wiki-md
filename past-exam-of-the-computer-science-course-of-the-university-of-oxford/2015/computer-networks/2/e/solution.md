<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

In [reverse path forwarding](../../../../../reverse-path-forwarding.md), a [router](../../../../../router.md) uses its [unicast](../../../../../unicast.md) routing information to ask which interface it would use to send a [packet](../../../../../network-packet.md) back towards source $S$. It accepts a [multicast](../../../../../multicast.md) [packet](../../../../../network-packet.md) from $S$ only when it arrives on that interface, and otherwise discards it. An accepted [packet](../../../../../network-packet.md) can be forwarded on the other eligible interfaces. This needs no globally computed [multicast distribution tree](../../../../../multicast-distribution-tree.md) before the first transmission.[§2: reverse-path broadcasting and truncation](../../../../../distance-vector-multicast-routing-protocol-rfc-1075.md)

With stable, loop-free routes and a consistent choice of parent when routes tie, each non-source [router](../../../../../router.md) selects one upstream parent towards $S$. Following parent links reaches $S$, so the accepted parent links form a source-rooted [tree](../../../../../tree-graph-theory-split.md) over reachable [routers](../../../../../router.md). A [packet](../../../../../network-packet.md) arriving across a cross-link from a non-parent fails the reverse-path test. Basic flooding can still transmit copies that will be discarded; downstream-neighbour information can suppress such useless transmissions, and a designated forwarder prevents duplicate delivery on a shared local network.

To adapt the forwarding structure to a particular [multicast](../../../../../multicast.md) group, retain branches with local members or interested descendants and prune the others. Leaf [routers](../../../../../router.md) with no interested receivers initiate pruning; a [router](../../../../../router.md) with no local members and no remaining interested children can propagate that condition upstream. A new subscriber requires a join/graft or later refresh to restore a pruned branch. Thus [reverse path forwarding](../../../../../reverse-path-forwarding.md) gives the source-rooted reachability structure, while membership and pruning restrict it to useful branches.

This [tree](../../../../../tree-graph-theory-split.md) need not minimize total transmission cost. Even if the [unicast](../../../../../unicast.md) routes are [shortest paths](../../../../../shortest-path.md) under symmetric positive link costs, their union minimizes individual distances from the source, rather than the sum of the costs of all used links. For a small example, let $SA$ and $SB$ each cost 2 and let $AB$ cost 1, with receivers at $A$ and $B$. The [shortest-path tree](../../../../../shortest-path-tree.md) uses $SA$ and $SB$, costing 4 in total. Using $SA$ and $AB$ costs 3, although the route from $S$ to $B$ then has length 3 instead of 2. Moreover, real [unicast](../../../../../unicast.md) policies may optimize other criteria, and reverse routes need not be best forward routes when costs are asymmetric. Therefore

$$
\boxed{\text{reverse-path acceptance yields a delivery tree, not necessarily a minimum-cost tree}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
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
