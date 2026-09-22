<h1 id="8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Override the operation and scale the result of exactly one superclass call:

```
class ScaledSumChannel(factor: Int) extends SumChannel {
  override def apply(n: Int): Int = factor * super.apply(n)
}
```

The superclass updates its previous-input state once and returns its ordinary sum; only that returned value is scaled. **The inputs and superclass history are unchanged by the scaling.** Reimplementing the state update is unnecessary and could accidentally diverge from the superclass contract. As in the supplied channel, arithmetic uses the declared fixed-width [integer](../../../../../../integer-split.md) type.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
