<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Represent zero by one digit. Since `int_part` is nonnegative, a logical right shift is exactly [integer division](../../../../../integer-division.md) by two:
```
var digits = 1
var scratch = int_part
while (scratch >= 2) {
  scratch = scratch >>> 1
  digits += 1
}
```
The [loop invariant](../../../../../loop-invariant.md) is $digits\geq1$ and $scratch=\lfloor int\_part/2^{digits-1}\rfloor$; for positive `int_part`, also $scratch\geq1$. The [loop variant](../../../../../loop-variant.md) is `scratch`, strictly decreased whenever the guard holds. On exit, a positive input has $scratch=1$, yielding $2^{digits-1}\leq int\_part<2^{digits}$. Therefore **`digits` is the required width**, including width one for zero. Shifting avoids an explicit multiplication or division in the code. This uses the supplied assumption that `dec.toInt` really is the mathematical floor; saturating or invalid conversions are not covered by that assumption.

## ↑ Ancestors (12)

1. [C](../c.md)
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
