<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the unbiased [sample covariance matrix](../../../../../../sample-covariance-matrix.md)

$$
S=\frac1{n-1}\sum_{j=1}^n(X_j-\bar X)(X_j-\bar X)^T,
$$

and assume $\Sigma$ is [positive-definite](../../../../../../positive-definite-bilinear-form.md) and $n>p$, so $S$ is invertible almost surely. For a nonzero fixed direction $a$, the observations $Y_j=a^TX_j$ have mean $a^T\mu$ and [variance](../../../../../../variance-split.md) $a^T\Sigma a$. Their squared [Student t-test](../../../../../../student-s-t-test.md) statistic for the projected null mean is

$$
t_a^2=\frac{n\{a^T(\bar X-\mu_0)\}^2}{a^TSa}.
$$

Put $b=\bar X-\mu_0$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
(a^Tb)^2=\{(S^{1/2}a)^T(S^{-1/2}b)\}^2
\le(a^TSa)(b^TS^{-1}b),
$$

with equality when $a$ is proportional to $S^{-1}b$, if $b\ne0$. For $b=0$ every projected statistic is zero. Maximizing the squared discrepancy over directions therefore gives [Hotelling's T-squared statistic](../../../../../../hotelling-s-t-squared-statistic.md):

$$
\boxed{T^2=\max_{a\ne0}t_a^2=n(\bar X-\mu_0)^TS^{-1}(\bar X-\mu_0).}
$$

This uses the squared generalized [Rayleigh quotient](../../../../../../rayleigh-quotient.md). The preliminary formula on the printed cover has an unsquared numerator and is not valid as written: setting $a=tC^{-1}b$ makes that ratio $1/t$ for $b\ne0$, so it is unbounded. The displayed Cauchy-Schwarz argument supplies the needed corrected identity independently.

Under the null, let $Z=\sqrt n(\bar X-\mu_0)$ and $C=(n-1)S$. Then $Z\sim N_p(0,\Sigma)$, $C\sim W_p(n-1,\Sigma)$, and $Z,C$ are independent. To see these sample properties, apply an orthogonal transformation to the $n$ observation indices with first row $n^{-1/2}(1,\ldots,1)$. Its first centered row is $Z$; its other $n-1$ rows are independent $N_p(0,\Sigma)$ residual contrasts, independent of the first. Their outer products sum to $C$, establishing the [Wishart distribution](../../../../../../wishart-distribution.md) and [independence](../../../../../../independent-random-variables.md).

Since $T^2=(n-1)Z^TC^{-1}Z$, use the supplied Gaussian-Wishart quadratic-form law with $k=n-1$ to obtain

$$
\boxed{\frac{n-p}{p(n-1)}T^2\sim F_{p,n-p}\quad\text{under }H_0.}
$$

Thus a level-$\eta$ test rejects when this scaled statistic exceeds the $(1-\eta)$ quantile of the [F-distribution](../../../../../../f-distribution.md). The Gaussian-Wishart law requires [independence](../../../../../../independent-random-variables.md); it holds here because of the orthogonal sample decomposition. Its printed use of $X$ instead of the introduced $Z$ is a notational slip. A fixed-direction Student law alone would not calibrate the maximized statistic, because its maximizing direction depends on the sample.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
