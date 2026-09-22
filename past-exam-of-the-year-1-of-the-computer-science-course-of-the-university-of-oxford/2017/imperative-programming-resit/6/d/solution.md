<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a covariant element type and a lower type bound when adding potentially more general elements:

```
class VendingMachine[+A](val currentItem: Option[A], items: List[A]) {
  def this(items: List[A]) = this(None,items)
  def dispenseNext(): VendingMachine[A] = items match {
    case Nil =>
      if (currentItem.isDefined) new VendingMachine[A](None,Nil)
      else this
    case t :: ts => new VendingMachine[A](Some(t),ts)
  }
  def addAll[B >: A](newItems: List[B]): VendingMachine[B] =
    new VendingMachine[B](items ++ newItems)
}
```

The [lower type bound](../../../../../lower-type-bound.md) permits the old pending elements of type `A` to be used as type `B`, so concatenation is type-correct. The resulting machine is immutable and can return the wider type without changing the existing machine. With the given client expressions, `VM1` has type `VendingMachine[Juice]` and `VM2` can have type `VendingMachine[Drink]`. The supplied `addAll` body constructs a new pending-item machine; its constructor sets `currentItem` to `None`.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
