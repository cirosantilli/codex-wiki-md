<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
L=\log\log x,
\qquad
S=\sum_{p\leq x}\frac1p=L+O(1)
$$

by part a. Double-counting divisibility gives the first moment of the [prime omega function](../../../../../../prime-omega-function.md):

$$
\sum_{n\leq x}\omega(n)
=\sum_{p\leq x}\left\lfloor\frac xp\right\rfloor
=xS+O(\pi(x)).
$$

Moreover,

$$
\omega(n)^2=\omega(n)+2\sum_{\substack{p<q\\pq\mid n}}1,
$$

so

$$
\sum_{n\leq x}\omega(n)^2
\leq xS+2x\sum_{p<q\leq x}\frac1{pq}
\leq xS+xS^2.
$$

Expanding the square and using the given bound $\pi(x)\ll x/\log x$ now gives the [Turán normal-order theorem for distinct prime divisors](../../../../../../turan-normal-order-theorem-for-distinct-prime-divisors.md) estimate

$$
\sum_{n\leq x}(\omega(n)-L)^2
\ll x(S-L)^2+xS+L\pi(x)
\ll xL.
$$

By the [Chebyshev inequality](../../../../../../chebyshev-inequality.md), the number of $n\leq x$ for which

$$
|\omega(n)-L|>\tfrac12L^{3/4}
$$

is $O(x/L^{1/2})=o(x)$. Discard the $O(\sqrt x)$ integers below $\sqrt x$. For $\sqrt x<n\leq x$,

$$
|\log\log n-L|\leq\log2
$$

and $(\log\log n)^{3/4}\sim L^{3/4}$. Hence, for all sufficiently large $x$, every remaining integer counted in the question also satisfies the preceding inequality. Therefore

$$
\boxed{\#\{n\leq x:|\omega(n)-\log\log n|>(\log\log n)^{3/4}\}=o(x)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
