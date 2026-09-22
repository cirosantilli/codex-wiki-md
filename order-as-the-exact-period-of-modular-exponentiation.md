# Order as the exact period of modular exponentiation

↑ **Parent:** [Periodic modular exponentiation](periodic-modular-exponentiation.md)

Let $a,n$ be [coprime integers](coprime-integers.md) with $n>1$, and let $d=\operatorname{ord}_n(a)$ be their [multiplicative order](multiplicative-order.md). For [integers](integer.md) $x,y$,

$$
a^x\equiv a^y\pmod n\quad\Longleftrightarrow\quad d\mid(x-y).
$$

Negative exponents mean powers of the [modular inverse](modular-multiplicative-inverse.md) of $a$. Thus [periodic modular exponentiation](periodic-modular-exponentiation.md) has smallest positive [period](period-of-a-function.md) $d$, and $1,a,\ldots,a^{d-1}$ are distinct [congruence classes](congruence-class.md).[pp. 156–157, Theorem 6.29; multiplicative notation on p. 153](a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup.md)

This lets a huge [modular exponentiation](modular-exponentiation.md) reuse a short list: reduce its exponent modulo the [multiplicative order](multiplicative-order.md), then look up the corresponding power. For example, $1000\equiv1\pmod3$ gives $2^{1000}\equiv2\pmod7$, while $1001\equiv2\pmod3$ gives $2^{1001}\equiv4\pmod7$. When the [multiplicative order](multiplicative-order.md) is unknown, [Euler's theorem](euler-s-theorem.md) permits reduction modulo [Euler's totient function](euler-totient-function.md), though that [period](period-of-a-function.md) may be longer. [Repeated squaring](exponentiation-by-squaring.md) remains useful when computing either the unreduced or the reduced power.

For a proof outline, multiply $a^x\equiv a^y$ by the [modular inverse](modular-multiplicative-inverse.md) of $a^y$, leaving $a^{x-y}\equiv1$. Apply [Euclidean division](euclidean-division.md) to write $x-y=td+r$ with $0\leq r<d$. Then $a^{x-y}\equiv a^r$; minimality of the [multiplicative order](multiplicative-order.md) forces $r=0$. The reverse implication follows from $a^d\equiv1$. The [coprime integers](coprime-integers.md) hypothesis enables cancellation: modulo eight, $2^3\equiv2^4\equiv0$, but this repetition supplies no [multiplicative order](multiplicative-order.md) for two.

## ↑ Ancestors (6)

1. [Periodic modular exponentiation](periodic-modular-exponentiation.md)
2. [Multiplicative order](multiplicative-order.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/10d/b/solution.md)
