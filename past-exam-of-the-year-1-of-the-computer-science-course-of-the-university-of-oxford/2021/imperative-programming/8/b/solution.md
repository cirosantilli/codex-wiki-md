<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Feed each returned output back as the next input to the same channel [software object](../../../../../software-object.md):

```
class RepeatedChannel(inner: Channel, times: Int) extends Channel {
  require(times > 0)
  override def apply(n: Int): Int = {
    var value = n
    var completed = 0
    while (completed < times) {
      value = inner(value)
      completed += 1
    }
    value
  }
}
```

The [loop invariant](../../../../../loop-invariant.md) says that `value` and the component's current state are exactly those after `completed` successive applications starting from this invocation's input and the entry state. The [loop variant](../../../../../loop-variant.md) is `times - completed`. On exit the specified number of applications has occurred; the component is not reset or replaced between them.

For input one and a freshly created sum channel, the successive outputs are

$$
1,\ 2,\ 3,\ 5,\ 8,\ 13,\ 21,\ 34,\ 55,\ \boxed{89}.
$$

Initially the component's previous input is zero. The first output is one; on each later call its previous-input state is the input used on the preceding call. Consequently outputs follow the [Fibonacci recurrence](../../../../../fibonacci-recurrence.md) with initial outputs one and two. The answer is **89**, rather than the result of repeatedly supplying the unchanged external input or recreating the component at every iteration. The component retains its final state for later wrapper calls.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
