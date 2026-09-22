<h1 id="11g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

It suffices first to prove the [elementary primorial bound](../../../../../../elementary-primorial-bound.md) for positive integers $n$, by strong induction. The case $n=1$ is immediate.

If $n=2k$, every prime $p$ with $k<p\leq2k$ divides $\binom{2k}{k}$: the numerator $(2k)!$ contains $p$, whereas the two copies of $k!$ do not. Since these primes are distinct,

$$
P(2k)\leq P(k)\binom{2k}{k}.
$$

The induction hypothesis and the binomial theorem give

$$
P(2k)\leq4^k\binom{2k}{k}
\leq4^k2^{2k}=4^{2k}.
$$

If $n=2k+1$, part (b) shows that every prime $k+2\leq p\leq2k+1$ divides $\binom{2k+1}{k+1}$. Hence

$$
P(2k+1)\leq P(k+1)\binom{2k+1}{k+1}.
$$

The two central coefficients of $(1+1)^{2k+1}$ are equal, so

$$
2\binom{2k+1}{k+1}\leq2^{2k+1},
$$

and therefore

$$
P(2k+1)\leq4^{k+1}4^k=4^{2k+1}.
$$

This completes the induction. For real $X\geq1$,

$$
\boxed{P(X)=P(\lfloor X\rfloor)\leq4^{\lfloor X\rfloor}\leq4^X.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11G](../../11g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
