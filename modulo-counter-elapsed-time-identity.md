# Modulo-counter elapsed-time identity

↑ **Parent:** [Modular arithmetic](modular-arithmetic-split.md)

A free-running [digital counter](digital-counter.md) with modulus $M$ shows only the residue of elapsed ticks. If two observations differ by a true interval $d<M$, their modular difference is congruent to $d$ and is the unique representative in $\{0,\ldots,M-1\}$, proving the displayed identity. It handles a wrap between observations without a conditional branch. A complete elapsed modulus is indistinguishable from zero, so the interval bound is essential. For a $w$-bit timer at frequency $f$, the wrap period is $2^w/f$, and [unsigned integer arithmetic in C](unsigned-integer-arithmetic-in-c.md) can implement the difference directly on an appropriate type.

## ↑ Ancestors (5)

1. [Modular arithmetic](modular-arithmetic-split.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/digital-systems-linear-algebra-introduction-to-formal-proof/2/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/2/c/solution.md)
