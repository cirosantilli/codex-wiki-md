<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

The [Legendre prime-counting formula](../../../../../legendre-prime-counting-formula.md) counts positive [integers](../../../../../integer.md) surviving a finite prime sieve. For $x\geq2$, put $a=\pi(\sqrt{x})$ and let $p_1,\ldots,p_a$ be the [primes](../../../../../prime-number.md) at most $\sqrt{x}$. By [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md), the number of positive [integers](../../../../../integer.md) at most $x$ divisible by none of these [primes](../../../../../prime-number.md) is

$$
\phi(x,a)=\sum_{S\subseteq\{1,\ldots,a\}}(-1)^{|S|}\left\lfloor\frac{x}{\prod_{i\in S}p_i}\right\rfloor.
$$

The empty product is $1$. Every [composite number](../../../../../composite-number.md) at most $x$ has a [prime factor](../../../../../prime-factor.md) at most $\sqrt{x}$, so the survivors are precisely $1$ and the [primes](../../../../../prime-number.md) between $\sqrt{x}$ and $x$. Consequently

$$
\boxed{\pi(x)=a-1+\phi(x,a).}
$$

For $x=42$, the sieving [primes](../../../../../prime-number.md) are $2,3,5$, and

$$
\phi(42,3)=42-21-14-8+7+4+2-1=11,\qquad\boxed{\pi(42)=13.}
$$

As a direct check, the [primes](../../../../../prime-number.md) are $2,3,5,7,11,13,17,19,23,29,31,37,41$.

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
