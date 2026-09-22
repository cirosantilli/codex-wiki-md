# Digit block frequency

↑ **Parent:** [Normal number](normal-number.md)

For a finite prefix of $N\geq r$ digits in [positional notation](positional-notation.md), the digit block frequency $F_N(w)$ of a length-$r$ [word](string.md) $w$ is its number of overlapping occurrences divided by $N-r+1$, the number of available starting positions. All such [digit block frequencies](digit-block-frequency.md) sum to one. The infinite [limit](limit-of-a-function.md) used for a [normal number](normal-number.md) can instead divide counts by $N$: the factor $(N-r+1)/N$ tends to one for fixed $r$.

For the six [binary digits](binary-digit.md) $010101$, the single-digit counts are three zeros and three ones. Its five adjacent pairs are $01,10,01,10,01$, giving

$$
F_6(00)=F_6(11)=0,\qquad F_6(01)=\frac35,\qquad F_6(10)=\frac25.
$$

This example explains both the overlapping convention and the end correction in a finite sample. The corresponding infinite [binary expansion](binary-expansion.md) has pair frequencies $0,1/2,1/2,0$, rather than the four values $1/4$ required of a [normal number](normal-number.md) in base two.

## ↑ Ancestors (5)

1. [Normal number](normal-number.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Absolutely normal number](absolutely-normal-number.md)
- [Champernowne constant](champernowne-constant.md)
- [Digit block frequency](digit-block-frequency.md)
- [Normal number](normal-number.md)
- [Simply normal number](simply-normal-number.md)
