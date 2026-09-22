<h1 id="4/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Place this [object method](../../../../../../object-method.md) inside the concrete class. Its [precondition](../../../../../../precondition.md) is the [representation invariant](../../../../../../representation-invariant.md); its [postcondition](../../../../../../postcondition.md) is that the [abstract data type](../../../../../../abstract-data-type.md) state is unchanged and its left-to-right contents have been printed in bracket notation followed by a newline:
```
def display: Unit = {
  print("[")
  var i = 0
  while (i < size) {
    if (i > 0) print(", ")
    print(a(slot(i)))
    i += 1
  }
  println("]")
}
```
Assume ordinary sequential execution and successful output. The [loop invariant](../../../../../../loop-invariant.md) is $0\leq i\leq size$, unchanged representation, and output consisting of `[` followed by precisely the first $i$ abstract values, separated by commas and spaces. The [loop variant](../../../../../../loop-variant.md) $size-i$ decreases. At exit the closing bracket completes the required display, including `[]` for emptiness. This takes $O(size+1)$ output operations and [constant space](../../../../../../constant-space.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [4](../../../4.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
