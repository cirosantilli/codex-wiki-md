<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let `r1:r0` hold the first operand, high limb first, and `r3:r2` the second. In [assembly language](../../../../../assembly-language.md) the addition can be written:

```
adds r0, r0, r2
adcs r1, r1, r3
```

The first instruction produces the low result and its [arithmetic carry](../../../../../carry-arithmetic.md); the second immediately consumes that [arithmetic carry](../../../../../carry-arithmetic.md) while adding the high limbs. No intervening flag-setting instruction is permitted.

For a [proof](../../../../../mathematical-proof.md), put $M=2^{32}$ and denote the input limbs by $X_1,X_0,Y_1,Y_0$. If the low addition gives $Z_0$ and [arithmetic carry](../../../../../carry-arithmetic.md) $c$, then $X_0+Y_0=Z_0+Mc$. The high addition gives $Z_1$ and final [arithmetic carry](../../../../../carry-arithmetic.md) $d$, so $X_1+Y_1+c=Z_1+Md$. Multiplying the second identity by $M$ and combining yields

$$
(MX_1+X_0)+(MY_1+Y_0)=MZ_1+Z_0+M^2d.
$$

**The [processor register](../../../../../processor-register.md) pair is the correct result [modulo](../../../../../modulo-operation.md) $2^{64}$**, and the final [arithmetic carry](../../../../../carry-arithmetic.md) records overflow beyond that unsigned width. If the mathematical sum fits in 64 [bits](../../../../../bit.md), no reduction changes it.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
