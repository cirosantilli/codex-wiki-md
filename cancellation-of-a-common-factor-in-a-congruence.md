# Cancellation of a common factor in a congruence

↑ **Parent:** [Linear congruence](linear-congruence.md)

For [integers](integer-split.md) $a,b$ and positive [integers](integer-split.md) $c,n$, a common factor may be cancelled from a [integer congruence](integer-congruence.md) provided the modulus is divided by the corresponding [greatest common divisor](greatest-common-divisor.md). Let $d=\gcd(c,n)$, $c=dc'$, and $n=dn'$. The [integers](integer-split.md) $c',n'$ are coprime: any common divisor greater than one would give a common divisor of $c,n$ larger than $d$.

By [divisibility](divisibility-split.md) and [Euclid's lemma](euclid-s-lemma.md),

$$
ac\equiv bc\pmod n
\iff n'\mid c'(a-b)
\iff n'\mid a-b.
$$

This proves the displayed equivalence. If $c$ is coprime to $n$, the modulus stays unchanged and this is ordinary cancellation by a [modular multiplicative inverse](modular-multiplicative-inverse.md). If $n\mid c$, the reduced modulus is $1$, so every pair $a,b$ satisfies the reduced [integer congruence](integer-congruence.md).

## ↑ Ancestors (7)

1. [Linear congruence](linear-congruence.md)
2. [Modular congruence](modular-congruence.md)
3. [Modular arithmetic](modular-arithmetic-split.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/1/c/ii/solution.md)
