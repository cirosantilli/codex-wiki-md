<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Represent a [binary semaphore](../../../../../binary-semaphore.md) by a two-element [list](../../../../../list-abstract-data-type.md) containing the addresses of its busy flag and its waiting [FIFO queue](../../../../../fifo-queue.md). A blocked [continuation](../../../../../continuation-computer-science.md) belongs to the waiting [FIFO queue](../../../../../fifo-queue.md), not the scheduler's runnable [FIFO queue](../../../../../fifo-queue.md). These definitions extend the `FunMem` scheduler from the preceding part:

```
val semaphore() =
  let val busy = new() in
  let val waiting = new() in
    busy := false; waiting := nil; busy : waiting : nil;

val acquire(s) =
  let val busy = head(s) in
  let val waiting = head(tail(s)) in
    if !busy then
      callcc(lambda (blocked)
        waiting := append(!waiting,blocked:nil); dispatch())
    else (busy := true; nil);

val release(s) =
  let val busy = head(s) in
  let val waiting = head(tail(s)) in
    if !waiting = nil then (busy := false; nil)
    else let val next = head(!waiting) in
      waiting := tail(!waiting); enqueue(next); nil
```

A newly created [semaphore](../../../../../semaphore-programming.md) is free. Acquiring it while free marks it busy and immediately returns `nil`. Acquiring it while busy captures the remainder of the caller, appends that [continuation](../../../../../continuation-computer-science.md) to the waiting [FIFO queue](../../../../../fifo-queue.md), and dispatches a runnable computation. No runnable copy of the blocked caller is retained.

When a waiting caller exists, `release` keeps the busy flag true: the released permit is reserved for that caller. It removes exactly one waiting [continuation](../../../../../continuation-computer-science.md) and appends it to the scheduler's runnable [FIFO queue](../../../../../fifo-queue.md). It does not invoke `dispatch`, so the releasing computation keeps running. A newcomer cannot steal the reserved permit during the interval before the released caller resumes. That caller's captured [continuation](../../../../../continuation-computer-science.md) resumes after `acquire` with `nil`, already possessing the permit.

$$
\boxed{\begin{array}{ll}
\text{free acquire:}&\text{mark busy and continue};\\
\text{busy acquire:}&\text{block outside the runnable queue};\\
\text{release with waiter:}&\text{keep busy and enqueue one waiter};\\
\text{release without waiter:}&\text{mark free}.
\end{array}}
$$

These are [FIFO semaphores](../../../../../fifo-semaphore.md); the question only requires selecting one waiter, so choosing the oldest is a valid stronger discipline. The updates contain no suspension except at the explicit blocking point, making them atomic relative to this [cooperative multitasking](../../../../../cooperative-multitasking.md) scheduler. As allowed in the paper, invalid releases and executions in which every remaining computation is blocked need no error handling; the latter are [deadlocks](../../../../../deadlock.md), not a way to make progress.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Principles of programming languages](../../../principles-of-programming-languages-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
