<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

O1 supplies [mutual exclusion](../../../../../../mutual-exclusion.md) over each complete operation. A reader sees the protected state from a serial order of readers and writers; a writer can safely mutate the existing object while holding the common [mutex](../../../../../../mutex.md). If an update reads the old state and modifies it, the entire read-modify-write can be protected against a [lost update](../../../../../../lost-update.md).

O2 has different semantics. Assume an indivisible aligned access to `p`, correct publication ordering, and no later mutation of a published version. A reader chooses one version when it loads `p`; the subsequent [load instructions](../../../../../../load-instruction.md) use the same saved [pointer](../../../../../../pointer-computer-programming.md), so an overlapping writer need not block that reader. The reader may continue observing the old complete version after the writer has published the new one. A sufficiently specified snapshot read can still be [linearizable](../../../../../../linearizability.md), with the load of `p` as its [linearization point](../../../../../../linearization-point.md): a read overlapping a write is allowed to come before that write in the abstract order. Thus reading an old version during overlap does not by itself prove failure of [linearizability](../../../../../../linearizability.md).

Multiple writers can each construct a valid replacement and race to publish it. If the operation is simply “replace the whole object”, atomic pointer stores give a last-publication order. If each writer instead computes a change from the previously published state, O2 alone does not preserve both changes. Two writers can both read a counter value zero, independently build a version containing one, and publish their respective versions; the final counter is one. A writer [mutex](../../../../../../mutex.md) or [compare-and-swap](../../../../../../compare-and-swap.md) with retry is needed when the required operation must avoid that [lost update](../../../../../../lost-update.md). [Memory barriers](../../../../../../memory-barrier.md) alone do not provide this exclusion.

Releasing the old object's [computer memory](../../../../../../computer-memory-split.md) immediately after publishing a replacement is unsafe. For example:
```
reader: q := LOAD [p]          // gets the old object
writer: STORE [p], new_object
writer: free(old_object)
reader: LOAD [q + field]       // accesses freed storage
```
The final operation is a [use-after-free](../../../../../../use-after-free.md): it may crash, see allocator metadata, or read a different object that reuses the same [memory address](../../../../../../memory-address.md). An atomic update of `p` does not update the reader's already copied [pointer](../../../../../../pointer-computer-programming.md). Freeing the new object immediately would of course also invalidate `p` itself.

**Publication and reclamation are separate: publish a fully initialized version, and retain every old version until all readers that might hold it have finished.** A [read-copy-update](../../../../../../read-copy-update.md) [grace period](../../../../../../grace-period.md) or a suitable [hazard pointer](../../../../../../hazard-pointer.md) protocol can provide that lifetime guarantee; naive reference-count acquisition after loading an unprotected [pointer](../../../../../../pointer-computer-programming.md) can itself race with freeing. Correct [memory barriers](../../../../../../memory-barrier.md) in part (iii) ensure visibility, not object lifetime.

$$
\boxed{\text{Retain old versions until every possible reader has finished.}}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Computer architecture](../../../../computer-architecture-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
