<h1 id="8/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the **[adapter pattern](../../../../../../adapter-pattern.md)**, keeping the existing component [software object](../../../../../../software-object.md) in both directions:

```
class PipeAsChannel(pipe: Pipe) extends Channel {
  override def apply(n: Int): Int = {
    pipe.consume(n)
    pipe.result
  }
}

class ChannelAsPipe(channel: Channel, initialResult: Int) extends Pipe {
  private var last = initialResult
  override def consume(n: Int): Unit = {
    last = channel(n)
  }
  override def result: Int = last
}
```

The first adapter feeds the input before reading the pipe's output. The second invokes the channel exactly once per consume and caches its returned output; subsequent result queries do not advance it. **Its initial result must be supplied explicitly**, because a general channel [object interface](../../../../../../object-interface.md) exposes no initial-output query. Calling the channel on a dummy input during construction would mutate arbitrary state and would invent behavior the [object interface](../../../../../../object-interface.md) does not promise.

These adapters preserve the sequential update/output behavior after each real input, assuming no interfering access to the wrapped component. They do not claim a perfect inverse for every aspect of the original [object interfaces](../../../../../../object-interface.md): pipe initialization is additional observable state, whereas a channel alone does not specify that observation.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
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
