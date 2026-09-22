<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual unit-cost model for [Standard ML](../../../../../../standard-ml.md) list constructors and fixed-size arithmetic. The input size $n$ in the list examples is the number of list elements, rather than the size of the integer entries. Inspecting only the first constructor has constant [time complexity](../../../../../../time-complexity.md):
```
sml
fun firstOrZero [] = 0
  | firstOrZero (x :: _) = x;
```
No tail is traversed. **The running time is $\Theta(1)$.**

## ↑ Ancestors (11)

1. [A](../a.md)
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
