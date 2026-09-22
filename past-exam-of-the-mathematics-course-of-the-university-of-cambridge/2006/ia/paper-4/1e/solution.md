<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

A [prime number](../../../../../prime-number.md) is an integer $p>1$ whose only positive divisors are $1$ and $p$. Every integer greater than one has a [prime factorization](../../../../../fundamental-theorem-of-arithmetic.md); in particular it has a [prime](../../../../../prime-number.md) divisor.

To prove [infinitely many primes congruent to minus one modulo six](../../../../../infinitely-many-primes-congruent-to-minus-one-modulo-six.md), suppose a finite list $p_1,\ldots,p_n$ contains all such [primes](../../../../../prime-number.md), and put $P=p_1\cdots p_n$; the empty product is one. The integer $N=6P-1>1$ is [coprime](../../../../../coprime-integers.md) to $6$, so each [prime factor](../../../../../prime-factor.md) is congruent to $1$ or $-1$ modulo $6$. If all its [prime factors](../../../../../prime-factor.md), counted with multiplicity, were congruent to $1$, their product would also be congruent to $1$. But $N\equiv-1\pmod6$. Hence some [prime](../../../../../prime-number.md) divisor $q$ satisfies $q\equiv-1\pmod6$. None of the listed [primes](../../../../../prime-number.md) divides $N$, since $N\equiv-1\pmod{p_i}$. This contradicts completeness of the list.

For [infinitely many primes congruent to one modulo six](../../../../../infinitely-many-primes-congruent-to-one-modulo-six.md), suppose instead that $p_1,\ldots,p_n$ lists every [prime](../../../../../prime-number.md) congruent to $1$ modulo $6$, and use

$$
N=(2P)^2+3.
$$

It is odd. Since each listed [prime](../../../../../prime-number.md) is [coprime](../../../../../coprime-integers.md) to $3$, $P^2\equiv1\pmod3$, so $N\equiv1\pmod3$ and $3$ does not divide it. Any [prime](../../../../../prime-number.md) divisor $q$ is therefore greater than $3$ and satisfies the [modular congruence](../../../../../modular-congruence.md)

$$
(2P)^2\equiv-3\pmod q.
$$

The allowed quadratic-congruence result gives $q\equiv1\pmod6$. Yet $N\equiv3\pmod{p_i}$, and $p_i>3$, so no listed [prime](../../../../../prime-number.md) divides $N$. Again there is a new [prime](../../../../../prime-number.md) in the required residue class. Thus **both residue classes $6k-1$ and $6k+1$ contain infinitely many [primes](../../../../../prime-number.md)**.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
