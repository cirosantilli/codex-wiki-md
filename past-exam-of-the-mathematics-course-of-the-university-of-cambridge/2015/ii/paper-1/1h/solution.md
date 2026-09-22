<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

For an odd prime $p$, the [Legendre symbol](../../../../../legendre-symbol.md) $(a/p)$ is $0$ if $p\mid a$, $1$ if $a$ is a nonzero square modulo $p$, and $-1$ otherwise. [Euler's criterion](../../../../../euler-s-criterion.md) states

$$
\boxed{a^{(p-1)/2}\equiv (a/p)\pmod p}.
$$

If $p\mid a$ both sides vanish. Otherwise write $a\equiv g^j$ for a [primitive root](../../../../../primitive-root-modulo-n.md) $g$. The squares are precisely the even powers of $g$, while $g^{(p-1)/2}$ has order two and therefore equals $-1$. Hence $a^{(p-1)/2}=(-1)^j$, proving the criterion and the useful special case $(-1/p)=(-1)^{(p-1)/2}$.

For odd $n$, $n^2+4\equiv5\pmod8$. Every prime divisor $p$ of this number is odd, and $p\nmid n$, so $(n/2)^2\equiv-1\pmod p$. [Euler's criterion](../../../../../euler-s-criterion.md) forces $p\equiv1\pmod4$, hence $p\equiv1$ or $5\pmod8$. A product of such primes can be $5\pmod8$ only if a prime $5\pmod8$ occurs to an odd power.

Suppose the primes $5\pmod8$ were $p_1,\ldots,p_r$. Choose the odd integer $n=p_1\cdots p_r$ (or $n=1$ for an empty list). None of these primes divides $n^2+4$, since the latter is $4$ modulo each $p_i$. Yet the preceding argument gives a prime divisor $5\pmod8$, outside the list. This contradiction proves **infinitely many primes congruent to $5$ modulo $8$**.

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
