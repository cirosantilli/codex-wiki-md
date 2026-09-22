# Stack alignment

↑ **Parent:** [Call stack](call-stack.md)

[Stack alignment](stack-alignment.md) constrains the [stack pointer](stack-pointer.md) to a multiple of a specified byte boundary. [AAPCS32](aapcs32.md) requires word alignment generally and eight-byte alignment at public interfaces. Saving four 32-bit words preserves eight-byte alignment; saving three would change it by four bytes and may require padding before another call. Frame size and the alignment of local objects must be considered together.[Base standard, universal and public-interface stack constraints](procedure-call-standard-for-the-arm-architecture-by-arm-limited.md)

## ↑ Ancestors (5)

1. [Call stack](call-stack.md)
2. [Stack (data structure)](stack-data-structure.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/1/a/solution.md)
- [Stack alignment](stack-alignment.md)
