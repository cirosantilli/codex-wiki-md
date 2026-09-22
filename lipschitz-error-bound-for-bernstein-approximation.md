# Lipschitz error bound for Bernstein approximation

↑ **Parent:** [Bernstein polynomial](bernstein-polynomial.md)

If $f$ is [Lipschitz continuous](lipschitz-continuity.md) on $[0,1]$ with [Lipschitz constant](lipschitz-constant.md) $L$, then [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) and the [binomial distribution](binomial-distribution.md) [variance](variance-split.md) give

$$
|B_nf(x)-f(x)|
\leq L\mathbb E|K/n-x|
\leq L\sqrt{\mathbb E[(K/n-x)^2]}
=L\sqrt{\frac{x(1-x)}n}
\leq\frac L{2\sqrt n}.
$$

This is an explicit error guarantee, rather than only an existence theorem. For the [Bernstein approximation of a corner](bernstein-approximation-of-a-corner.md), choosing $n\geq2500$ guarantees [supremum norm](supremum-norm.md) error at most $0.01$; $n>2500$ guarantees error strictly less than $0.01$. The guarantee is sufficient, not optimal.

<a id="image-the-corner-s-approximation-error-stays-below-a-binomial-distribution-variance-bound"></a>
![](bernstein-corner-errors-and-probability-bound.png)

**[Figure 2](#image-the-corner-s-approximation-error-stays-below-a-binomial-distribution-variance-bound). The corner's approximation error stays below a binomial distribution variance bound**. Left: error profiles for $|x-1/2|$ and selected [Bernstein polynomials](bernstein-polynomial.md). Right: for even positive degrees, exact maximum error $\binom n{n/2}/2^{n+1}$ is compared with the sufficient bound $1/(2\sqrt n)$. All values are model calculations; no experimental data are represented.

For this specific target, the error reaches its maximum at $x=1/2$. Indeed the [derivative](derivative.md) of $B_nf$ is a weighted average of the slopes $n[f((k+1)/n)-f(k/n)]$, all in $[-1,1]$: see [derivatives of Bernstein polynomials](derivatives-of-bernstein-polynomials.md). Subtracting the target makes the error nondecreasing to the left of the corner and nonincreasing to its right. For even $n\geq2$, the symmetric [binomial distribution](binomial-distribution.md) at $x=1/2$ gives the exact value

$$
\|B_nf-f\|_\infty=B_nf(1/2)
=\frac1{n2^n}\sum_{k=0}^n\binom nk\left|k-\frac n2\right|
=\frac{\binom n{n/2}}{2^{n+1}}.
$$

The last equality follows by pairing terms about $n/2$ and telescoping the [binomial coefficients](binomial-coefficient-split.md). It gives $1/4$ for $n=2$ and $3/16$ for $n=4$.

## ↑ Ancestors (8)

1. [Bernstein polynomial](bernstein-polynomial.md)
2. [Weierstrass approximation theorem](weierstrass-approximation-theorem.md)
3. [Stone-Weierstrass theorem](stone-weierstrass-theorem.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Bernstein approximation of a corner](bernstein-approximation-of-a-corner.md)
