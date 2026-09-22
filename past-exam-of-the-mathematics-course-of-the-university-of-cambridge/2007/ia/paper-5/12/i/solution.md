<h1 id="12/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose $p$ is a [prime number](../../../../../../prime-number.md), $p\mid xy$ and $p\nmid x$. Since the only positive divisors of $p$ are one and $p$, the [greatest common divisor](../../../../../../greatest-common-divisor.md) of $p$ and $x$ is one. By [Bézout's identity](../../../../../../bezout-identity.md), integers $u,v$ exist with $up+vx=1$. Multiplying by $y$ gives $upy+vxy=y$. Both terms on the left are divisible by $p$, so $p\mid y$. Thus [Euclid lemma](../../../../../../euclid-lemma.md) gives

$$
\boxed{p\mid xy\ \Longrightarrow\ p\mid x\ \text{or}\ p\mid y.}
$$

The [Fundamental theorem of arithmetic](../../../../../../fundamental-theorem-of-arithmetic.md) says that every positive integer greater than one is a product of [prime numbers](../../../../../../prime-number.md), uniquely up to their order. Existence follows by strong [mathematical induction](../../../../../../mathematical-induction.md): if $n$ is prime it already has a factorization; otherwise $n=ab$ with $1<a,b<n$, and the factorizations of $a,b$ combine to factor $n$.

For uniqueness, suppose $p_1\cdots p_r=q_1\cdots q_s$ are two prime factorizations. Repeated application of [Euclid lemma](../../../../../../euclid-lemma.md) makes $p_1$ divide one of the $q_j$, so primality forces $p_1=q_j$. Reorder that factor to the front, cancel it and repeat. Neither side can retain extra primes when the other has become one, since every prime exceeds one. The two multisets are therefore identical. For a negative integer there is additionally the uniquely determined sign; one has the empty positive factorization, and zero is excluded. **The prime-product divisibility lemma is the step which makes factorization unique.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12](../../12.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
