<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Take $\mathcal P$ to contain the primes at least $5$; the exceptional local behavior at $2$ and $3$ is then harmless. Fix a sufficiently large constant $w$ and later choose

$$
z=X^\delta,
\qquad D=X^\eta,
$$

with fixed small $0<\delta<\eta$. The [Buchstab identity](../../../../../../buchstab-identity.md) gives

$$
S(\mathcal A,\mathcal P,z)
=S(\mathcal A,\mathcal P,w)
-\sum_{\substack{w\leq p<z\\p\in\mathcal P}}
S(\mathcal A_p,\mathcal P,p).
$$

The first term is $c_wX+O_w(1)$ for a positive constant $c_w$, by direct counting in the finitely many permitted residue classes modulo $P_w$.

For each term in the sum, part c supplies the local factor $g(p)=3/p$ and remainders bounded by powers of $3^{\omega(d)}$. Apply the [Selberg upper-bound sieve](../../../../../../selberg-upper-bound-sieve.md) to the remaining prime conditions. [Mertens theorem](../../../../../../mertens-theorems.md) gives the dimension-three density

$$
\prod_{w\leq q<p}\left(1-\frac3q\right)
\asymp_w\frac1{(\log p)^3},
$$

so the main terms in the Buchstab sum are bounded by

$$
O_w(X)\sum_{p\geq w}\frac1{p(\log p)^3}.
$$

This convergent tail can be made smaller than $c_wX/4$ by taking $w$ large. The weighted remainder terms are $o(X)$: the estimate $k^{\omega(n)}\ll_{k,\varepsilon}n^\varepsilon$ controls the summed remainders, while part d controls uniformly the loss caused by the finite sieve level. Choosing $\delta$ sufficiently small relative to $\eta$, and then taking $X$ large, therefore gives

$$
S(\mathcal A,\mathcal P,X^\delta)\geq cX
$$

for some absolute $c>0$.

For every counted $m$, the distinct prime divisors of $F(m)$ are either below the fixed $w$ or at least $X^\delta$. The first class contains at most $\pi(w)$ primes, while $F(m)\ll X^3$ makes the second class contain at most

$$
\frac{\log F(m)}{\log X^\delta}\leq\frac3\delta+O(1)
$$

primes. Since every prime divisor of $m$, $m+2$, or $m+6$ divides $F(m)$,

$$
\omega(m)+\omega(m+2)+\omega(m+6)
\leq 3\omega(F(m))
\leq C
$$

after enlarging an absolute constant $C$. A positive proportion occurs for arbitrarily large $X$, so infinitely many such $m$ exist. This is the [almost-primes from an upper-bound sieve and Buchstab identity](../../../../../../almost-primes-from-an-upper-bound-sieve-and-buchstab-identity.md) method.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
