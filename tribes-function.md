# Tribes function

↑ **Parent:** [Boolean function](boolean-function.md)

A tribes function is an OR of AND blocks: partition $mw$ coordinates into $m$ blocks of size $w$, and let $f=1$ when at least one block consists entirely of ones. For [independent random variables](independent-random-variables.md) with each bit uniform, $\mathbb P(f=0)=(1-2^{-w})^m$. The [influence of a variable](influence-of-a-variable.md) is $2^{-(w-1)}(1-2^{-w})^{m-1}$, because every other bit in its block must be one and every other block must fail. Taking $m$ approximately $(\log2)2^w$ keeps both output probabilities bounded away from zero and gives influences of order $\log(mw)/(mw)$. This shows the order in the [Kahn-Kalai-Linial theorem](kahn-kalai-linial-theorem.md) is sharp.

**Table of contents**

- [Balanced tribes construction with unused coordinates](balanced-tribes-construction-with-unused-coordinates.md)
- [Tribes threshold window](tribes-threshold-window.md)

## ↑ Ancestors (7)

1. [Boolean function](boolean-function.md)
2. [Boolean hypercube](boolean-hypercube.md)
3. [Analysis of Boolean functions](analysis-of-boolean-functions.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Kahn-Kalai-Linial theorem](kahn-kalai-linial-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-7/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-13/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-82/4/solution.md)
