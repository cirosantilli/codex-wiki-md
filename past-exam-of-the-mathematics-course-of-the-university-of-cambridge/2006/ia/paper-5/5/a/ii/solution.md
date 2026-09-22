<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use a [two-list functional queue](../../../../../../../two-list-functional-queue.md). Its representation `(front, rear)` denotes the abstract sequence `front @ rev rear`; the front is nonempty unless the whole [FIFO queue](../../../../../../../fifo-queue.md) is empty. Normalize only when the front runs out:
```
sml
datatype 'a queue = Q of 'a list * 'a list;
exception EmptyQueue;

fun check ([], rear) = Q (rev rear, [])
  | check (front, rear) = Q (front, rear);

fun empty () = Q ([], []);
fun isEmpty (Q (front, _)) = null front;
fun enqueue x (Q (front, rear)) = check (front, x :: rear);

fun peek (Q ([], _)) = raise EmptyQueue
  | peek (Q (x :: _, _)) = x;

fun dequeue (Q ([], _)) = raise EmptyQueue
  | dequeue (Q (x :: front, rear)) = (x, check (front, rear));
```
Enqueue prepends to the reversed rear list. Removing the head either leaves a nonempty front or reverses the accumulated rear to restore the invariant. The result pair from `dequeue` contains the removed element and the new [FIFO queue](../../../../../../../fifo-queue.md). The constructor should be hidden behind an abstract interface so clients cannot construct an unnormalized representation that invalidates `isEmpty`.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Ia](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
