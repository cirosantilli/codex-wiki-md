<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Chebyshev estimate from central binomial coefficients](../../../../../../chebyshev-estimate-from-central-binomial-coefficients.md). Define

$$
\vartheta(x)=\sum_{p\leq x}\log p,\qquad
\psi(x)=\sum_{p^k\leq x}\log p.
$$

The first is the [Chebyshev theta function](../../../../../../chebyshev-theta-function.md); the second counts prime powers with the same logarithmic prime weight. For a positive integer $m$, every prime $m<p\leq2m$ divides $\binom{2m}{m}$, hence

$$
\vartheta(2m)-\vartheta(m)\leq\log\binom{2m}{m}\leq2m\log2.
$$

Summing over dyadic intervals yields $\vartheta(2^j)\leq2^{j+1}\log2$. By monotonicity and rounding $x$ upward to a power of two,

$$
\vartheta(x)\leq Cx,\qquad C=4\log2.
$$

For the lower bound, the central [binomial coefficient](../../../../../../binomial-coefficient.md) is the largest of the $2m+1$ coefficients whose sum is $4^m$, so

$$
\log\binom{2m}{m}\geq2m\log2-\log(2m+1).
$$

The exponent of a prime in the central coefficient is

$$
\sum_{k\geq1}\left(\left\lfloor\frac{2m}{p^k}\right\rfloor
-2\left\lfloor\frac m{p^k}\right\rfloor\right).
$$

Each summand is zero or one. Therefore $\log\binom{2m}{m}\leq\psi(2m)$. Higher prime powers contribute only

$$
0\leq\psi(x)-\vartheta(x)
=\sum_{k=2}^{\lfloor\log_2x\rfloor}\vartheta(x^{1/k})
\leq C\sqrt x\,\log_2x=o(x).
$$

Combining the lower bound with $2m$ just below $x$ shows $\vartheta(x)\geq cx$ for sufficiently large $x$, with, for example, $c=(\log2)/2$.

Let $\pi(x)$ denote the number of primes at most $x$. Since every prime weight is at most $\log x$,

$$
\pi(x)\geq\frac{\vartheta(x)}{\log x}\geq c\frac{x}{\log x}.
$$

For the upper bound, separate the primes at $\sqrt x$. The small ones number at most $\sqrt x$, and every larger one has weight at least $(\log x)/2$, giving

$$
\pi(x)\leq\sqrt x+\frac{2\vartheta(x)}{\log x}
\leq\sqrt x+2C\frac{x}{\log x}.
$$

Since $\sqrt x=o(x/\log x)$, this proves

$$
\boxed{A\frac n{\log n}\leq N(n)\leq B\frac n{\log n}}
$$

for all sufficiently large $n$, for instance with $A=(\log2)/2$ and $B=8\log2+1$. This elementary [Chebyshev estimate](../../../../../../chebyshev-estimate.md) does not assume the [Prime number theorem](../../../../../../prime-number-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
