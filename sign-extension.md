# Sign extension

↑ **Parent:** [Two's complement](two-s-complement.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sign_extension)

To widen an $m$-[bit](bit.md) [two's complement](two-s-complement.md) [integer](integer-split.md) to $w>m$ [bits](bit.md), preserve the original low [bits](bit.md) and fill the new high positions with the old sign [bit](bit.md) $s$. The change in signed positional weights is $-s2^{w-1}+s\sum_{i=m-1}^{w-2}2^i=-s2^{m-1}$, so the represented signed value is unchanged. Zero extension instead preserves the [unsigned interpretation](unsigned-interpretation-of-a-bit-string.md), and changes the signed value of negative inputs.

## ↑ Ancestors (4)

1. [Two's complement](two-s-complement.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/digital-systems-linear-algebra-introduction-to-formal-proof/2/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/digital-systems-linear-algebra-introduction-to-formal-proof/1/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/digital-systems-linear-algebra-introduction-to-formal-proof/1/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/digital-systems-linear-algebra-introduction-to-formal-proof/1/c/ii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/2/b/solution.md)
- [Zero extension](zero-extension.md)
