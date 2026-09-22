<h1 id="8e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

If the [prime](../../../../../../prime-number.md) $p$ does not divide $x$, then $\gcd(p,x)=1$. The [Bezout identity](../../../../../../bezout-identity.md) gives [integers](../../../../../../integer.md) $a,b$ with $ap+bx=1$. Multiplying by $y$ gives $apy+bxy=y$. If $p\mid xy$, both terms on the left are divisible by $p$, so $p\mid y$. Thus [Euclid lemma](../../../../../../euclid-lemma.md) holds:

$$
\boxed{p\mid xy\implies p\mid x\text{ or }p\mid y.}
$$

For completeness, existence in the [Fundamental theorem of arithmetic](../../../../../../fundamental-theorem-of-arithmetic.md) follows by strong induction on a positive [integer](../../../../../../integer.md) $n>1$. If $n$ is [prime](../../../../../../prime-number.md) there is nothing to prove; otherwise $n=ab$ with $1<a,b<n$, and the inductive [prime](../../../../../../prime-number.md) factorizations of $a,b$ give one for $n$. The [integer](../../../../../../integer.md) $1$ has the empty factorization.

For uniqueness, suppose $p_1\cdots p_r=q_1\cdots q_s$ are two [prime](../../../../../../prime-number.md) factorizations. Repeated application of [Euclid lemma](../../../../../../euclid-lemma.md) shows that $p_1$ divides some $q_j$. Both are [primes](../../../../../../prime-number.md), so they are equal. Reorder the second list, cancel this equal factor, and repeat. All factors must be matched, including their multiplicities. Thus **[prime factorization](../../../../../../fundamental-theorem-of-arithmetic.md) exists and is unique up to the order of its factors**. For nonzero negative [integers](../../../../../../integer.md) one also records the sign.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [8E](../../8e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
