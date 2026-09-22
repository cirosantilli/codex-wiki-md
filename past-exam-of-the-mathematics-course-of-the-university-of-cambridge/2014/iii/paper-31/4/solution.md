<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write the year-$j$ count as a sum of its $m_j$ individual counts, with $m_j>0$. The specified [conditional independence](../../../../../conditional-independence.md) within that year gives

$$
\mathbb E[Y_j\mid\Theta]=m_j\mu(\Theta),\qquad
\operatorname{Var}(Y_j\mid\Theta)=m_j\sigma^2(\Theta).
$$

Dividing by $m_j$ and scaling the [conditional variance](../../../../../conditional-variance.md) by $m_j^{-2}$ therefore gives

$$
\boxed{\mathbb E[X_j\mid\Theta]=\mu(\Theta),\qquad
\operatorname{Var}(X_j\mid\Theta)=\frac{\sigma^2(\Theta)}{m_j}.}
$$

This is the [Bühlmann–Straub model](../../../../../buhlmann-straub-model.md): larger exposures reduce the process noise in a year's average.

Define the population parameters and total observed exposure by

$$
m_0=\mathbb E[\mu(\Theta)],\qquad
v=\mathbb E[\sigma^2(\Theta)],\qquad
a=\operatorname{Var}(\mu(\Theta)),\qquad
W=\sum_{j=1}^n m_j.
$$

Here $v$ is the [expected process variance](../../../../../expected-process-variance.md) and $a$ the [variance of hypothetical means](../../../../../variance-of-hypothetical-means.md). Assume finite second moments. The [law of total variance](../../../../../law-of-total-variance.md) gives $\operatorname{Var}(X_j)=a+v/m_j$, and conditional independence between years gives $\operatorname{Cov}(X_j,X_k)=a$ for $j\ne k$: their only shared variation is the latent conditional mean.

To derive the [Bühlmann–Straub credibility estimate](../../../../../buhlmann-straub-credibility-estimate.md), minimize [mean squared error](../../../../../mean-squared-error.md) among affine estimates of $\mu(\Theta)$. For coefficients $b_j$ and $B=\sum_jb_j$, the optimal intercept is $m_0(1-B)$. Centering at $m_0$ and conditioning on $\Theta$ shows that the resulting error is

$$
\mathbb E\left[\left(\mu(\Theta)-m_0(1-B)-\sum_jb_jX_j\right)^2\right]
=a(1-B)^2+v\sum_j\frac{b_j^2}{m_j}.
$$

The cross term vanishes because $X_j-\mu(\Theta)$ has conditional mean zero; the conditional noise cross terms vanish by the between-year independence assumption.

For fixed $B$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
B^2\le\left(\sum_j\frac{b_j^2}{m_j}\right)W,
$$

with equality when $b_j=B m_j/W$. Minimize the remaining quadratic $a(1-B)^2+(v/W)B^2$. Its minimizing value is the [Bühlmann–Straub credibility factor](../../../../../buhlmann-straub-credibility-factor.md)

$$
\boxed{Z=\frac{Wa}{Wa+v}=\frac{W}{W+v/a}\quad(a>0).}
$$

The experience term is exposure-weighted:

$$
\overline X_w=\frac{\sum_jm_jX_j}{W}=\frac{\sum_jy_j}{W},\qquad
\widehat\mu=Z\overline X_w+(1-Z)m_0.
$$

Since the future conditional mean count is $m_{n+1}\mu(\Theta)$, multiplying the optimal estimate by the known future exposure gives

$$
\boxed{\widehat{\mathbb E[Y_{n+1}\mid\Theta]}
=m_{n+1}\left[Z\frac{\sum_{j=1}^n y_j}{\sum_{j=1}^n m_j}
+(1-Z)\mathbb E[\mu(\Theta)]\right].}
$$

It is the best affine [linear least-squares projection](../../../../../linear-least-squares-projection.md), not a claim that the exact conditional expectation given all data is always affine. If $a=0$, the conditional mean is a known constant almost surely and one takes $Z=0$; if $v=0<a$, the observations reveal it without process noise and $Z=1$. The ordinary case has $a,v>0$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
