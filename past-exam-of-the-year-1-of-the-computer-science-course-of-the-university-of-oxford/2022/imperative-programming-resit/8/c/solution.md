<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use an immutable [hash map](../../../../../hash-map.md) for the concrete value, omitting zero-count entries:

```
class CompleteMultiSetImp[T](initial: Map[T, Int]) extends CompleteMultiSet[T] {
  private val table = initial.filter { case (_, n) => n != 0 }
  override def count(t: T): Int = table.getOrElse(t, 0)
  override lazy val present: Seq[T] = table.keys.toVector
}

def cms[T](ts: T*): CompleteMultiSet[T] =
  new CompleteMultiSetImp[T](ts.distinct.map(t => (t, 1)).toMap)
```

The [abstraction function](../../../../../abstraction-function.md) is the map with implicit zero outside its keys. Immutable storage makes saved values independent of later operations, and the inherited defaults dispatch through the overridden `count` and `present`. A hash lookup has expected constant cost under ordinary hashing assumptions, with collision-dependent worst cases.

**Repeated arguments still get count one**, because the constructor first removes duplicates. All other elements have count zero, satisfying the intended stronger reading of the constructor specification. Treating `ts` as a bag and adding one for every repetition would implement a different operation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
