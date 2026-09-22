<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Replace the overloaded entry point by one forwarding method and add a virtual callback on the drink. The callbacks choose a reaction overload using the concrete drink class's statically known `this` type:

```
class Drink {
  def serveTo(b: Boy): Unit = b.react(this)
}
class Milk extends Drink {
  override def serveTo(b: Boy): Unit = b.react(this)
}
class Boy {
  def concept(d: Drink): Unit = d.serveTo(this)
  def react(d: Drink): Unit = println("Drink")
  def react(m: Milk): Unit = println("Milk")
}
class Baby extends Boy {
  override def react(d: Drink): Unit = println("Food")
  override def react(m: Milk): Unit = println("White drink")
}
```

The original `b.concept(d)` call now dynamically selects `Milk.serveTo`. Inside that method `this` has static type `Milk`, selecting `react(Milk)`; virtual dispatch on `b` then selects `Baby.react(Milk)`. Thus the output is **`White drink`**. This is [double dispatch](../../../../../double-dispatch.md): changing only an overload's parameter name or the reference's runtime object would not change static overload selection.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
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
