<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $A(x)$ count [primes](../../../../../prime-number.md) $p\le x$ for which $p+2$ is also [prime](../../../../../prime-number.md). We prove $A(x)\ll x/\log^2x$ using a quadratic [Selberg sieve](../../../../../selberg-sieve.md), then apply [Abel summation](../../../../../abel-s-summation-formula.md).

For $F(n)=n(n+2)$, each odd [prime](../../../../../prime-number.md) has exactly two roots modulo that prime. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) gives the [polynomial root density in a sieve](../../../../../polynomial-root-density-in-a-sieve.md)

$$
\#\{n\le x:d\mid F(n)\}=xg(d)+O(\rho_F(d)),\qquad g(d)=\frac{2^{\omega(d)}}d,
$$

for odd [squarefree integers](../../../../../squarefree-integer.md) $d$. Put $R=x^{1/8}$ and choose the optimizing real [Selberg sieve weights](../../../../../selberg-sieve-weights.md) $\lambda_d$, supported on these $d\le R$, with $\lambda_1=1$. If $p,p+2$ are prime and $p>R$, their weight $(\sum_{d\mid F(p)}\lambda_d)^2$ is one. It is nonnegative for every other integer. Expanding the square therefore gives

$$
A(x)\le O(R)+x\sum_{d,e\le R}\lambda_d\lambda_e g([d,e])+O\left(\sum_{d,e\le R}|\lambda_d\lambda_e|\rho_F([d,e])\right).
$$

The [Selberg sieve diagonalization](../../../../../selberg-sieve-diagonalization.md) makes the main quadratic form $1/J(R)$, where

$$
J(R)=\sum_{\substack{d\le R\\d\text{ odd and squarefree}}}\prod_{p\mid d}\frac2{p-2}.
$$

The [optimal Selberg weights have modulus at most one](../../../../../optimal-selberg-weights-have-modulus-at-most-one.md). Since $\rho_F([d,e])\le[d,e]\le R^2$, the remainder is at most $O(R^4)$.

For completeness, the lower bound on $J$ is where the second logarithm enters. Restrict to [primes](../../../../../prime-number.md) $3\le p\le y=R^{1/8}$ and put $k(p)=2/(p-2)$. The full product $W=\prod_{3\le p\le y}(1+k(p))$ is $\asymp\log^2 y$, since its [logarithm](../../../../../logarithm.md) is $2\sum_{3\le p\le y}1/p+O(1)$ and the [Mertens second theorem](../../../../../mertens-second-theorem.md) applies. Give the associated [squarefree divisor](../../../../../squarefree-divisor.md) $d$ probability $k(d)/W$. Prime inclusion probabilities are $2/p$, so the [Mertens first theorem](../../../../../mertens-first-theorem.md) gives

$$
\mathbb E\log d=2\sum_{3\le p\le y}\frac{\log p}p=2\log y+O(1)<\frac12\log R
$$

for large $R$. The [Markov inequality](../../../../../markov-inequality.md) shows that at least half the weight has $d\le R$. This proves the [truncated Euler-product lower bound](../../../../../truncated-euler-product-lower-bound.md) $J(R)\gg W\gg\log^2R$. Consequently the [twin-prime upper bound from a quadratic sieve](../../../../../twin-prime-upper-bound-from-a-quadratic-sieve.md) is

$$
A(x)\ll R+\frac{x}{\log^2R}+R^4\ll\frac{x}{\log^2x}.
$$

Finally, [Abel summation](../../../../../abel-s-summation-formula.md) gives

$$
\sum_{\substack{p\le X\\p,p+2\text{ prime}}}\frac1p=\frac{A(X)}X+\int_2^X\frac{A(t)}{t^2}\,dt.
$$

The tail is dominated by $\int_3^\infty dt/(t\log^2t)<\infty$. Thus [reciprocal-sum convergence from a counting bound](../../../../../reciprocal-sum-convergence-from-a-counting-bound.md) proves convergence of the first reciprocal sum. The second is smaller termwise. We have proved [Brun's theorem](../../../../../brun-s-theorem.md):

$$
\boxed{\sum_{p,p+2\text{ prime}}\left(\frac1p+\frac1{p+2}\right)<\infty.}
$$

Counting each twin prime just once changes at most a finite repetition and gives the same conclusion.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
