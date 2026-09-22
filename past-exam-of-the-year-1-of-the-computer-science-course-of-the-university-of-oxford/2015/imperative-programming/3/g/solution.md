<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Extend the data [linked list node](../../../../../linked-list-node.md) type by a [real number](../../../../../real-number.md) field and compare that field through an [Oberon](../../../../../oberon-programming-language.md) [type guard](../../../../../type-guard.md).
```
TYPE RealNode = RECORD (Node) value: REAL END;
     RealTail = POINTER TO RealNode;

PROCEDURE RealLess(p, q: Tail): BOOLEAN;
BEGIN
  RETURN p(RealTail).value < q(RealTail).value
END RealLess;
```
Construct the data chain from `RealTail` nodes, retain the ordinary `Header` for its header, set its count correctly, and call
```
MergeSort(RealLess, p)
```
Only data nodes reach `RealLess`, so the header needs no real-valued field. Its [precondition](../../../../../precondition.md) is that every data node has the `RealNode` extension. With ordinary [real numbers](../../../../../real-number.md), the comparison supplies a [total order](../../../../../total-order.md); machine values such as `NaN` must be excluded if the machine [floating-point number](../../../../../floating-point-number.md) type admits them.

$$
\boxed{\mathrm{RealLess}(p,q)\iff p.\mathrm{value}<q.\mathrm{value};\quad\mathrm{MergeSort}(\mathrm{RealLess},p).}
$$

## ↑ Ancestors (12)

1. [G](../g.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
