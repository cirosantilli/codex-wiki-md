# Subtract with carry

↑ **Parent:** [Carry flag](carry-flag.md)

With the [ARM architecture family](arm-architecture-family.md)'s no-borrow convention, [subtract with carry](subtract-with-carry.md) forms $X-Y-(1-C_{\rm in})$. The same [adder](adder.md) used for addition can form $X+(2^n-1-Y)+C_{\rm in}$. If its output is $Z+2^nC_{\rm out}$, rearranging proves $X-Y-(1-C_{\rm in})=Z-2^n(1-C_{\rm out})$. Thus complementing the second operand implements both the result and the correctly chained borrow information.[Page 1, Subtract with carry](thumb-16-bit-instruction-set-quick-reference-by-arm.md)

## ↑ Ancestors (5)

1. [Carry flag](carry-flag.md)
2. [Processor register](processor-register.md)
3. [Central processing unit](central-processing-unit.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/1/d/solution.md)
- [Subtract with carry](subtract-with-carry.md)
