<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The following method belongs inside the source class and uses the helper from part (d). It preserves the existing outgoing count, and a newly encountered user starts with exactly one incoming and zero outgoing payments.

```
def recordIncoming(user: Int): Unit = {
  require(1 <= user && user <= 99999999, "invalid user identity")
  val bucket = hash(user)
  val p = find(user, table(bucket))
  if (p == null) {
    table(bucket) = new PaymentsHash.Node(user, 1, 0, table(bucket))
  } else {
    require(p.countIn < Int.MaxValue, "incoming count is full")
    p.countIn += 1
  }
}
```

On a hit, exactly one field is incremented after the overflow check. On a miss, inserting at the bucket head preserves all existing records and gives precisely the required change from implicit zero to one. The given [hash function](../../../../../hash-function.md) must return an index in $[0,N)$ consistently for a given user. Its actual formula is not needed by this method. The nested private node class is accessible to its [companion class](../../../../../companion-class.md) in Scala, so retaining the source's `PaymentsHash.Node` visibility is valid.[Modifiers: private members are accessible to the enclosing template and its companion](../../../../../scala-2-13-classes-and-objects-specification.md)

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
