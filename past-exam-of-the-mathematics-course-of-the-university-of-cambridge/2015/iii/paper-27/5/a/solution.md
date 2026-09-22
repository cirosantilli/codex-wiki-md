<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the level-$D$ convention used here, the [Selberg upper-bound sieve](../../../../../../selberg-upper-bound-sieve.md) states that a nonnegative sequence with [sieve distribution](../../../../../../sieve-distribution.md) $A_d=Xg(d)+r(d)$ satisfies

$$
S\leq\frac XJ+\sum_{d\leq D}3^{\omega(d)}|r(d)|,\qquad
J=\sum_{\substack{d\leq\sqrt D\\d\text{ squarefree}\\p\mid d\Rightarrow p\in\mathcal P}}\prod_{p\mid d}\frac{g(p)}{1-g(p)}.
$$

It follows by minimizing the quadratic form with the [Selberg sieve weights](../../../../../../selberg-sieve-weights.md) and using the [Selberg least-common-multiple weights](../../../../../../selberg-least-common-multiple-weights.md) bound $|\lambda_d|\leq3^{\omega(d)}$.

Sieve the interval $x<n\leq x+z$ by two and by the [primes](../../../../../../prime-number.md) congruent to three modulo four, up to $L=\sqrt D$. The interval [divisor](../../../../../../divisor.md) counts give

$$
A_d=\left\lfloor\frac{x+z}{d}\right\rfloor-\left\lfloor\frac xd\right\rfloor
=\frac zd+O(1).
$$

Thus $X=z$, $g(p)=1/p$, and $r(d)=O(1)$ uniformly in the location of the interval. Take $D=z^{1/2}$ and $L=z^{1/4}$.

To bound $J$, let $y=L^{1/4}$ and form the [Euler product](../../../../../../euler-product.md) over the forbidden [primes](../../../../../../prime-number.md) at most $y$. The given [reciprocal-prime sum in residue class one modulo four](../../../../../../reciprocal-prime-sum-in-residue-class-one-modulo-four.md), subtracted from the [Mertens second theorem](../../../../../../mertens-second-theorem.md), yields

$$
\sum_{\substack{p\leq y\\p=2\text{ or }p\equiv3\pmod4}}\frac1p
=\tfrac12\log\log y+O(1),\qquad
W=\prod_{\substack{p\leq y\\p=2\text{ or }p\equiv3\pmod4}}(1-1/p)^{-1}\asymp\sqrt{\log y}.
$$

Moreover, the [Mertens first theorem](../../../../../../mertens-first-theorem.md) bounds the logarithmic mean by $\sum_{p\leq y}(\log p)/p=\log y+O(1)\leq\tfrac12\log L$ for large $L$. The [truncated Euler-product lower bound](../../../../../../truncated-euler-product-lower-bound.md) gives $J\geq W/2\gg\sqrt{\log z}$.

The full-range [summatory bound for three to the prime omega](../../../../../../summatory-bound-for-three-to-the-prime-omega.md) bounds the error by $O(D\log^2D)=O(\sqrt z\log^2z)$, which is $O(z/\sqrt{\log z})$. Every integer whose [prime factors](../../../../../../prime-factor.md) are all congruent to one modulo four survives this finite sieve. Therefore the [half-dimensional interval sieve](../../../../../../half-dimensional-interval-sieve.md) gives

$$
\boxed{\#\{x<n\leq x+z:\ p\mid n\Rightarrow p\equiv1\pmod4\}\ll\frac z{\sqrt{\log z}}.}
$$

The constants are independent of $x$. Enlarging them covers the bounded range of $z$ before the asymptotic product estimates apply, so the result holds throughout $1000\leq z\leq x$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
