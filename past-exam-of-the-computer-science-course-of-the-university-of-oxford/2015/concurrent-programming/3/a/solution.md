<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [counting semaphore](../../../../../counting-semaphore.md) holds a nonnegative number of permits. `down` waits until a permit is available and consumes one; `up` returns a permit and can release a waiting caller. A [binary semaphore](../../../../../binary-semaphore.md) restricts the number available to zero or one. Unlike a [mutex](../../../../../mutex.md), a [semaphore](../../../../../semaphore-programming.md) need not be released by the same [software thread](../../../../../thread-computing.md) that acquired it; this permits producer-to-consumer signalling.

Interpret `maxCount` as the initial number of permits and, for this bounded implementation, the maximum permitted number of unmatched releases. An `up` beyond that capacity is a programming error, rather than a blocking operation. Clients obey this release discipline. If an unbounded [counting semaphore](../../../../../counting-semaphore.md) is desired instead, remove the upper-bound requirement and use a sufficiently wide counter; a capacity-one instance is binary only under the corresponding balanced-use discipline.

```
class CountingSemaphore(maxCount: Int) extends Semaphore {
  require(maxCount > 0)
  private var count = maxCount
  def down: Unit = synchronized {
    while (count == 0) wait()
    count -= 1
  }
  def up: Unit = synchronized {
    require(count < maxCount, "unmatched semaphore release")
    count += 1
    notify()
  }
}
```

All accesses to `count` occur under the same [monitor](../../../../../monitor-synchronization.md). `wait` atomically releases that [monitor](../../../../../monitor-synchronization.md) while sleeping, then reacquires it before returning. The `while` is needed because of [spurious wakeups](../../../../../spurious-wakeup.md) and because another caller can consume the returned permit before the notified caller reacquires the [monitor](../../../../../monitor-synchronization.md). Only `down` callers wait here, and they all wait on the same predicate; hence waking one with `notify` is sufficient. A later `up` notifies another waiter if necessary. This use of `notify` will not be safe for the mixed predicates in the next part.[notify and wait: arbitrary notification choice, monitor reacquisition and spurious wakeups](../../../../../java-8-object-api-documentation.md)

A [binary semaphore](../../../../../binary-semaphore.md) initially available is `new CountingSemaphore(1)`. To initialize it unavailable, call its `down` once during construction, before publishing it to other [software threads](../../../../../thread-computing.md). Its state obeys

$$
\boxed{0\leq\mathrm{count}\leq\mathrm{maxCount};\quad\mathrm{down}:c\mapsto c-1\ (c>0),\quad\mathrm{up}:c\mapsto c+1.}
$$

This implementation provides no first-come-first-served guarantee: a new caller can acquire the [monitor](../../../../../monitor-synchronization.md) before a notified waiter. The following examples assume ordinary successful execution without cancellation or interruption of a partially completed buffer operation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Concurrent programming](../../../concurrent-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
