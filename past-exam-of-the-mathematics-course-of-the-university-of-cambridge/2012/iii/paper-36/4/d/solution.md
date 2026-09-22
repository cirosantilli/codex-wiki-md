<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First use the additional admitted form of the [efficient score](../../../../../../efficient-score.md). Write $\widetilde\ell=e\zeta(X)$ and let $\tau^2=E_f\varepsilon^2>0$. The difference $\dot\ell-\widetilde\ell$ is the [orthogonal projection](../../../../../../orthogonal-projection.md) onto the [nuisance tangent space](../../../../../../nuisance-tangent-space.md). Part (c) makes every $e\psi(X)$ orthogonal to that space. Therefore, for all $\psi\in L^2(v)$,

$$
0=E[(h_\theta(X)\rho(\varepsilon)-\varepsilon\zeta(X))\varepsilon\psi(X)]
=E_v\bigl[\{h_\theta E_f(\varepsilon\rho)-\tau^2\zeta\}\psi\bigr].
$$

The [function](../../../../../../function-split.md) in braces belongs to [L2 space](../../../../../../l2-space-is-a-hilbert-space.md); choosing it as $\psi$ shows it vanishes $v$-almost everywhere. Hence the required conditional deduction is

$$
\boxed{\widetilde\ell_{\theta,\eta}(x,e)
=-e\,\frac{\int s f'(s)\,ds}{\int s^2f(s)\,ds}\,h_\theta(x).}
$$

Under the regular tail condition $s f(s)\to0$ at both infinities, [integration by parts](../../../../../../integration-by-parts.md) gives $\int s f'(s)\,ds=-1$, and the formula becomes $e h_\theta(x)/\tau^2$. This also confirms the sign.

**The admitted product form is an extra restriction; it does not follow for every independent-error regression model.** To locate the restriction precisely, suppose the error-density nuisance [statistical paths](../../../../../../statistical-path.md) preserve both normalization and mean to first order. Their closed [mean-preserving error tangent space](../../../../../../mean-preserving-error-tangent-space.md) is $\{\gamma:E_f\gamma=E_f(\varepsilon\gamma)=0\}$. The full [nuisance tangent space](../../../../../../nuisance-tangent-space.md) is the orthogonal sum of this space and the centered [functions](../../../../../../function-split.md) of $X$.

For completeness, bounded [functions](../../../../../../function-split.md) satisfying the two constraints are dense in the error space. Truncate an arbitrary element, subtract its [expected value](../../../../../../expected-value.md), and then subtract a multiple of a fixed bounded centered [function](../../../../../../function-split.md) $q$ with $E_f(\varepsilon q)\ne0$. Such a $q$ exists by truncating $\varepsilon$, since $\tau^2>0$. The correction coefficients tend to zero by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), so the corrected truncations converge in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md).

Let $m=E_vh_\theta(X)$. With $E_f\rho=0$ and $E_f(\varepsilon\rho)=1$, the [orthogonal projection](../../../../../../orthogonal-projection.md) of $h_\theta(X)\rho(\varepsilon)$ onto the error nuisance space is $m\{\rho(\varepsilon)-\varepsilon/\tau^2\}$; its projection onto the covariate nuisance space is zero. Thus the general [efficient score in independent-error regression](../../../../../../efficient-score-in-independent-error-regression.md) is

$$
\boxed{\widetilde\ell=(h_\theta(X)-m)\rho(\varepsilon)+\frac{m\varepsilon}{\tau^2},
\qquad
\widetilde I=\operatorname{Var}_v(h_\theta)E_f\rho^2+\frac{m^2}{\tau^2}.}
$$

The [orthogonality](../../../../../../orthogonal-vectors.md) of the two terms gives the displayed [efficient information](../../../../../../efficient-information.md). For a [normal distribution](../../../../../../normal-distribution.md) of the error, $\rho(e)=e/\tau^2$, so this reduces to the admitted formula. It also does so when $h_\theta$ is constant.

A concrete counterexample to the generality of the admission is $g_\theta(x)=\theta x$, with $X$ uniform on $[-1,1]$ and independent standard [logistic distribution](../../../../../../logistic-distribution.md) error. Here $m=0$ and $\rho(e)=\tanh(e/2)$, so the actual [efficient score](../../../../../../efficient-score.md) is $x\tanh(e/2)$. It cannot equal $e\zeta(x)$ because $\tanh(e/2)/e$ is not constant. This [score function](../../../../../../informant-function.md) is already orthogonal to every nuisance [score function](../../../../../../informant-function.md): its factor $X$ is centered against error-only directions, and its factor $\rho(\varepsilon)$ is centered against covariate-only directions. **The requested formula is valid under its stated additional admission, with the general independent-error formula above explaining its limits.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
