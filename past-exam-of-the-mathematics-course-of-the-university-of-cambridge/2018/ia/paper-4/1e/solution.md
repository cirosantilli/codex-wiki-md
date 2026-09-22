<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

[Fermat's little theorem](../../../../../fermat-little-theorem.md) states that if $p$ is prime, then $a^p\equiv a\pmod p$ for every integer $a$; equivalently, $a^{p-1}\equiv1\pmod p$ when $p\nmid a$.

If $p\equiv3\pmod4$ and $x^2\equiv-1\pmod p$, then

$$
x^{p-1}=(x^2)^{(p-1)/2}\equiv(-1)^{(p-1)/2}=-1\pmod p,
$$

because $(p-1)/2$ is odd. This contradicts Fermat's theorem, so **$x^2\equiv-1\pmod p$ has no solution**.

If the primes congruent to $1\pmod4$ were $p_1,\ldots,p_k$, set $N=(2p_1\cdots p_k)^2+1$. Any prime divisor $q$ of $N$ is odd and has $-1$ as a [quadratic residue](../../../../../quadratic-residue.md). The preceding result forces $q\equiv1\pmod4$, but $q$ divides none of the $p_i$ because $N\equiv1\pmod{p_i}$. This contradiction proves that **infinitely many primes are congruent to $1\pmod4$**.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
