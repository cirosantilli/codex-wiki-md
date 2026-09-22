# Unsigned integer arithmetic in C

↑ **Parent:** [C programming language](c-programming-language.md)

For a $w$-bit unsigned [integer](integer-split.md) type without padding, [C programming language](c-programming-language.md) arithmetic on that type reduces results modulo $2^w$. In particular, subtracting two `uint32_t` timestamps gives their modular difference when that subtraction is evaluated in the 32-bit unsigned type. [Integer](integer-split.md) promotions must be checked for narrower types or unusual implementations. Signed [integer overflow](integer-overflow.md) has different rules and must not be treated as the same operation.[Section 6.2.5 paragraph 9 and Section 6.3.1.1](c11-committee-draft-n1570.md)

## ↑ Ancestors (4)

1. [C programming language](c-programming-language.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Modulo-counter elapsed-time identity](modulo-counter-elapsed-time-identity.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/2/c/solution.md)
