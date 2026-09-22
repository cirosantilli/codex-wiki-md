<h1 id="17b/solution">Solution</h1>

↑ **Parent:** [17B](../17b.md)

The [Legendre symbol](../../../../../legendre-symbol.md) $(a/p)$ is $+1$ when $a$ is a nonzero square modulo the odd prime $p$, $-1$ when it is not a square, and $0$ when $p\mid a$. For the coprime case, [Euler's criterion](../../../../../euler-s-criterion.md) states

$$
\boxed{a^{(p-1)/2}\equiv\left(\frac ap\right)\pmod p.}
$$

Write $h=(p-1)/2$. For $1\le j\le h$, the balanced residues $r_j$ are nonzero and their absolute values lie in $\{1,\ldots,h\}$. If $|r_j|=|r_k|$, then $aj\equiv\pm ak\pmod p$. Cancel $a$. The plus sign forces $j=k$; the minus sign would require $j+k=p$, impossible because $j+k\le p-1$. Thus the absolute residues form a permutation of $1,\ldots,h$. If exactly $l$ are negative, multiplying gives

$$
a^h h!\equiv\prod_{j=1}^h r_j=(-1)^l h!\pmod p.
$$

Since $p$ does not divide $h!$, cancellation and [Euler's criterion](../../../../../euler-s-criterion.md) prove [Gauss's lemma](../../../../../gauss-s-lemma-number-theory.md):

$$
\boxed{\left(\frac ap\right)=(-1)^l.}
$$

The two signs are distinct modulo the odd prime, so this congruence identifies the integer symbol itself.

For $a=2$, the balanced representative of $2j$ is negative precisely when $j>p/4$, giving $l=(p-1)/2-\lfloor p/4\rfloor$. Checking the four odd residue classes modulo eight gives even $l$ for $p\equiv1,7$ and odd $l$ for $p\equiv3,5$. Hence

$$
\boxed{2\text{ is a quadratic residue modulo }p\iff p\equiv1\text{ or }7\pmod8.}
$$

This is the [quadratic character of two](../../../../../second-supplementary-law-for-quadratic-reciprocity.md) obtained from the lemma.

Let $P=p_1\cdots p_m$ and $N=8P^2-1$. If a prime $q$ divides $N$, then $q$ is odd and cannot divide $P$. Moreover

$$
(4P)^2=16P^2=2(N+1)\equiv2\pmod q,
$$

so $2$ has an explicit nonzero square root modulo $q$. The criterion just proved forces every prime divisor of $N$ into the classes $1$ or $7$ modulo eight. But $N\equiv7\pmod8$: if all its prime factors were $1$ modulo eight, their product, with multiplicities, would also be $1$. Thus at least one prime divisor is $7$ modulo eight. No listed $p_i$ divides $N$, because $N\equiv-1\pmod{p_i}$. This always produces another such prime, proving **infinitely many primes are congruent to seven modulo eight**, the [Euclid proof for infinitely many primes congruent to seven modulo eight](../../../../../euclid-proof-for-infinitely-many-primes-congruent-to-seven-modulo-eight.md).

## ↑ Ancestors (10)

1. [17B](../17b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
