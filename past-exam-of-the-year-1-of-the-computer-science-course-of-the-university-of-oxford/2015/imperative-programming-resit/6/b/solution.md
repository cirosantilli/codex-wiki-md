<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Maintain one [frequency count](../../../../../frequency-count.md) for each lowercase alphabet character. Update only after a successful delegated operation:
```
trait CharTrackPlugIn extends Doc {
  private val counts = Array.fill[Int](26)(0)

  private def lower(x: Char): Boolean = 'a' <= x && x <= 'z'

  abstract override def insert(x: Char, pos: Int): Unit = {
    super.insert(x, pos)
    if (lower(x)) counts(x - 'a') += 1
  }

  abstract override def delete(pos: Int): Char = {
    val old = super.delete(pos)
    if (lower(old)) counts(old - 'a') -= 1
    old
  }

  def getCount(x: Char): Int = {
    assert('a' <= x && x <= 'z')
    counts(x - 'a')
  }
}
```
For an initially empty underlying implementation that inserts the character it receives and returns the character actually deleted, the [representation invariant](../../../../../representation-invariant.md) is

$$
\mathrm{counts}(j)=\#\{i:0\leq i<\operatorname{size},\ \operatorname{read}(i)=\texttt{'a'}+j\},\quad0\leq j<26.
$$

Insertion increases exactly one applicable [frequency count](../../../../../frequency-count.md), and deletion decreases the count of the returned character. Uppercase and nonletter characters contribute nothing. Exceptions from failed underlying operations leave the counters unchanged. The [stackable trait modification](../../../../../stackable-trait-modification.md) uses `abstract override` because it delegates to a concrete implementation elsewhere in the mixin chain.[Modifiers, abstract override; Inheritance](../../../../../scala-2-11-classes-and-objects-specification.md)

$$
\boxed{\operatorname{getCount}:\Theta(1),\qquad\text{extra storage: }26\text{ counters}.}
$$

The counters depend on the character seen by this [trait](../../../../../trait.md). A later [trait](../../../../../trait.md) that transforms characters can break the stated underlying-operation assumption; part (d) deliberately exposes that order dependence.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
