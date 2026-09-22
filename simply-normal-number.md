# Simply normal number

↑ **Parent:** [Normal number](normal-number.md)

A [real number](real-number.md) is simply normal in base $K$ if each individual digit in its [positional notation](positional-notation.md) has limiting [digit block frequency](digit-block-frequency.md) $1/K$. This is the length-one part of the definition of a [normal number](normal-number.md). It places no equal-frequency requirement on longer [words](string.md).

For example, $x=0.010101\ldots_2=1/3$ is a [simply normal number](simply-normal-number.md) in base two: each [binary digit](binary-digit.md) has frequency $1/2$. But $00$ and $11$ never occur, and $01$ and $10$ each have frequency $1/2$. Thus $x$ is not a [normal number](normal-number.md) in base two. Even a [sequence](sequence.md) that looks more complicated, such as the deterministic [Thue–Morse sequence](thue-morse-sequence.md), must be tested against the actual [digit block frequency](digit-block-frequency.md) definition; visual complexity is no substitute for it.

The [decimal representation](decimal-representation.md) $y=0.01234567890123456789\ldots$ makes the same point in base ten. Every digit has frequency $1/10$, yet the only adjacent pairs are

$$
01,12,23,34,45,56,67,78,89,90.
$$

Each has limiting [digit block frequency](digit-block-frequency.md) $1/10$; the other ninety pairs have frequency zero. A [normal number](normal-number.md) in base ten requires $1/100$ for every one of the hundred pairs. This [rational number](rational-number.md) is a [simply normal number](simply-normal-number.md) in base ten, but it is not a [normal number](normal-number.md) in that base.

## ↑ Ancestors (5)

1. [Normal number](normal-number.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Normal number](normal-number.md)
- [Simply normal number](simply-normal-number.md)
