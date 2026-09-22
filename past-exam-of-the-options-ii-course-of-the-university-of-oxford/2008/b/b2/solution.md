<h1 id="b/b2/solution">Solution</h1>

↑ **Parent:** [B2](../b2.md)

The [characteristic of a field](../../../../characteristic-of-a-field.md) is the least positive [integer](../../../../integer-split.md) $p$ with $p1_F=0$, or zero if none exists. Finiteness forces a positive characteristic, since the sequence of [integer](../../../../integer-split.md) multiples of one must repeat. If this least [integer](../../../../integer-split.md) factored into two smaller positive factors, their nonzero field multiples would multiply to zero, contradicting the absence of zero divisors. Hence it is prime. The field is a [finite-dimensional vector space](../../../../finite-dimensional-vector-space.md) over its prime [subfield](../../../../subfield.md) $\mathbb F_p$, so choosing a [basis](../../../../basis.md) gives $|F|=p^a$.

A nonzero [polynomial](../../../../polynomial-split.md) of degree $n$ over a field has at most $n$ roots: each root supplies a linear factor by [polynomial](../../../../polynomial-split.md) division, and induction applies to the quotient. In particular $X^n-1$ has at most $n$ roots. The elements of $F^\times$ whose orders divide $n$ are precisely those roots. The permitted finite-[group](../../../../group-split.md) criterion therefore proves **$F^\times$ is cyclic**.

For the final assertion take an odd [Fermat prime](../../../../fermat-prime.md) $p=2^m+1$, $m\geq1$. Primality forces $m$ to be a power of two: an odd factor $s>1$ in $m=2^rs$ would factor $(2^{2^r})^s+1$ nontrivially. Since $2^m\equiv-1\pmod p$, the order of two divides $2m$ but not $m$. As $2m$ is a power of two, its only divisor not dividing $m$ is $2m$ itself. Thus

$$
\boxed{\operatorname{ord}_p(2)=2m}.
$$

It generates the full [group](../../../../group-split.md) exactly when $2m=2^m$, which holds for $m=1,2$ and fails for $m\geq3$. Therefore the possibilities are **$p=3,5$**, equivalently $p\leq5$ among odd Fermat primes. The oddness is implicit in referring to two as a unit; $p=2$ is not an admissible case for that claim.

## ↑ Ancestors (12)

1. [B2](../b2.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
