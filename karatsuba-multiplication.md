# Karatsuba multiplication

↑ **Parent:** [Algorithm](algorithm-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Karatsuba_multiplication)

[Karatsuba multiplication](karatsuba-multiplication.md) is a [divide-and-conquer algorithm](divide-and-conquer-algorithm.md) for [multiplication](multiplication.md) of [integers](integer-split.md). Splitting each operand into two blocks seems to require four smaller products; the [Karatsuba three-product identity](karatsuba-three-product-identity.md) recovers the two cross terms together from just three products. Repeating that saving through [recursion](recursion-computer-science.md) changes the [time complexity](time-complexity.md) from quadratic to $O(n^{\log_2 3})$, where $n$ counts digits in a fixed [positional notation](positional-notation.md). The exponent is about $1.585$: the benefit comes from the [algorithm](algorithm-split.md), even though each splitting step needs more [addition](addition.md) and [subtraction](subtraction.md).

The [Karatsuba worked multiplication](karatsuba-worked-multiplication.md) below computes $1234\cdot5678=7{,}006{,}652$ using $12\cdot56$, $34\cdot78$, and $46\cdot134$. The last operand already shows why “half-size” needs care: [Karatsuba carry handling](karatsuba-carry-handling.md) and [Karatsuba recursion termination](karatsuba-recursion-termination.md) account for the extra digit. [Karatsuba digit-operation cost](karatsuba-digit-operation-cost.md) states the operation model; [Karatsuba practical crossover](karatsuba-practical-crossover.md) explains why the asymptotic saving alone does not select a useful threshold.

The original 1962 paper presents a [binary numeral system](binary-numeral-system.md) automaton construction: its Theorem 2 and proof reduce [multiplication](multiplication.md) to taking [squares of numbers](square-of-a-number.md), then reduce a larger [square of a number](square-of-a-number.md) to three smaller [squares of numbers](square-of-a-number.md). Its footnote explicitly addresses the extra digit in a sum of halves. The sequential [time complexity](time-complexity.md) analysis below uses a different operation model from that paper's automaton size and depth bounds, including its [Boolean circuit](boolean-circuit.md) realization without feedback.[Karatsuba and Ofman, Multiplication of many-digital numbers by automatic computers, original Russian article, 1962, pp. 293–294: Theorem 2, its proof, and the footnote on p. 294](multiplication-of-many-digital-numbers-by-automatic-computers-by-a-karatsuba-and-yu-ofman.md)

**Table of contents**

- [Karatsuba operand splitting](karatsuba-operand-splitting.md)
- [Karatsuba three-product identity](karatsuba-three-product-identity.md)
- [Karatsuba worked multiplication](karatsuba-worked-multiplication.md)
- [Karatsuba carry handling](karatsuba-carry-handling.md)
- [Karatsuba recursion termination](karatsuba-recursion-termination.md)
- [Karatsuba digit-operation cost](karatsuba-digit-operation-cost.md)
- [Karatsuba practical crossover](karatsuba-practical-crossover.md)

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Divide-and-conquer algorithm](divide-and-conquer-algorithm.md)
- [Divide-and-conquer product ledger](divide-and-conquer-product-ledger.md)
- [Karatsuba multiplication](karatsuba-multiplication.md)
- [Karatsuba recursion termination](karatsuba-recursion-termination.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-124/3/ii/solution.md)
