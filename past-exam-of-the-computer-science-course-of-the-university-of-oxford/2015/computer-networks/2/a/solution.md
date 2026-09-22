<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Soft state](../../../../../soft-state.md) is information maintained by refreshes and allowed to expire when those refreshes cease. It can be reconstructed from continuing communication with the participants that still need it. [Hard state](../../../../../hard-state.md) instead persists until explicitly changed or removed; a lost deletion or failed participant can therefore leave stale information indefinitely. This distinction concerns the maintenance rules, rather than simply whether the information is in volatile memory.

For example, a [router](../../../../../router.md) can keep [IP multicast](../../../../../ip-multicast.md) membership information for a local network. Periodic membership queries and reports refresh that information; if no member reports within the prescribed interval, the membership expires. A host that crashes without unsubscribing is eventually forgotten. A lost report need not remove membership immediately, because repeated reports and a suitable expiry interval tolerate occasional loss. If the [router](../../../../../router.md) loses its membership information, subsequent queries and reports rebuild it.[Appendix I, §§I.1–I.3: queries, reports and membership timers](../../../../../host-extensions-for-ip-multicasting-rfc-1112.md)

This is attractive in [Internet](../../../../../internet.md) components because [packet](../../../../../network-packet.md) loss, host crashes and [router](../../../../../router.md) restarts need not be repaired by a perfectly delivered sequence of explicit deletions. Refreshes repair some omissions, and expiry removes abandoned entries and releases resources. Components can recover local state without retaining an indefinitely accurate history of everyone else's actions. [Soft state](../../../../../soft-state.md) does have a cost: refresh traffic, timer storage and temporary stale or missing information, with a tradeoff between rapid expiry and tolerance of delayed refreshes. Its central benefit is

$$
\boxed{\text{refresh reconstructs live state; timeout removes abandoned state}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
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
