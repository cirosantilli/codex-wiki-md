<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

Write $n=2^r m$ with $m$ odd. If $m>1$, the [polynomial factor](../../../../../polynomial-factor.md) of $X^m+1$ by $X+1$, evaluated at $X=10^{2^r}$, supplies a proper divisor. Therefore **$n$ must be a power of two**. Conversely this is only a necessary condition for [primality testing](../../../../../primality-testing.md).

For a [prime factor](../../../../../prime-factor.md) $p$ of the number, $p$ is odd and does not divide $10$. Its [multiplicative order](../../../../../multiplicative-order.md) $d$ satisfies $d\mid 2n$ but $d\nmid n$, since $10^n\equiv-1\pmod p$. When $n$ is a power of two, every proper divisor of $2n$ divides $n$, so $d=2n$. By [Lagrange theorem](../../../../../lagrange-s-theorem.md) in the [multiplicative group of a finite field](../../../../../multiplicative-group-of-a-finite-field.md), $2n\mid p-1$. Thus $\boxed{p\equiv1\pmod{2n}}$.

The [Fermat factorization method](../../../../../fermat-s-factorization-method.md) searches for a [difference of two squares](../../../../../difference-of-two-squares.md): starting at $a=\lceil\sqrt N\rceil$, increase $a$ until $a^2-N=b^2$, and return $(a-b)(a+b)$. Every factorization of an odd integer has this form, with $a=(d+e)/2$ and $b=(e-d)/2$. For $N=10001$, the successive differences at $a=101,102,103,104,105$ are $200,403,608,815,1024$. The last is $32^2$, giving $\boxed{10001=73\cdot137}$. Trial division by the [primes](../../../../../prime-number.md) up to their respective square roots confirms that both factors are [prime](../../../../../prime-number.md).

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
