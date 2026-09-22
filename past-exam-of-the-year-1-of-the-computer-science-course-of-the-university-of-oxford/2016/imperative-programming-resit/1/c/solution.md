<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [repeated squaring](../../../../../exponentiation-by-squaring.md), including index zero:
```
b2[0] := b; top := 0;
WHILE b2[top]*b2[top] <= n DO
  b2[top+1] := b2[top]*b2[top];
  top := top+1
END;
```
The [loop invariant](../../../../../loop-invariant.md) is $b_2[j]=b^{2^j}$ for $0\leq j\leq\mathrm{top}$, with $b_2[j]\leq n$ for every stored entry except possibly the initial entry when $b>n$. Squaring $b^{2^j}$ gives $b^{2^{j+1}}$, proving preservation. The first failed guard identifies the first larger power outside the range. If $b>n$, no power with $k\geq1$ needs storing.

**Index zero is deliberately included.** The original paper asks for indices $k\geq1$ but then claims that their products represent every allowable power. Taken without $b_2[0]=b$, that claim fails for odd exponents, since every available exponent would be even. The extra initialized entry makes the intended [binary expansion](../../../../../binary-expansion.md) argument valid without changing the requested entries.

Let $M$ be the largest representable positive [integer](../../../../../integer-split.md). The worst case is $b=2$, requiring indices through $\lfloor\log_2\lfloor\log_2 M\rfloor\rfloor$. Thus **`enough = 5` for signed 32-bit integers, or `6` for signed 64-bit integers**, suffices for stored powers that fit; a larger convenient constant is harmless. This counts slots starting at zero and does not reserve a slot for an out-of-range sentinel. The multiplication in the guard can still suffer [integer overflow](../../../../../integer-overflow.md), independently of this [array](../../../../../array-data-structure.md) capacity bound.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
