<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Extract low bits and fill the [integer](../../../../../integer-split.md) positions from right to left:
```
var remaining = int_part
var pos = digits - 1
while (pos >= 0) {
  res(pos) = if ((remaining & 1) == 0) '0' else '1'
  remaining = remaining >>> 1
  pos -= 1
}
```
At the start of an iteration, the [loop invariant](../../../../../loop-invariant.md) says that positions $pos+1,\ldots,digits-1$ contain the correct low bits and

$$
int\_part=remaining\,2^{digits-1-pos}
+\sum_{t=pos+1}^{digits-1}(res(t)-\mathtt{'0'})2^{digits-1-t}.
$$

The bitwise AND extracts the remainder modulo two; the shift supplies its quotient. These two facts preserve the [loop invariant](../../../../../loop-invariant.md). The [loop variant](../../../../../loop-variant.md) is $pos+1$. The width established in part (c) ensures that `remaining` is zero at exit, so **the first `digits` entries encode the whole [integer](../../../../../integer-split.md) part**. For zero the single entry becomes `'0'`. There are no explicit multiplications or divisions, and no extra digit [array](../../../../../array-data-structure.md) is needed.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
