<h1 id="15c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $r$ is even,

$$
(a^{r/2}-1)(a^{r/2}+1)=a^r-1\equiv0\pmod N.
$$

The first factor is not divisible by $N$, since that would contradict minimality of $r$, and the second is not divisible by $N$ by hypothesis. Nevertheless their product is divisible by $N$. Therefore

$$
1<\gcd(a^{r/2}-1,N)<N,
$$

and Euclid's algorithm computes a nontrivial factor. One can also compute $\gcd(a^{r/2}+1,N)$; together the two gcds expose factors lying on opposite sides of the congruence $a^{r/2}\equiv\pm1$ modulo the prime-power divisors of $N$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15C](../../15c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
