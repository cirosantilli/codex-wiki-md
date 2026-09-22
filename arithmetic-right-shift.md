# Arithmetic right shift

↑ **Parent:** [Bit shift](bit-shift.md)

An [arithmetic right shift](arithmetic-right-shift.md) propagates the sign [bit](bit.md) into the vacated high positions. For a signed [two's complement](two-s-complement.md) [integer](integer-split.md), its result is division by $2^k$ rounded down. This differs from [C integer division](c-integer-division.md) on negative nonmultiples of $2^k$, because that quotient truncates towards zero. Shifting an $n$-[bit](bit.md) word arithmetically by $n-1$ produces zero for a nonnegative value and the all-one word, representing $-1$, for a negative value.

## ↑ Ancestors (4)

1. [Bit shift](bit-shift.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Arithmetic right shift](arithmetic-right-shift.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/1/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/1/e/solution.md)
- [Signed power-of-two division by biasing](signed-power-of-two-division-by-biasing.md)
- [Thumb 16-bit instruction set quick reference by Arm](thumb-16-bit-instruction-set-quick-reference-by-arm.md)
