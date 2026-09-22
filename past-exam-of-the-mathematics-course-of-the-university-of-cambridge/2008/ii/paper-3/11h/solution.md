<h1 id="11h/solution">Solution</h1>

↑ **Parent:** [11H](../11h.md)

For positive odd coprime integers $m,n$, the [Jacobi reciprocity law](../../../../../jacobi-reciprocity-law.md) is

$$
\boxed{\left(\frac mn\right)\left(\frac nm\right)=(-1)^{(m-1)(n-1)/4}.}
$$

Factor $a=\prod_jq_j^{e_j}$. Since $a$ is not a square, some $e_j$ is [odd](../../../../../odd-function.md). Choose a [quadratic nonresidue](../../../../../quadratic-nonresidue.md) modulo that $q_j$, and choose residue one modulo each other $q_i$. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) provides a positive $n$ with these residues and with $n\equiv1\pmod4$. Multiplicativity of the [Jacobi symbol](../../../../../jacobi-symbol.md) then gives $(n/a)=-1$.

Suppose only finitely many [primes](../../../../../prime-number.md) $p_1,\ldots,p_s$ satisfy $(a/p_i)=-1$. They are coprime to $a$. Repeat the preceding [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) construction, additionally imposing $n\equiv1\pmod{p_i}$ at every odd $p_i$ and taking $n\equiv1\pmod4$ to avoid two. Since $n\equiv1\pmod4$, [Jacobi reciprocity](../../../../../jacobi-reciprocity-law.md) gives $(a/n)=(n/a)=-1$. Factoring this [Jacobi symbol](../../../../../jacobi-symbol.md) over the prime factors of $n$ shows that at least one such prime $p$ has $(a/p)=-1$. But none of the listed primes divides $n$, a contradiction. This proves the [infinitely many prime quadratic nonresidues of a nonsquare integer](../../../../../infinitely-many-prime-quadratic-nonresidues-of-a-nonsquare-integer.md) assertion.

## ↑ Ancestors (10)

1. [11H](../11h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
