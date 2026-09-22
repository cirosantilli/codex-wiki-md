# Logical right shift

↑ **Parent:** [Bit shift](bit-shift.md)

A [logical right shift](logical-right-shift.md) moves [bits](bit.md) toward less significant positions, discards those shifted out, and fills the high positions with zero. On the [unsigned interpretation](unsigned-interpretation-of-a-bit-string.md) of a [machine word](machine-word.md), it computes the quotient in [integer division](integer-division.md) by $2^k$. Indeed, splitting the [binary representation](binary-number.md) after its lowest $k$ [bits](bit.md) gives $a=2^kq+r$ with $0\leq r<2^k$; the retained upper [bits](bit.md) represent $q$. A fixed-width [left bit shift](left-bit-shift.md) by $n-k$ followed by a [logical right shift](logical-right-shift.md) by $n-k$ extracts precisely the low $k$ [bits](bit.md), giving the remainder.

## ↑ Ancestors (4)

1. [Bit shift](bit-shift.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Byte-table population count](byte-table-population-count.md)
- [Logical right shift](logical-right-shift.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/digital-systems-linear-algebra-introduction-to-formal-proof/2/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof-resit/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/1/c/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/1/d/solution.md)
- [Thumb 16-bit instruction set quick reference by Arm](thumb-16-bit-instruction-set-quick-reference-by-arm.md)
