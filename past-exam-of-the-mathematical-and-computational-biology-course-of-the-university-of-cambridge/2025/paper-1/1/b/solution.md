<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

It performs a [trial division](../../../../../trial-division.md) test for a [prime number](../../../../../prime-number-split.md). An [integer](../../../../../integer-split.md) below $2$ is rejected; otherwise the function searches for a [divisor](../../../../../divisor.md) from $2$ through $\lfloor\sqrt n\rfloor$. A [composite number](../../../../../composite-number.md) has a [prime factor](../../../../../prime-factor.md) no larger than its [square root](../../../../../square-root.md), so finding no such [divisor](../../../../../divisor.md) proves [primality](../../../../../primality.md). For example, `mystery2(97)` returns **`True`**, while `mystery2(91)` returns **`False`**, since $91=7\cdot13$.

This describes the intended mathematical test. For extremely large [integers](../../../../../integer-split.md), the floating-point computation `n**0.5` can round or overflow; an implementation intended for arbitrary-size [integers](../../../../../integer-split.md) should use an exact [integer square root](../../../../../integer-square-root.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
