<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [divergence-form elliptic operator](../../../../../../divergence-form-elliptic-operator.md) use the [weak subsolution](../../../../../../weak-subsolution-of-a-divergence-form-elliptic-equation.md) convention $\int a^{ij}D_juD_i\varphi\leq0$ for nonnegative [test functions](../../../../../../test-function.md). Set $u_\varepsilon=u+\varepsilon$ and test with $\varphi=\eta^2u_\varepsilon^{\beta-1}$, where $\beta>1$. The [Sobolev chain rule](../../../../../../sobolev-chain-rule.md) makes this test admissible; boundedness and the positive regularization control the derivative of its power. Ellipticity and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) give, with $X=\int|Du|^2u_\varepsilon^{\beta-2}\eta^2$ and $Y=\int u_\varepsilon^\beta|D\eta|^2$,

$$
\lambda(\beta-1)X\leq2\Lambda_*X^{1/2}Y^{1/2},\qquad
\Lambda_*\geq\operatorname*{ess\,sup}\|a(x)\|_{\mathrm{op}}.
$$

Division when $X>0$, and the trivial case $X=0$, establish the [power Caccioppoli inequality](../../../../../../power-caccioppoli-inequality.md). Letting $\varepsilon\downarrow0$ gives

$$
\boxed{\int|Du|^2u^{\beta-2}\eta^2\leq
\frac{4\Lambda_*^2}{\lambda^2(\beta-1)^2}\int u^\beta|D\eta|^2.}
$$

For $1<\beta<2$ this limit uses the [Fatou lemma](../../../../../../fatou-s-lemma.md); the [gradient of a Sobolev function vanishes on a level set](../../../../../../gradient-of-a-sobolev-function-vanishes-on-a-level-set.md), so the weighted integrand is assigned zero on $\{u=0\}$. The same regularization justifies differentiating $u^{\beta/2}\eta$ in $W^{1,2}$.

The PDF bounds individual entries by $\Lambda$. Then $\Lambda_*\leq n\Lambda$: dimensional factors are included in the ellipticity constants when the first estimate is written as $C(\lambda,\Lambda)$. With literal entrywise bounds, the explicit valid constant displayed here is $4n^2\Lambda^2/\lambda^2$. If $\Lambda$ bounds the [operator norm](../../../../../../operator-norm.md) instead, it is $4\Lambda^2/\lambda^2$. This distinction does not alter any later conclusion, whose constants explicitly depend on $n$.

For $n\geq3$, put $\sigma=n/(n-2)$. Apply the [Sobolev inequality](../../../../../../sobolev-inequality.md) to $g=u^{\beta/2}\eta$ and use

$$
\int|Dg|^2\leq\frac{\beta^2}{2}\int|Du|^2u^{\beta-2}\eta^2
+2\int u^\beta|D\eta|^2.
$$

For $\beta\geq p>1$, $\beta/(\beta-1)\leq p/(p-1)$, so the resulting constant is uniform in $\beta$. Taking a cutoff equal to one on $B_r$, supported in $B_R$, with $|D\eta|\leq C/(R-r)$, yields

$$
\boxed{\|u\|_{L^{\sigma\beta}(B_r)}
\leq C_p^{1/\beta}(R-r)^{-2/\beta}\|u\|_{L^\beta(B_R)},\qquad\beta\geq p.}
$$

At $R=1$ a compactly supported cutoff can still be chosen with this bound by leaving an outer margin; alternatively pass to the limit from smaller radii.

For [Moser iteration](../../../../../../moser-iteration.md), set $\beta_j=p\sigma^j$ and $r_j=1/2+2^{-j-1}$. Repeated use of the preceding estimate bounds the successive norms by

$$
\|u\|_{L^p(B_1)}\prod_{j\geq0}C_p^{1/\beta_j}2^{(2j+4)/\beta_j}.
$$

This product is finite because

$$
\sum_{j\geq0}\frac1{\beta_j}=\frac n{2p},\qquad
\sum_{j\geq0}\frac j{\beta_j}=\frac{n(n-2)}{4p}.
$$

As the exponents tend to infinity, their norms on the [Euclidean ball](../../../../../../euclidean-ball.md) of radius $1/2$ tend to its [essential supremum](../../../../../../essential-supremum.md). Therefore

$$
\boxed{\|u\|_{L^\infty(B_{1/2})}\leq C_{n,p,\lambda,\Lambda}\|u\|_{L^p(B_1)}.}
$$

The power $\beta$ is independent of the exponents of [Hölder continuity](../../../../../../holder-condition.md) in earlier questions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
