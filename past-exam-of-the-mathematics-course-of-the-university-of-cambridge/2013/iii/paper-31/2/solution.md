<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the following normalization for the [Lasso estimator](../../../../../lasso.md), leaving the intercept unpenalized:

$$
(\widehat a,\widehat\beta_\lambda^L)\in\operatorname*{argmin}_{a\in\mathbb R,\ b\in\mathbb R^p}\left\{\frac1{2n}\|Y-a\mathbf1_n-Xb\|_2^2+\lambda\|b\|_1\right\}.
$$

A different convention for the factor in front of squared error rescales the [regularization parameter](../../../../../regularization-parameter.md). With this convention, centering of the columns gives $\widehat a=\overline Y$. Put $Y_c=Y-\overline Y\mathbf1_n$ and $\epsilon_c=\epsilon-\overline\epsilon\mathbf1_n$. Then $Y_c=X\beta+\epsilon_c$ and $X^T\epsilon_c=X^T\epsilon$. The [Lasso](../../../../../lasso.md) minimizes $\|Y_c-Xb\|_2^2/(2n)+\lambda\|b\|_1$. A minimum exists since $\lambda>0$ makes this continuous objective coercive; the bound below holds for every minimizer.

We first prove the needed [sharp two-sided Gaussian tail bound](../../../../../sharp-two-sided-gaussian-tail-bound.md). If $Z$ is standard normal and $t\geq0$, substituting $u=t+v$ in its density integral yields

$$
\begin{aligned}
\mathbb P(|Z|>t)&=\sqrt{\frac2\pi}\int_t^\infty e^{-u^2/2}\,du\\
&=e^{-t^2/2}\sqrt{\frac2\pi}\int_0^\infty e^{-v^2/2-tv}\,dv\leq e^{-t^2/2}.
\end{aligned}
$$

The last integral without $e^{-tv}$ is one after multiplication by $\sqrt{2/\pi}$. In particular this proves the two-sided bound with no extra factor of two.

Since $\|x_j\|_2^2=n$, each $x_j^T\epsilon/(\sigma\sqrt n)$ has a [standard normal distribution](../../../../../standard-normal-distribution.md). The [union bound](../../../../../boole-s-inequality.md), which does not require independent columns or independent scores, gives the [Gaussian score event for the Lasso](../../../../../gaussian-score-event-for-the-lasso.md)

$$
\mathcal E=\left\{\left\|\frac{X^T\epsilon}{n}\right\|_\infty\leq\frac\lambda2\right\},\qquad
\mathbb P(\mathcal E^c)\leq p\exp\left(-\frac{n\lambda^2}{8\sigma^2}\right)=p^{1-A^2/8}.
$$

Here the positive tuning choice presupposes $p\geq2$ and $\sigma>0$. When the displayed lower bound is negative it is simply a valid, vacuous lower bound. For $p=1$ the prescribed parameter is zero and the probability lower bound is also zero, so no positive-parameter assertion is supplied by that prescription.

Let $\delta=\widehat\beta_\lambda^L-\beta$ and $Q=\|X\delta\|_2^2/n$. Comparing the [Lasso](../../../../../lasso.md) objective at its minimizer and at $\beta$ and expanding the squares gives the [Basic inequality for the Lasso](../../../../../basic-inequality-for-the-lasso.md)

$$
Q\leq \frac2n\epsilon^TX\delta+2\lambda(\|\beta\|_1-\|\beta+\delta\|_1).
$$

On $\mathcal E$, the stochastic term is at most $\lambda\|\delta\|_1$. Because $\beta_N=0$, the [triangle inequality](../../../../../triangle-inequality.md) gives

$$
\|\beta\|_1-\|\beta+\delta\|_1\leq\|\delta_S\|_1-\|\delta_N\|_1.
$$

It follows that

$$
Q+\lambda\|\delta_N\|_1\leq3\lambda\|\delta_S\|_1.
$$

In particular $\|\delta_N\|_1\leq3\|\delta_S\|_1$, which is the [Lasso cone condition](../../../../../lasso-cone-condition.md). The given [Compatibility condition for the Lasso](../../../../../compatibility-condition-for-the-lasso.md) is therefore applicable and gives $\|\delta_S\|_1\leq\sqrt{sQ}/\phi_0$.

Adding $\lambda\|\delta_S\|_1$ to the preceding inequality and using compatibility now yields

$$
Q+\lambda\|\delta\|_1\leq4\lambda\|\delta_S\|_1\leq\frac{4\lambda\sqrt{sQ}}{\phi_0}\leq\frac Q2+\frac{8\lambda^2s}{\phi_0^2}.
$$

The last inequality is just the nonnegativity of $(\sqrt{Q/2}-\sqrt8\lambda\sqrt{s}/\phi_0)^2$. Thus $Q+2\lambda\|\delta\|_1\leq16\lambda^2s/\phi_0^2$, and dropping one nonnegative coefficient-error term gives

$$
\boxed{\frac1n\|X(\widehat\beta_\lambda^L-\beta)\|_2^2+\lambda\|\widehat\beta_\lambda^L-\beta\|_1\leq\frac{16A^2}{\phi_0^2}\frac{\sigma^2s\log p}{n}.}
$$

This [prediction and coefficient error bound for compatible Lasso](../../../../../prediction-and-coefficient-error-bound-for-compatible-lasso.md) holds on $\mathcal E$, and hence with the required probability. If $s=0$, the earlier basic inequality directly forces $\delta=0$ on $\mathcal E$, so the zero right side is also correct.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
