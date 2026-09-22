<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For the unit-modulus [prime](../../../../../prime-number.md) values in this question, the [Granville-Soundararajan distance](../../../../../pretentious-distance.md) is

$$
\boxed{D(f,g;X)^2=\sum_{p\leq X}\frac{1-\operatorname{Re}(f(p)\overline{g(p)})}{p}
=\frac12\sum_{p\leq X}\frac{|f(p)-g(p)|^2}{p}.}
$$

The second identity uses $|f(p)|=|g(p)|=1$. Thus it is the [Euclidean distance](../../../../../euclidean-distance.md) between the finite weighted vectors $(f(p)/\sqrt{2p})_{p\leq X}$ and $(g(p)/\sqrt{2p})_{p\leq X}$. Nonnegativity, symmetry and the [triangle inequality](../../../../../triangle-inequality.md) follow from that [norm](../../../../../norm.md) representation, and it vanishes exactly when the two prime-value vectors agree. This proves the [prime-restriction metric for pretentious distance](../../../../../prime-restriction-metric-for-pretentious-distance.md).

**On whole [arithmetic functions](../../../../../arithmetic-function.md) at fixed $X$ it is a [pseudometric](../../../../../pseudometric.md).** For example $f=\mathbf1$ and $g=\mu^2$ have identical values at every [prime](../../../../../prime-number.md) and zero distance for every $X$, but different values at four. Thus the literal identity-of-indiscernibles assertion needs the prime-restriction quotient.

Since $\mu(p)=-1$,

$$
D(1,\mu;X)^2=2\sum_{p\leq X}\frac1p.
$$

For completeness, [partial summation](../../../../../abel-s-summation-formula.md) and the prime-counting form of the [Prime number theorem](../../../../../prime-number-theorem.md) give

$$
\sum_{p\leq X}\frac1p=\frac{\pi(X)}X+\int_2^X\frac{\pi(u)}{u^2}\,du
=\log\log X+B_1+o(1).
$$

To verify the constant and the error, replace $\pi$ by $\operatorname{Li}+E$ in the first expression. Differentiating $\operatorname{Li}(u)/u$ shows its two contributions combine to $\log\log X$ plus a constant. The error integral converges absolutely because $|E(u)|/u^2\ll e^{-c\sqrt{\log u}}/u$, and $E(X)/X\to0$. This proves the [Mertens second theorem](../../../../../mertens-second-theorem.md) in the form needed here. In particular the [pretentious distance between one and the Möbius function](../../../../../pretentious-distance-between-one-and-the-mobius-function.md) satisfies

$$
\boxed{D(1,\mu;X)^2=2\log\log X+2B_1+o(1),\qquad D(1,\mu;X)\sim\sqrt{2\log\log X}.}
$$

For the last request, retain the earlier [prime](../../../../../prime-number.md) normalization $|f(p)|=1$; the proof also works with the weaker assumption $|f(p)|\leq1$. Without a bound on [prime](../../../../../prime-number.md) values, the original definition and the [absolute convergence](../../../../../absolute-convergence.md) of the displayed measure need not apply to an unrestricted [multiplicative arithmetic function](../../../../../multiplicative-function.md). For example $f(n)=\mu(n)^2n$ is multiplicative and squarefree-supported, but for $X>e$ the displayed measure has infinite positive mass: its [prime](../../../../../prime-number.md) terms alone are $\sum_p p^{-1/\log X}$, which diverges by the [Prime number theorem](../../../../../prime-number-theorem.md).

Put $L=\log X$, $\sigma=1+1/L$, and use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat\nu(t)=\int e^{-itu}\,d\nu(u)$. Since $f$ is supported on [squarefree integers](../../../../../squarefree-integer.md), the defining property of a [multiplicative arithmetic function](../../../../../multiplicative-function.md) gives the absolutely convergent [Euler product](../../../../../euler-product.md)

$$
\widehat\nu(t)=\sum_{n\geq1}\frac{f(n)}{n^{\sigma+it}}
=\prod_p\left(1+\frac{f(p)p^{-it}}{p^\sigma}\right).
$$

The bound on [prime](../../../../../prime-number.md) values gives $|f(n)|\leq1$ for squarefree $n$, so the [total variation norm of a measure](../../../../../total-variation-norm-of-a-measure.md) is bounded by $\zeta(\sigma)$; thus $\nu$ is a [finite measure](../../../../../finite-measure.md). Expanding the logarithm of the modulus, with an absolute $O(1)$ remainder since $\sum_pp^{-2\sigma}\ll1$, gives

$$
\log|\widehat\nu(t)|=\sum_p\frac{\operatorname{Re}(f(p)p^{-it})}{p^\sigma}+O(1).
$$

All constants here are uniform in $t$. Moreover

$$
\sum_pp^{-\sigma}=\log\zeta(\sigma)+O(1)=\log L+O(1),
$$

using the pole of the [Riemann zeta function](../../../../../riemann-zeta-function.md). The nonnegative deficits $1-\operatorname{Re}(f(p)p^{-it})$ give

$$
\sum_p\frac{1-\operatorname{Re}(f(p)p^{-it})}{p^\sigma}
\geq D(f,n^{it};X)^2-O(1).
$$

Indeed, the replacement of $p^{-\sigma}$ by $1/p$ for $p\leq X$ costs at most

$$
2\sum_{p\leq X}\frac{1-p^{-1/L}}p
\leq\frac2L\sum_{p\leq X}\frac{\log p}p=O(1),
$$

by the [Mertens first theorem](../../../../../mertens-first-theorem.md), while discarding the $p>X$ terms costs nothing in this lower bound. Thus the [large Fourier coefficient criterion for pretentiousness](../../../../../large-fourier-coefficient-criterion-for-pretentiousness.md) is

$$
|\widehat\nu(t)|\leq C\log X\,e^{-D(f,n^{it};X)^2}.
$$

In particular,

$$
|\widehat\nu(t)|\geq\delta\log X\ \Longrightarrow\
\boxed{D(f,n^{it};X)^2\leq\log(C/\delta)=O_\delta(1).}
$$

The comparison function is the [Archimedean character](../../../../../archimedean-character.md) $n^{it}$ with this sign because our [Fourier transform](../../../../../fourier-transform.md) uses $e^{-itu}$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
