<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Traverse the whole original list once for each of its elements:
```
sml
fun scan [] = ()
  | scan (_ :: xs) = scan xs;

fun scanForEach [] whole = ()
  | scanForEach (_ :: rest) whole =
      (scan whole; scanForEach rest whole);

fun quadratic xs = scanForEach xs xs;
```
The outer [structural recursion](../../../../../../structural-recursion.md) runs $n$ times, and each `scan whole` visits $n$ constructors. In the ordinary source-evaluation cost model, **the [time complexity](../../../../../../time-complexity.md) is $\Theta(n^2)$**. This example counts executed traversals, without assuming an optimizing compiler that removes deliberately unused computations.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
