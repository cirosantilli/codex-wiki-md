# Binary numeral system

↑ **Parent:** [Positional notation](positional-notation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_numeral_system)

The binary numeral system is [positional notation](positional-notation.md) with [radix](radix.md) two. Each [binary digit](binary-digit.md) is zero or one, and its [place value](place-value.md) is a [power of two](power-of-two.md). A one includes that weight in the sum; a zero skips it. The [binary representation](binary-number.md) $11001101_2$ therefore selects $128,64,8,4,1$ and represents the [integer](integer-split.md) $205$.

To obtain those [binary digits](binary-digit.md) from $205$, repeatedly use [Euclidean division](euclidean-division.md) by two:

$$
\begin{aligned}
205&=2\cdot102+1,&102&=2\cdot51+0,\\
51&=2\cdot25+1,&25&=2\cdot12+1,\\
12&=2\cdot6+0,&6&=2\cdot3+0,\\
3&=2\cdot1+1,&1&=2\cdot0+1.
\end{aligned}
$$

The [remainders](remainder.md), in the order produced, are $1,0,1,1,0,0,1,1$. **Read them in reverse order to get $11001101_2$.** The final zero is the [quotient](quotient.md) that stops the conversion, not an additional leading [binary digit](binary-digit.md). Starting with zero itself needs the special single-digit representation $0_2$.

A useful independent check reads the [binary digits](binary-digit.md) from left to right. Start with $v=0$ and, for each [binary digit](binary-digit.md) $d$, replace $v$ by $2v+d$. For $11001101_2$, the intermediate values are $1,3,6,12,25,51,102,205$. This reconstructs the [integer](integer-split.md) without reversing a list and explains why appending a zero on the right doubles the value.

Binary is well suited to computation because each [binary digit](binary-digit.md) has just two possibilities. A stored [bit](bit.md) can encode either possibility; groups of [bits](bit.md) encode larger [integers](integer-split.md). Practical integer arithmetic can use a [radix](radix.md) that is itself a [power of two](power-of-two.md), grouping several [binary digits](binary-digit.md) into each stored [numeral digit](numerical-digit.md).[§3.3, p. 56: choice of a power-of-two base for stored integer digits](a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup.md) A displayed negative [integer](integer-split.md), such as $-11001101_2=-205_{10}$, uses a separate sign. A computer's particular signed storage convention is an additional encoding choice, so the displayed sign should not be confused with an extra binary place.

**Table of contents**

- [Binary digit](binary-digit.md)
  - [Most significant bit](most-significant-bit.md)
  - [Least significant bit](least-significant-bit.md)

## ↑ Ancestors (6)

1. [Positional notation](positional-notation.md)
2. [Integer](integer-split.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Cache line](cache-line.md)
- [Deterministic finite automaton](deterministic-finite-automaton.md)
- [Dynamic programming](dynamic-programming.md)
- [Floating-point arithmetic](floating-point-arithmetic-split.md)
- [Karatsuba multiplication](karatsuba-multiplication.md)
- [Outward rounding](outward-rounding.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/12f/solution.md)
- [Pseudo-polynomial time](pseudo-polynomial-time.md)
- [Two-level address translation](two-level-address-translation.md)
