<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use an abstract finite [sequence](../../../../../sequence.md) $s$ of [integers](../../../../../integer-split.md), initially empty. In the following [trait](../../../../../trait.md), comments are the mathematical specification; $s_0$ means the abstract state on entry, and `result` means the returned value.
```
trait ReversableBuffer {
  // Abstract state s: finite sequence of Int, initially [].

  // Pre: true. Post: s = s0 ++ [x].
  def append(x: Int): Unit

  // Pre: true. Post: s = [x] ++ s0.
  def prepend(x: Int): Unit

  // Pre: 0 <= i < length(s0).
  // Post: result = s0 !! i,
  //       s = take i s0 ++ drop (i+1) s0.
  def get(i: Int): Int

  // Pre: true. Post: s = reverse(s0).
  def rev: Unit
}
```
The [postcondition](../../../../../postcondition.md) of `get` includes removal: it is not merely indexed reading. In particular,

$$
\boxed{\operatorname{get}(i)\text{ returns }s_{0,i}\text{ and deletes exactly that occurrence}.}
$$

Repeated equal values elsewhere in the [sequence](../../../../../sequence.md) remain present. [List concatenation](../../../../../list-concatenation.md), indexing and [list reversal](../../../../../list-reversal.md) in the specification describe abstract behavior without committing to a physical representation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
