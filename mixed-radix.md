# Mixed radix

↑ **Parent:** [Radix](radix.md)

A positional representation in which each digit has its own positive [integer](integer-split.md) base. Least-significant-first digits satisfy $0\leq x_i<b_i$, and digit $i$ has weight $\prod_{j<i}b_j$. For $k$ positions, assume $0\leq n<\prod_{i=0}^{k-1}b_i$. Repeated [Euclidean division](euclidean-division.md) by the successive bases converts that [integer](integer-split.md) to digits; a backwards version of [Horner's method](horner-s-method.md) converts the digits back.

## ↑ Ancestors (7)

1. [Radix](radix.md)
2. [Positional notation](positional-notation.md)
3. [Integer](integer-split.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/imperative-programming/1/a/solution.md)
