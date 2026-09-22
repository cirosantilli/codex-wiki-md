<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Adapt one machine update into one forward [iterator](../../../../../iterator.md) element, then apply the skipping [iterator](../../../../../iterator.md) of part (a) with $n=\mathrm{step}-1$ and the [bidirectional iterator](../../../../../bidirectional-iterator.md) of part (b). Require a positive step and reset once on construction.
```
trait StateMachineIter[T] extends StateMachine[T] {
  def getBiIter(step: Int): BiIter[T] = {
    require(step > 0)
    val machine = this
    machine.reset()
    val everyUpdate = new Iter[T] {
      def hasNext: Boolean = !machine.shouldStop
      def next(): T = {
        if (!hasNext)
          throw new NoSuchElementException("StateMachine.next")
        machine.update()
        machine.getValue
      }
    }
    genBiIter(skipIter(everyUpdate, step-1))
  }
}
```
After $j$ forward results at the unexplored frontier, the returned value is the machine's value after exactly $j\,\mathrm{step}$ updates. A partial final block contributes no element, and `update` is never called after `shouldStop` becomes true. For the printed `Add` example, the first three observed states are

$$
\boxed{1+2=3,\quad1+2+3+4=10,\quad1+2+3+4+5+6=21.}
$$

Because the [state machine](../../../../../state-machine.md) interface exposes no copy or rollback operation, determining whether enough updates remain generally requires executing them. Thus `hasNext` may advance the physical machine and cache the next observation. Backward traversal replays stored observations; it does not undo machine effects. This is a trace [iterator](../../../../../iterator.md), with the ordinary cursor semantics of part (b). Assume exclusive use of the machine while this [iterator](../../../../../iterator.md) is active, and that returned values remain valid observations rather than mutable views overwritten by later updates.

Each physical update is executed at most once. Previously observed values can be revisited without rerunning the machine, and repeated `hasNext` calls do not perform duplicate updates once the next result is prepared.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
