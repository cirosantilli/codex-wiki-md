<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a positive integer $N$, a [Dirichlet character](../../../../../dirichlet-character.md) $\psi$ modulo $N$ is a [group homomorphism](../../../../../group-homomorphism.md) $(\mathbb Z/N\mathbb Z)^\times\to\mathbb C^\times$, extended periodically to the integers and set equal to zero on integers not coprime to $N$. Its nonzero values are [roots of unity](../../../../../root-of-unity.md). For $\operatorname{Re}s>1$, its [Dirichlet L-function](../../../../../dirichlet-l-function.md) is the absolutely convergent [Dirichlet series](../../../../../dirichlet-series.md)

$$
\boxed{L_N(\psi,s)=\sum_{n=1}^\infty\frac{\psi(n)}{n^s}=\prod_{p\nmid N}(1-\psi(p)p^{-s})^{-1}.}
$$

Complete multiplicativity of $\psi$ proves the [Euler product](../../../../../euler-product.md) by expanding each factor as a [geometric series](../../../../../geometric-series.md) and applying unique [integer factorization](../../../../../integer-factorization.md); absolute convergence justifies these rearrangements.

Suppose $\psi$ is a [nonprincipal Dirichlet character](../../../../../nonprincipal-dirichlet-character.md). Choose a unit $u$ with $\psi(u)\ne1$. Multiplication by $u$ permutes a complete residue system, so $\sum_{a=1}^N\psi(a)=\psi(u)\sum_{a=1}^N\psi(a)$, and the sum is zero. Consequently $A(x)=\sum_{n\le x}\psi(n)$ is bounded: complete periods contribute zero and the remaining incomplete period has at most $N$ terms. The [Abel summation formula](../../../../../abel-s-summation-formula.md) gives, initially for $\operatorname{Re}s>1$,

$$
L_N(\psi,s)=s\int_1^\infty A(x)x^{-s-1}\,dx.
$$

For $\operatorname{Re}s>0$ the integral converges, locally uniformly together with its derivatives in $s$, because on a compact set with $\operatorname{Re}s\ge\delta>0$ the differentiated integrands are bounded by constants times $x^{-1-\delta}(1+\log x)^k$. Thus [holomorphy of a Dirichlet series from bounded partial sums](../../../../../holomorphy-of-a-dirichlet-series-from-bounded-partial-sums.md) proves

$$
\boxed{L_N(\psi,s)\text{ is holomorphic on }\operatorname{Re}s>0.}
$$

For a nonreal $\psi$, the character $\psi^2$ is also nonprincipal. The supplied logarithmic [Euler product](../../../../../euler-product.md) yields, for real $\sigma>1$,

$$
\log\bigl(\zeta(\sigma)^3|L_N(\psi,\sigma)|^4|L_N(\psi^2,\sigma)|\bigr)=\sum_p\sum_{k\ge1}\frac{3+4\operatorname{Re}(\psi(p)^k)+\operatorname{Re}(\psi(p)^{2k})}{kp^{k\sigma}}.
$$

At a prime dividing $N$ the numerator is $3$. At every other prime put $\psi(p)^k=e^{i\theta}$; then the numerator is $3+4\cos\theta+\cos2\theta=2(1+\cos\theta)^2\ge0$. This [Euler product positivity for L-function nonvanishing](../../../../../euler-product-positivity-for-l-function-nonvanishing.md) proves that the product inside the logarithm is at least one. If $L_N(\psi,1)=0$, its holomorphy would give $L_N(\psi,\sigma)=O(\sigma-1)$. Meanwhile $L_N(\psi^2,\sigma)$ is bounded near one and the [Riemann zeta function](../../../../../riemann-zeta-function.md) has a simple [pole](../../../../../pole.md) there. The product would therefore be $O(\sigma-1)$ and tend to zero, a contradiction.

For a real nonprincipal $\psi$, suppose instead that $L_N(\psi,1)=0$. The product $H(s)=\zeta(s)L_N(\psi,s)$ would then be holomorphic on the whole half-plane $\operatorname{Re}s>0$, because the zero cancels the only zeta pole there. In $\operatorname{Re}s>1$ it has coefficients

$$
H(s)=\sum_{n\ge1}b_n n^{-s},\qquad b_n=\sum_{d\mid n}\psi(d).
$$

