<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply part a to $A=\{1,\ldots,\lfloor x\rfloor\}$ and all primes. Since

$$
|\{n\leq x:d\mid n\}|=\left\lfloor\frac xd\right\rfloor,
$$

we obtain

$$
S(A,\mathbb P,z)
=x\sum_{d\mid P(z)}\frac{\mu(d)}d+O\left(\sum_{d\mid P(z)}1\right)
=x\prod_{p\leq z}\left(1-\frac1p\right)+O(2^{\pi(z)}).
$$

For $z\leq\log x$, the error is at most $2^z\leq x^{\log2}=o(x/\log z)$. By [Mertens theorem](../../../../../../mertens-theorems.md), as $z\to\infty$,

$$
\prod_{p\leq z}\left(1-\frac1p\right)
=\frac{e^{-\gamma}+o(1)}{\log z}.
$$

Thus

$$
|\{n\in[1,x]:n\text{ has no prime factor at most }z\}|
=\left(e^{-\gamma}+o(1)\right)\frac{x}{\log z},
$$

so one may take $C=e^{-\gamma}>0$. For bounded $z$, the preceding exact product formula gives the corresponding fixed density.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
