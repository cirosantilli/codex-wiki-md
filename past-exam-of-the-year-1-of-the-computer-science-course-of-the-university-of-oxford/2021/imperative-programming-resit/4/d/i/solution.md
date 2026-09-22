<h1 id="4/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Add this method inside the concrete class:
```
def display: Unit = {
  print("[")
  var current = first
  var separator = ""
  while (current != null) {
    print(separator)
    print(current.datum)
    separator = ", "
    current = current.next
  }
  println("]")
}
```
Its [precondition](../../../../../../precondition.md) is a valid receiver, including an empty one. Its [postcondition](../../../../../../postcondition.md) leaves $q=q_0$ and prints the entries of $q_0$ from left to right in the displayed bracket format, followed by a newline. The [loop invariant](../../../../../../loop-invariant.md) says that the printed entries are precisely the chain before `current`; the not-yet-printed entries are the chain starting there. Advancing along the acyclic chain terminates after its length. Printing changes the output stream, but it changes neither links nor payloads.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [4](../../../4.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
