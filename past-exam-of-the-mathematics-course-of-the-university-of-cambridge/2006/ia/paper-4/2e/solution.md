<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

For integers $0\leq r\leq n$, the [binomial coefficient](../../../../../binomial-coefficient.md) is

$$
\binom nr=\frac{n!}{r!(n-r)!},
$$

the number of $r$-element [subsets](../../../../../subset.md) of an $n$-element set. It is zero outside that range. To obtain [Pascal's identity](../../../../../pascal-s-rule.md), distinguish one element of an $(n+1)$-element set. An $r$-element [subset](../../../../../subset.md) either omits it, giving $\binom nr$ choices, or contains it, leaving $\binom n{r-1}$ choices. These cases are disjoint and exhaustive, so

$$
\boxed{\binom{n+1}r=\binom nr+\binom n{r-1}\qquad(0<r\leq n).}
$$

If $p$ is a [prime number](../../../../../prime-number.md) and $0<r<p$, then

$$
r!\binom pr=p(p-1)\cdots(p-r+1).
$$

The right side is divisible by $p$, while $r!$ is [coprime](../../../../../coprime-integers.md) to $p$. Cancellation modulo $p$ proves the [prime-row binomial coefficient divisibility](../../../../../prime-row-binomial-coefficient-divisibility.md)

$$
\boxed{p\mid\binom pr\qquad(0<r<p).}
$$

Apply the [binomial theorem](../../../../../binomial-theorem.md) in the polynomial ring modulo $p$. The intermediate coefficients just proved to vanish give

$$
(1+X)^p\equiv1+X^p\pmod p.
$$

Multiplying by $(1+X)^k$ yields

$$
(1+X)^{p+k}\equiv(1+X^p)(1+X)^k\pmod p.
$$

For $0\leq r\leq k<p$, the $X^p$ factor cannot contribute to the coefficient of $X^r$. Comparing coefficients proves the [binomial coefficient congruence across a prime row](../../../../../binomial-coefficient-congruence-across-a-prime-row.md)

$$
\boxed{\binom{p+k}r\equiv\binom kr\pmod p.}
$$

This also covers $r=0$, when both sides are one.

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
