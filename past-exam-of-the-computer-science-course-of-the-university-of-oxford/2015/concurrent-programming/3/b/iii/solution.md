<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A [FIFO semaphore](../../../../../../fifo-semaphore.md) must reserve a released permit for the oldest waiter. Merely waking the oldest caller is insufficient if a newcomer can consume the permit first. Keep an explicit [FIFO queue](../../../../../../fifo-queue.md) of private wait records, and transfer the permit directly to the oldest record. Each record has its own [monitor](../../../../../../monitor-synchronization.md), so releasing a permit wakes exactly its chosen recipient.

```
class FifoBinarySemaphore(initiallyAvailable: Boolean) extends Semaphore {
  private final class Waiter { var granted = false }
  private val queue = scala.collection.mutable.Queue[Waiter]()
  private var available = initiallyAvailable

  def down: Unit = {
    val mine: Option[Waiter] = synchronized {
      if (available) {
        assert(queue.isEmpty)
        available = false
        None
      } else {
        val w = new Waiter
        queue.enqueue(w)
        Some(w)
      }
    }
    mine.foreach { w =>
      var interrupted = false
      w.synchronized {
        while (!w.granted) {
          try { w.wait() }
          catch { case _: InterruptedException => interrupted = true }
        }
      }
      if (interrupted) Thread.currentThread().interrupt()
    }
  }

  def up: Unit = synchronized {
    if (queue.nonEmpty) {
      val w = queue.dequeue()
      // available stays false: this permit is reserved for w.
      w.synchronized {
        w.granted = true
        w.notify()
      }
    } else {
      require(!available, "unmatched binary-semaphore release")
      available = true
    }
  }
}
```

The wait loop is deliberately uninterruptible with interruption status restored after acquisition: abandoning a queued wait record would otherwise strand its reserved permit. A caller that acquires must still complete the buffer operation. `granted` is read and written under the wait record's own [monitor](../../../../../../monitor-synchronization.md). The persistent flag prevents a [lost wake-up](../../../../../../lost-wake-up.md) if `up` runs after registration but before the caller begins waiting. [Spurious wakeups](../../../../../../spurious-wakeup.md) simply repeat the loop.

The outer [monitor](../../../../../../monitor-synchronization.md) serializes registration and the [FIFO queue](../../../../../../fifo-queue.md). A caller either consumes a genuinely free permit when nobody is queued, or appends one record. `up` removes exactly the front record and leaves `available` false, even if its owner has not yet resumed. A newcomer must queue behind existing records instead of stealing the handoff. The outer-to-inner [lock ordering](../../../../../../lock-ordering.md) in `up` is safe because waiting callers release the outer [monitor](../../../../../../monitor-synchronization.md) before acquiring their private [monitors](../../../../../../monitor-synchronization.md); no caller holds a private [monitor](../../../../../../monitor-synchronization.md) while trying to reacquire the outer one.

Now use the same buffer body as in (ii), replacing only the initialization of its two fields:

```
private val empty: Semaphore = new FifoBinarySemaphore(true)
private val full: Semaphore = new FifoBinarySemaphore(false)
```

This is a complete implementation when inserted in `SemaphoreMemory`: its `write` and `read` methods remain exactly the displayed methods. Pending writers obtain empty-slot permissions in registration order on `empty`; pending readers obtain full-slot permissions in registration order on `full`. Each handoff permits just one caller to access the slot, so

$$
\boxed{\text{writers are FIFO among writers, and readers are FIFO among readers}.}
$$

First-come-first-served means the order in which concurrent calls register under the [monitor](../../../../../../monitor-synchronization.md); two overlapping calls have no externally determined order. The guarantee is separate for the two kinds of caller. A global order combining reads and writes cannot be required: an initial read must wait while a later write supplies its value. Subject to eventual scheduling and the arrival of matching operations of the opposite kind, no registered caller is overtaken by a later caller of its own kind. The design avoids broadcast wakeups as well as barging.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
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
