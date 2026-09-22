<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use one [monitor](../../../../../../monitor-synchronization.md) to protect both the occupied flag and the slot. `Option` supplies an empty marker without confusing an empty slot with a valid `null` payload.

```
class MonitorMemory[T] extends Memory[T] {
  private var slot: Option[T] = None
  def write(msg: T): Unit = synchronized {
    while (slot.nonEmpty) wait()
    slot = Some(msg)
    notifyAll()
  }
  def read: T = synchronized {
    while (slot.isEmpty) wait()
    val result = slot.get
    slot = None
    notifyAll()
    result
  }
}
```

A writer changes empty to full while holding the [monitor](../../../../../../monitor-synchronization.md); a reader changes full to empty while holding the same [monitor](../../../../../../monitor-synchronization.md). The corresponding successful assignment or removal is its [linearization point](../../../../../../linearization-point.md). No second writer can overwrite a full slot, and no two readers can remove one value. Rechecking in a `while` handles [spurious wakeups](../../../../../../spurious-wakeup.md) and competition after notification.

There are two different waiting predicates on the same [monitor](../../../../../../monitor-synchronization.md): writers need empty, readers need full. A single arbitrary `notify` could wake a caller of the wrong kind. For example, after a reader empties the slot, waking another reader leaves it waiting again while a writer remains asleep, potentially stranding the computation. `notifyAll` prevents that [lost wake-up](../../../../../../lost-wake-up.md) pattern by allowing every waiter to recheck. Thus,

$$
\boxed{\text{one protected slot, two while-guarded waits, and notifyAll after either state change}.}
$$

With many users, each change wakes numerous [software threads](../../../../../../thread-computing.md) even though at most one can use that new slot state. Most reacquire the [monitor](../../../../../../monitor-synchronization.md), find their predicate false and sleep again. This [thundering herd](../../../../../../thundering-herd.md) wastes [context switches](../../../../../../context-switch.md) and lock acquisitions. It also supplies no fairness or arrival-order guarantee.

## ↑ Ancestors (12)

1. [I](../i.md)
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