These are [nonnegative zeta-times-real-L coefficients](../../../../../nonnegative-zeta-times-real-l-coefficients.md). They are multiplicative, and their prime-power values are $k+1$ if $\psi(p)=1$, one or zero according as $k$ is even or odd if $\psi(p)=-1$, and one if $\psi(p)=0$. In particular $b_n\ge0$ and $b_{m^2}\ge1$ for every $m$.

The [Taylor series](../../../../../taylor-series.md) of the assumed holomorphic $H$ about $2$ converges in the disk $|s-2|<2$. Termwise differentiation of its absolutely convergent [Dirichlet series](../../../../../dirichlet-series.md) at $2$ gives $(-1)^kH^{(k)}(2)=\sum_n b_n(\log n)^k/n^2$. Evaluate the [Taylor series](../../../../../taylor-series.md) at $s=1/2$ and apply the [Tonelli theorem](../../../../../tonelli-theorem.md) to the resulting nonnegative terms:

$$
H(1/2)=\sum_{k\ge0}\frac{(3/2)^k}{k!}\sum_{n\ge1}\frac{b_n(\log n)^k}{n^2}=\sum_{n\ge1}\frac{b_n}{n^{1/2}}\ge\sum_{m\ge1}\frac1m=\infty.
$$

This contradicts holomorphy at $1/2$. The argument is the positive-coefficient mechanism of the [Landau theorem for a Dirichlet series with nonnegative coefficients](../../../../../landau-theorem-for-a-dirichlet-series-with-nonnegative-coefficients.md), with the needed step proved explicitly. Combining the real and nonreal cases gives the [nonvanishing of a nonprincipal Dirichlet L-function at one](../../../../../nonvanishing-of-a-nonprincipal-dirichlet-l-function-at-one.md):

$$
\boxed{L_N(\psi,1)\ne0\quad\text{for every nonprincipal }\psi.}
$$

Now let $a$ be coprime to $N$. The [Dirichlet theorem on primes in arithmetic progressions](../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md) asserts that infinitely many [prime numbers](../../../../../prime-number.md) satisfy $p\equiv a\pmod N$. To prove it, separate the first-power terms in the given logarithmic [Euler product](../../../../../euler-product.md):

$$
\log L_N(\psi,\sigma)=\sum_{p\nmid N}\frac{\psi(p)}{p^\sigma}+R_\psi(\sigma),\qquad \sigma>1.
$$

For $\sigma\ge1$, the remainder is bounded uniformly by

$$
|R_\psi(\sigma)|\le\sum_p\sum_{k\ge2}p^{-k}\le\sum_{n=2}^\infty\frac1{n(n-1)}=1.
$$

For a nonprincipal character, holomorphy and nonvanishing near one give a local [holomorphic logarithm](../../../../../holomorphic-logarithm.md). Along a short real interval to the right of one, this logarithm and the supplied continuous logarithm differ by a fixed integer multiple of $2\pi i$. Hence the [prime-character sum near one](../../../../../prime-character-sum-near-one.md) is bounded:

$$
\sum_{p\nmid N}\psi(p)p^{-\sigma}=O(1),\qquad \psi\ne\psi_0.
$$

For the [principal Dirichlet character](../../../../../principal-dirichlet-character.md) $\psi_0$,

$$
L_N(\psi_0,\sigma)=\zeta(\sigma)\prod_{p\mid N}(1-p^{-\sigma}),\qquad \sum_{p\nmid N}p^{-\sigma}=\log\frac1{\sigma-1}+O(1).
$$

The latter follows from the simple zeta pole and the bounded remainder. Finally [Orthogonality of Dirichlet characters](../../../../../orthogonality-of-dirichlet-characters.md) gives

$$
\sum_{\substack{p\text{ prime}\\p\equiv a\pmod N}}p^{-\sigma}=\frac1{\varphi(N)}\sum_{\psi\bmod N}\overline{\psi(a)}\sum_{p\nmid N}\psi(p)p^{-\sigma}=\frac1{\varphi(N)}\log\frac1{\sigma-1}+O(1).
$$

Here $\varphi$ is the [Euler totient function](../../../../../euler-totient-function.md). The right-hand side tends to infinity as $\sigma\downarrow1$, whereas a finite set of primes would give a bounded left-hand side. Therefore

$$
\boxed{\gcd(a,N)=1\implies\text{infinitely many primes }p\equiv a\pmod N.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
