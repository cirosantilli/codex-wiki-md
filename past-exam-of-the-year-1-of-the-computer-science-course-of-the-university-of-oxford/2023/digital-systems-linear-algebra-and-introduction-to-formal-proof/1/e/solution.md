<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the same bias, then an [arithmetic right shift](../../../../../arithmetic-right-shift.md) by ten:
```
div1024:
    asrs r3, r0, #31    // -1 when a<0, otherwise 0
    lsrs r3, r3, #22    // b = 1023 when a<0, otherwise 0
    adds r0, r0, r3     // a+b, representable for every signed input
    asrs r0, r0, #10    // floor((a+b)/1024)
    bx lr
```
An [arithmetic right shift](../../../../../arithmetic-right-shift.md) of a [two's complement](../../../../../two-s-complement.md) [integer](../../../../../integer-split.md) computes division rounded down. For $a\geq0$, this already equals truncation towards zero. For $a<0$, the [signed power-of-two division by biasing](../../../../../signed-power-of-two-division-by-biasing.md) identity is

$$
\boxed{\operatorname{trunc}(a/1024)=\left\lfloor\frac{a+1023}{1024}\right\rfloor.}
$$

Indeed, writing $-a=1024q+r$ with $0\leq r<1024$ makes the adjusted numerator $-1024q+(1023-r)$; its quotient rounded down is $-q$ for every $r$, including zero. Thus the code returns the signed quotient in all cases and contains no data-dependent branch. The final `bx lr` simply returns to the caller.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [1](../../1.md)
3. [Digital systems](../../digital-systems.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
