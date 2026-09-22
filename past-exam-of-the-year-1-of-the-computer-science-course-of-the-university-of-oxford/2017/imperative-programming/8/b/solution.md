<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Hypothetical covariance would allow the following unsound alias:

```
val narrow: MSet[Int] = new MSet[Int](Nil)
val wide: MSet[Any] = narrow       // hypothetical covariant conversion
wide.add("not an integer")
val n: Int = narrow.delete()      // would return the inserted string
```

The last value cannot satisfy its promised type. This is the [covariance failure for a mutable collection](../../../../../covariance-failure-for-a-mutable-collection.md): a broader consuming interface could insert values that violate a narrower alias's guarantee. The actual invariant `MSet[T]` rejects the conversion, and declaring `+T` while retaining `add(x: T)` is itself rejected by the [variance-position rule](../../../../../variance-position-rule.md). **The mutable read-and-write interface must remain invariant in `T`.**

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
