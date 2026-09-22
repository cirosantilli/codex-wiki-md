<h1 id="euclid-s-lemma">Euclid's lemma</h1>

↑ **Parent:** [Number theory](number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclid's_lemma)

If a [prime number](prime-number-split.md) $p$ divides a [product](product-of-numbers.md) $ab$ of [integers](integer-split.md) $a,b$, then $p$ divides $a$ or $b$ (possibly both):

$$
p\mid ab\quad\Longrightarrow\quad p\mid a\text{ or }p\mid b.
$$

For example, $5\mid6\cdot10$ and $5\mid10$. The hypothesis that $p$ is a [prime number](prime-number-split.md) matters: $6\mid2\cdot3$, although six divides neither factor. When $p$ does not divide $a$, the [greatest common divisor](greatest-common-divisor.md) of $p$ and $a$ is one; multiply [Bézout's identity](bezout-s-identity.md) $up+va=1$ by $b$ to see that $p\mid b$. Repeated application makes this the uniqueness step in the [fundamental theorem of arithmetic](fundamental-theorem-of-arithmetic.md). [Euclid, Elements, Book VII, Proposition 30](https://mathcs.clarku.edu/~djoyce/elements/bookVII/propVII30.html).

For a completely computed example, $7\mid20\cdot21$ because $20\cdot21=420=7\cdot60$, while $20=7\cdot2+6$ shows that seven does not divide twenty. [Bézout's identity](bezout-s-identity.md) $3\cdot7-20=1$ becomes, after [multiplication](multiplication.md) by $21$,

$$
21=3\cdot7\cdot21-20\cdot21=7\cdot63-7\cdot60=7\cdot3.
$$

The two terms on the right are divisible by seven, which explicitly recovers the forced [divisibility](divisibility-split.md) of the second factor. Both alternatives can hold: $7\mid14\cdot21$, and seven divides both $14$ and $21$.

In fact the property characterizes [prime numbers](prime-number-split.md) among the [integers](integer-split.md) greater than one. If $c$ is a [composite number](composite-number.md), choose $c=ab$ with $1<a,b<c$; then $c\mid ab$, but $c$ divides neither $a$ nor $b$. For several factors, repeated application of [Euclid's lemma](euclid-s-lemma.md) says that a [prime number](prime-number-split.md) dividing their [product](product-of-numbers.md) divides at least one factor. In a [product](product-of-numbers.md) of [prime numbers](prime-number-split.md), that factor must equal it, because a [prime number](prime-number-split.md) has no other [prime factor](prime-factor.md). This is what prevents a different collection of [prime factors](prime-factor.md) from representing the same [positive integer](positive-integer.md) in the [fundamental theorem of arithmetic](fundamental-theorem-of-arithmetic.md).

Book VII, Proposition 30 of [Euclid's Elements](euclid-s-elements.md) states the result in terms of a [prime number](prime-number-split.md) measuring a [product](product-of-numbers.md); its proof uses [coprimality](coprime-integers.md) and [ratios](ratio.md). The calculation using [Bézout's identity](bezout-s-identity.md) above is a modern way to explain the same [divisibility](divisibility-split.md) statement. [Euclid, Elements VII.30, translated text hosted by David Joyce](https://mathcs.clarku.edu/~djoyce/java/elements/bookVII/propVII30.html)

## ↑ Ancestors (4)

1. [Number theory](number-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Euclid's lemma](euclid-s-lemma.md)
- [Fundamental theorem of arithmetic](fundamental-theorem-of-arithmetic.md)
- [Wilson's theorem](wilson-s-theorem.md)
