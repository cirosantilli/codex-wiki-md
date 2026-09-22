# Byte-table population count

↑ **Parent:** [Hamming weight](hamming-weight.md)

Store the [Hamming weight](hamming-weight.md) of each possible [byte](byte.md) in a 256-entry table. Extract each byte of a word by a [logical right shift](logical-right-shift.md) and a [bit mask](bit-mask.md), then sum its table entries. The byte positions partition the word's bits, proving the formula. A 32-bit word needs four lookups, which can be unrolled. Logical extraction does not depend on the [endianness](endianness.md) of a stored word. The speed advantage depends on table-access costs as well as instruction counts.

## ↑ Ancestors (7)

1. [Hamming weight](hamming-weight.md)
2. [Linear code](linear-code.md)
3. [Coding theory](coding-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof-resit/1/b/solution.md)
