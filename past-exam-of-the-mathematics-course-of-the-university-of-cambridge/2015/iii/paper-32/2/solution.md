<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Put $S=X^{\mathsf T}X$, which is a [positive-definite matrix](../../../../../positive-definite-matrix.md) by the full column-rank assumption. The [ordinary least squares](../../../../../ordinary-least-squares.md) estimator is

$$
\boxed{\widehat\beta^{OLS}=S^{-1}X^{\mathsf T}Y.}
$$

For [ridge regression](../../../../../ridge-regression.md) use the criterion $\tfrac12\|Y-Xb\|_2^2+\tfrac\lambda2\|b\|_2^2$. Differentiating gives

$$
\boxed{\widehat\beta^R_\lambda=(S+\lambda I)^{-1}X^{\mathsf T}Y.}
$$

If instead the squared-error term is normalized by $n$, replace $\lambda$ in this formula and the calculations below by $n\lambda$. Only the scale of the tuning parameter changes.

As usual for this [linear regression](../../../../../linear-regression-split.md) model, use zero-mean errors; more generally $X^{\mathsf T}\mathbb E\varepsilon=0$ suffices. Since the columns are centred, $X^{\mathsf T}\mathbf1=0$, so the random centring term disappears from both estimators. Thus

$$
\widehat\beta^{OLS}=\beta^0+S^{-1}X^{\mathsf T}\varepsilon,\qquad
\operatorname{Cov}(\widehat\beta^{OLS})=\sigma^2S^{-1}.
$$

Let $A=(S+\lambda I)^{-1}$. The [bias](../../../../../bias-of-an-estimator.md) and [covariance matrix](../../../../../covariance-matrix.md) of the [ridge regression](../../../../../ridge-regression.md) estimator are

$$
\mathbb E\widehat\beta^R_\lambda-\beta^0=-\lambda A\beta^0,\qquad
\operatorname{Cov}(\widehat\beta^R_\lambda)=\sigma^2ASA.
$$

The [bias-variance decomposition of mean squared error](../../../../../bias-variance-decomposition-of-mean-squared-error.md) therefore represents directional risk by the quadratic forms

$$
R_R(x)=x^{\mathsf T}\left(\sigma^2ASA+\lambda^2A\beta^0\beta^{0\mathsf T}A\right)x,\qquad
R_{OLS}(x)=\sigma^2x^{\mathsf T}S^{-1}x.
$$

Their difference has the useful factorization

$$
\begin{aligned}
R_{OLS}(x)-R_R(x)
&=\lambda x^{\mathsf T}A\left(2\sigma^2I+\lambda\sigma^2S^{-1}-\lambda\beta^0\beta^{0\mathsf T}\right)Ax.
\end{aligned}
$$

To check it, multiply $S^{-1}-ASA$ on both sides by $A^{-1}=S+\lambda I$: the resulting matrix is $(S+\lambda I)S^{-1}(S+\lambda I)-S=2\lambda I+\lambda^2S^{-1}$.

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $\beta^0\beta^{0\mathsf T}\preceq\|\beta^0\|_2^2I$ in the [Loewner order](../../../../../loewner-order.md). Therefore the middle matrix is [positive-definite](../../../../../positive-definite-bilinear-form.md) whenever $\lambda\|\beta^0\|_2^2<2\sigma^2$. For example,

$$
\boxed{\lambda=\frac{\sigma^2}{1+\|\beta^0\|_2^2}>0}
$$

works, independently of the [eigenvalues](../../../../../eigenvalue.md) of $S$. Since $A$ is invertible, the risk difference is strictly positive for every nonzero $x$, in particular simultaneously for every unit $x^*$. This proves [uniform directional risk improvement by ridge regression](../../../../../uniform-directional-risk-improvement-by-ridge-regression.md). For the normalized-loss convention, take the displayed choice divided by $n$.

For the final assertion, fix any $\lambda>0$ and choose a unit [eigenvector](../../../../../eigenvector.md) $v$ of $S$ with [eigenvalue](../../../../../eigenvalue.md) $d>0$. Put $x^*=v$ and $\beta^0=Bv$. Directly,

$$
R_R(v)=\frac{\lambda^2B^2+\sigma^2d}{(d+\lambda)^2},\qquad
R_{OLS}(v)=\frac{\sigma^2}{d}.
$$

Choosing

$$
\boxed{B^2>\frac{(d+\lambda)^2}{\lambda^2}\left(\delta+\frac{\sigma^2}{d}\right)}
$$

makes the squared bias alone greater than $R_{OLS}(v)+\delta$, proving the required strict inequality. Thus [unbounded directional risk of fixed ridge shrinkage](../../../../../unbounded-directional-risk-of-fixed-ridge-shrinkage.md) is compatible with the existence of a beneficial signal-dependent small penalty: no fixed positive penalty uniformly improves risk over all possible signals.

The mean assumption matters if the printed covariance condition is read in isolation. With $n=2$, $X=(1,-1)^{\mathsf T}$, $\beta^0=10$, $\sigma^2=1$ and $\mathbb E\varepsilon=-5X$, the columns and response are still centred and $\operatorname{Var}\varepsilon=I$, but the [ordinary least squares](../../../../../ordinary-least-squares.md) risk is $25.5$. Writing $a=2/(2+\lambda)$, the [ridge regression](../../../../../ridge-regression.md) risk is $(5a-10)^2+\tfrac12a^2=100-100a+25.5a^2>25.5$ for every $0<a<1$. Hence the standard zero-mean regression-error convention, or its stated orthogonality version, is necessary for the first risk comparison; covariance alone is insufficient.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
