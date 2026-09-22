<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Poisson trick](../../../../../../poisson-trick.md) introduces $\lambda_i=\log\mu_{i1}$. With an exactly flat log-rate prior, the baseline prior measure is $du_i/u_i$. For $n_i>0$,

$$
\int_0^\infty u_i^{n_i-1}e^{-S_i u_i}\,du_i
=\Gamma(n_i)S_i^{-n_i}.
$$

Thus [flat log-rate marginalization gives the multinomial likelihood](../../../../../../flat-log-rate-marginalization-gives-the-multinomial-likelihood.md):

$$
\boxed{p(\mathbf y\mid\beta)\propto
\prod_i\frac{\exp\{\sum_k y_{ik}\eta_{ik}\}}{S_i^{n_i}}.}
$$

Alternatively, independent Poisson counts conditional on their total are exactly [multinomial distributions](../../../../../../multinomial-distribution.md) with probabilities $e^{\eta_{ik}}/S_i$. Locally uniform coefficient priors make the coefficient posterior proportional to this likelihood within their flat region.

The printed BUGS prior is a proper [normal distribution](../../../../../../normal-distribution.md) on $\lambda_i$, with variance $s^2=10^5$, since BUGS uses precision as its second argument. It is broad but not exactly flat. Substitution $v=S_i u_i$ shows that, apart from a coefficient-independent constant, the integrated likelihood is the multinomial kernel times the [Gaussian log-rate correction to the Poisson trick](../../../../../../gaussian-log-rate-correction-to-the-poisson-trick.md)

$$
\boxed{R_i(S_i)=
\mathbb E_{V\sim\operatorname{Gamma}(n_i,1)}
\left[\exp\left\{-\frac{(\log V-\log S_i)^2}{2s^2}\right\}\right].}
$$

It depends on the coefficients through $S_i$. [Dominated convergence](../../../../../../dominated-convergence-theorem.md) gives $R_i\to1$ as $s^2\to\infty$, so the finite-variance code yields **an approximation to the multinomial posterior**, not exact equality. Large log rates can make prior sensitivity relevant.

The cell-wise factors form a standard [Poisson regression](../../../../../../poisson-regression.md), convenient for BUGS. They avoid an explicitly constrained count vector and permit scalar log-concave updates for intercepts and coefficients; an exactly flat-log-rate implementation also gives gamma conditional baseline rates. This can be computationally efficient, although the actual log-normal baseline prior is not gamma-conjugate and introduces $I$ nuisance intercepts. Efficiency depends on the update scheme.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
