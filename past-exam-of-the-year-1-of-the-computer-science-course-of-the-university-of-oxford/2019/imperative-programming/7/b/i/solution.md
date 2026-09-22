<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The constructor stores a reference, not a copy:
```
val d = new Dimension(3, 4)
val f = new Frame(d)
d.width = 10
```
Now **`f.area` is still $12$, but the product of its stored dimension fields is $40$**. Even without retaining `d`, a client can break the same invariant through `f.dimension.height = 9`, because the accessor exposes the same mutable object. This is [representation exposure](../../../../../../representation-exposure.md) through [reference aliasing](../../../../../../reference-aliasing.md). A `val` prevents reassigning the reference; it does not freeze the referenced object.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
