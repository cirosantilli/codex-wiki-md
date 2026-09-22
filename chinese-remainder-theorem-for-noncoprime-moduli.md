# Chinese remainder theorem for noncoprime moduli

↑ **Parent:** [Chinese remainder theorem](chinese-remainder-theorem.md)

For positive [integer moduli](modulus-in-modular-arithmetic.md) $m,n$, the simultaneous [integer congruences](integer-congruence.md) $x\equiv a\pmod m$ and $x\equiv b\pmod n$ are solvable exactly when $a\equiv b\pmod{\gcd(m,n)}$. When solvable, they determine a unique [congruence class](congruence-class.md) modulo $\operatorname{lcm}(m,n)$. To see the condition, put $x=a+mk$: the remaining equation is the [linear congruence](linear-congruence.md) $mk\equiv b-a\pmod n$, which is solvable exactly when the [greatest common divisor](greatest-common-divisor.md) divides $b-a$.

For example, $x\equiv1\pmod6$ and $x\equiv3\pmod8$ give $6k\equiv2\pmod8$, hence $3k\equiv1\pmod4$ and $k\equiv3\pmod4$. Thus **$x\equiv19\pmod{24}$**. Changing the second remainder to two makes the conditions incompatible: the first requires an [odd integer](odd-integer.md), while the second requires an [even integer](even-number.md). Article 32 of [Carl Friedrich Gauss](carl-friedrich-gauss.md)'s _Disquisitiones arithmeticae_ gives a successive construction for simultaneous remainders, including the [greatest common divisor](greatest-common-divisor.md) and [least common multiple](least-common-multiple.md) that enter this general case. [Gauss, Disquisitiones arithmeticae, section II, article 32; text from the 1870 collected edition](https://la.wikisource.org/wiki/Disquisitiones_arithmeticae/Sectio_secunda)

## ↑ Ancestors (3)

1. [Chinese remainder theorem](chinese-remainder-theorem.md)
2. [Mathematics](mathematics-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Chinese remainder theorem](chinese-remainder-theorem.md)
- [Least common multiple](least-common-multiple.md)
