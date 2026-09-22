<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Give the two waiting predicates different [semaphores](../../../../../../semaphore-programming.md). `empty` has one permit initially; `full` has zero. A writer takes the empty permit before touching the slot and transfers permission to a reader by releasing `full`. A reader does the reverse.

```
class SemaphoreMemory[T] extends Memory[T] {
  private val empty: Semaphore = new CountingSemaphore(1)
  private val full: Semaphore = {
    val s = new CountingSemaphore(1)
    s.down
    s
  }
  private var slot: Option[T] = None

  def write(msg: T): Unit = {
    empty.down
    slot = Some(msg)
    full.up
  }
  def read: T = {
    full.down
    val result = slot.get
    slot = None
    empty.up
    result
  }
}
```

For a single slot, a separate [mutex](../../../../../../mutex.md) around `slot` is unnecessary. There is a unique circulating permission: either an empty permit is available, a writer holds it, a full permit is available, or a reader holds it. During the transition the sum of available permits can be zero; it is never necessary to assert that it is always one. In particular, the next writer cannot start until the preceding reader has finished reading, cleared the slot and released `empty`.

The [monitor](../../../../../../monitor-synchronization.md) operations inside each [semaphore](../../../../../../semaphore-programming.md) also establish the required [happens-before](../../../../../../happens-before.md) relation: the write precedes `full.up`, and a successful subsequent `full.down` makes it visible to the reader. Likewise, the reader's clearing precedes the next writer's successful `empty.down`. Slot accesses therefore need no unsynchronized visibility assumption. The invariant is

$$
\boxed{\text{exactly one slot-access permission, alternating writer then reader}.}
$$

Only writers wait on `empty`, and only readers wait on `full`. With the single-notification [semaphore](../../../../../../semaphore-programming.md) implementation in part (a), a state change wakes at most one waiter of the appropriate kind, avoiding the [thundering herd](../../../../../../thundering-herd.md) of part (i). This is an efficiency improvement, not yet a first-come-first-served guarantee.

If one or more readers arrive before the first writer, they block on the initially unavailable `full` [semaphore](../../../../../../semaphore-programming.md). Their waits release its [monitor](../../../../../../monitor-synchronization.md), so they do not prevent a writer from obtaining the independent `empty` permit. The first write releases `full` and permits exactly one reader to take that value. Remaining readers wait for later writes; they never see uninitialized storage.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Concurrent programming](../../../../concurrent-programming-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
