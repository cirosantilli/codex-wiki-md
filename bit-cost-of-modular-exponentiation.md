# Bit cost of modular exponentiation

↑ **Parent:** [Modular exponentiation](modular-exponentiation.md)

The [binary powering multiplication count](binary-powering-multiplication-count.md) counts [arithmetic operations](arithmetic-operation.md). The [time complexity](time-complexity.md) measured in operations on individual [bits](bit.md) also depends on operand lengths. Put $L=\lfloor\log_2m\rfloor+1$, the binary length of the modulus, and let $\ell$ be the positive exponent's binary length. Stored residues use at most $L$ [bits](bit.md), and an unreduced product uses at most $2L$ [bits](bit.md).

With ordinary long [multiplication](multiplication.md) and [division with remainder](euclidean-division.md), one modular product costs $O(L^2)$ operations on [bits](bit.md). Combining that cost with $O(\ell)$ modular products gives

$$
\text{bit cost of the powering loop}=O(\ell L^2).
$$

This bound includes reductions in the loop, and assumes the base has already been reduced and the exponent is available as a [binary expansion](binary-expansion.md). Reading the exponent takes $O(\ell)$ additional work; initial reduction of a very long base depends on its input length, and an inverse for a negative exponent adds further work. More generally, if a modular product costs $R(L)$ operations on [bits](bit.md), the powering loop costs $O(\ell R(L))$. Faster [multiplication](multiplication.md) and reduction methods can improve the quadratic bound.[Section 3.3.5, pp. 62–63, Theorem 3.3: operand-length costs; Section 3.4, p. 65: modular multiplication and powering bounds; Section 3.5, pp. 69–71: faster arithmetic](a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup.md)

For ordinary [integer](integer-split.md) powers with $|a|\geq2$, the output itself has $\lfloor n\log_2|a|\rfloor+1$ [binary digits](binary-digit.md). Even writing it takes work proportional to that length. Consequently $O(\log(n+1))$ [multiplications](multiplication.md) does not imply $O(\log(n+1))$ operations on [bits](bit.md): the operands grow during ordinary [exponentiation by squaring](exponentiation-by-squaring.md), whereas [modular exponentiation](modular-exponentiation.md) keeps them bounded by the modulus. A squaring or multiplication by a small fixed base can also cost less than a general product, so equal counts need not mean equal running times.

## ↑ Ancestors (6)

1. [Modular exponentiation](modular-exponentiation.md)
2. [Exponentiation by squaring](exponentiation-by-squaring.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
