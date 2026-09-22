<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $M=2^n$ for an $n$-bit [processor register](../../../../../processor-register.md). The [carry flag](../../../../../carry-flag.md) for addition satisfies **$\operatorname{bin}(x)+\operatorname{bin}(y)=\operatorname{bin}(z)+MC$**: the result retains the low $n$ [bits](../../../../../bit.md) and $C=1$ records an [arithmetic carry](../../../../../carry-arithmetic.md) beyond them.

For the [ARM architecture family](../../../../../arm-architecture-family.md) subtraction convention, **$\operatorname{bin}(x)-\operatorname{bin}(y)=\operatorname{bin}(z)-M(1-C)$**. Thus $C=1$ means _no borrow_, equivalently the unsigned minuend is at least the subtrahend. This flag is different from signed overflow: an [arithmetic carry](../../../../../carry-arithmetic.md) decision is not a test of the signed result.

## ↑ Ancestors (12)

1. [B](../b.md)
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
