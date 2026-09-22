<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Separate the two required orders. A writer must make all initialization [store instructions](../../../../../../store-instruction.md) to a fresh version visible before another [CPU core](../../../../../../cpu-core.md) can use the publication of its address. A reader must load `p` before the [load instructions](../../../../../../load-instruction.md) of fields addressed through the saved [pointer](../../../../../../pointer-computer-programming.md). Assume ordinary coherent cacheable [computer memory](../../../../../../computer-memory-split.md), atomic aligned pointer accesses, immutable published versions, and the lifetime guarantee from part (ii). The sequences below are architectural operations; a [compiler](../../../../../../compiler.md) must preserve the stated accesses and dependencies.

**TSO.** [Total store order](../../../../../../total-store-order.md) preserves store-to-store order, so initialization writes cannot become visible after the later pointer publication. It also preserves load-to-load order, so reading the pointer precedes reading its fields. Its store-to-load relaxation, illustrated in part (b), does not break either required ordering. Therefore

$$
\boxed{\text{TSO: no additional hardware fence is needed for this publication pattern}.}
$$

No drain of every reader's [store buffer](../../../../../../store-buffer.md) and no explicit cache flush is required. This statement is about hardware ordering; unsynchronized ordinary C or C++ accesses to `p` would still need the language's [atomic operation](../../../../../../atomic-operation.md) and [acquire-release synchronization](../../../../../../acquire-release-synchronization.md) facilities to avoid a [data race](../../../../../../data-race.md) and unwanted [compiler](../../../../../../compiler.md) transformations.

**Power/ARM.** These weaker [memory models](../../../../../../memory-model.md) can expose a new pointer before all the writer's initialization [store instructions](../../../../../../store-instruction.md) are visible. Put a write-ordering [memory barrier](../../../../../../memory-barrier.md) between the last initialization write and the store of `p`. A sufficient sequence uses `lwsync` on [POWER architecture](../../../../../../power-architecture.md) or an appropriately scoped `DMB`, such as `DMB ISH`, on the ARMv7 [ARM architecture family](../../../../../../arm-architecture-family.md):
```
writer:
    STORE [new + field1], value1
    STORE [new + field2], value2
    publication_barrier
    STORE [p], new
```
The scope must include every participating [CPU core](../../../../../../cpu-core.md). A broader full barrier is sufficient but can cost more. Without the writer barrier, observing the new `p` and stale initialization data is exactly the unwanted message-passing outcome.[§§2.1–2.2, message passing and ordering by `sync`/`lwsync`, printed pp. 2–4](../../../../../../understanding-power-multiprocessors-2011.md)

For the reader as actually specified, the saved [pointer](../../../../../../pointer-computer-programming.md) is an [address dependency](../../../../../../address-dependency.md): the loaded value directly determines each subsequent field's [memory address](../../../../../../memory-address.md).
```
reader:
    q := LOAD [p]
    a := LOAD [q + field1_offset]
    b := LOAD [q + field2_offset]
```
Both [POWER architecture](../../../../../../power-architecture.md) and the relevant ARM [memory models](../../../../../../memory-model.md) respect such dependent reads. Thus **no additional reader hardware fence is needed when every data access retains this real address dependency**. The writer's publication barrier together with the dependent reads supplies the necessary ordering. A mere test of `p` followed by unrelated fixed-address reads would be a [control dependency](../../../../../../control-dependency.md), which is not sufficient here.[§2.2, “Using dependencies” and “Control dependencies, observable speculative reads, and isync”, printed p. 3](../../../../../../understanding-power-multiprocessors-2011.md)

If that [address dependency](../../../../../../address-dependency.md) is not retained, use an acquire operation or an explicit read-ordering [memory barrier](../../../../../../memory-barrier.md) after loading `p` and before reading fields. `DMB ISH` on ARMv7 or `lwsync` on [POWER architecture](../../../../../../power-architecture.md) is a conservative sufficient choice for this load-to-load ordering; a suitable conditional branch followed by `isync` is another POWER acquire implementation. On later ARM instruction sets an acquire [load instruction](../../../../../../load-instruction.md) can express the reader requirement directly. Such stronger forms are often convenient even though they are not minimal for the dependent sequence in this question.

| Model | Before publishing `p` | After reading `p` |
| --- | --- | --- |
| [Total store order](../../../../../../total-store-order.md) | No extra hardware fence | No extra hardware fence |
| Power/ARM, genuine dependent field reads | Write-ordering publication barrier | Address dependency suffices |
| Power/ARM, general reads without the dependency | Write-ordering publication barrier | Acquire or sufficient read-ordering barrier |

**The minimal answer is a writer publication barrier on Power/ARM, with the stated reader's address dependence doing the read-side ordering; TSO needs neither extra hardware fence.** None of these choices repairs an invalid [pointer](../../../../../../pointer-computer-programming.md), premature [memory reclamation](../../../../../../memory-reclamation.md), or a [lost update](../../../../../../lost-update.md) between writers.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
