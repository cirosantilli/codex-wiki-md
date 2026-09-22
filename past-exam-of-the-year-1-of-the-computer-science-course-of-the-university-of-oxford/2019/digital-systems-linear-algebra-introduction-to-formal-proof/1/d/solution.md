<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A [subtract with carry](../../../../../subtract-with-carry.md) instruction consumes the _no-borrow_ [carry flag](../../../../../carry-flag.md). Its arithmetic is **$Z=X-Y-(1-C_{\mathrm{in}})\pmod{2^{32}}$**. Hence a low-limb `subs` followed immediately by a high-limb `sbcs` propagates exactly the low subtraction's borrow.

For example, with the same limb assignment as in (c):

```
subs r0, r0, r2
sbcs r1, r1, r3
```

It uses an ordinary 32-bit [adder](../../../../../adder.md) by complementing every [bit](../../../../../bit.md) of the subtrahend and adding the incoming [arithmetic carry](../../../../../carry-arithmetic.md). For $M=2^{32}$, the unreduced [adder](../../../../../adder.md) sum is

$$
X+(M-1-Y)+C_{\mathrm{in}}.
$$

If this is $Z+MC_{\mathrm{out}}$, rearrangement gives $X-Y-(1-C_{\mathrm{in}})=Z-M(1-C_{\mathrm{out}})$. Thus both the result and outgoing no-borrow flag have the required meanings. With incoming [arithmetic carry](../../../../../carry-arithmetic.md) one this becomes ordinary subtraction.[Page 1, Add with carry and Subtract with carry: subtraction subtracts NOT C-bit](../../../../../thumb-16-bit-instruction-set-quick-reference-by-arm.md)

## ↑ Ancestors (12)

1. [D](../d.md)
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
