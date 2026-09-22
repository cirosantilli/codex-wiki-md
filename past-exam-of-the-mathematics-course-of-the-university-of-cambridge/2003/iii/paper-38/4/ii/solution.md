<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here the [negative binomial distribution](../../../../../../negative-binomial-distribution.md) has mean parameter $\mu>0$ and size parameter $\theta>0$. Its support in the original PDF is all nonnegative integers; a finite endpoint appearing in the TeX aid would be incorrect. The [probability generating function](../../../../../../probability-generating-function.md), obtained from the generalized binomial series, is

$$
G(s)=\left(\frac{\theta}{\theta+\mu(1-s)}\right)^\theta.
$$

Differentiating at one gives $G'(1)=\mu$ and $G''(1)=\mu^2(1+1/\theta)$. Since the [variance](../../../../../../variance-split.md) is $G''(1)+G'(1)-G'(1)^2$, this proves

$$
\boxed{\mathbb E Y=\mu,\qquad\operatorname{Var}(Y)=\mu+\mu^2/\theta.}
$$

The extra positive term explains its [overdispersion](../../../../../../overdispersion.md) relative to a [Poisson distribution](../../../../../../poisson-distribution.md).

For one observation, write the [log-likelihood](../../../../../../log-likelihood.md) as

$$
\ell_y=\log\Gamma(\theta+y)-\log\Gamma(\theta)-\log(y!)+y\log\mu+\theta\log\theta-(\theta+y)\log(\mu+\theta).
$$

The mean [score function](../../../../../../informant-function.md) and its cross derivative are

$$
u_\mu=\frac{y}{\mu}-\frac{\theta+y}{\mu+\theta}=\frac{\theta(y-\mu)}{\mu(\mu+\theta)},\qquad \frac{\partial u_\mu}{\partial\theta}=\frac{y-\mu}{(\mu+\theta)^2}.
$$

Taking [expectations](../../../../../../expected-value.md) gives $I_{\mu\theta}=-\mathbb E(\partial_\theta u_\mu)=0$. In addition,

$$
I_{\mu\mu}=\frac{\theta}{\mu(\mu+\theta)}=\frac1{\mu+\mu^2/\theta}.
$$

For reference, with $\psi$ the [digamma function](../../../../../../digamma-function.md), the size [score function](../../../../../../informant-function.md) is

$$
u_\theta=\psi(\theta+y)-\psi(\theta)+\log\theta+1-\log(\mu+\theta)-\frac{\theta+y}{\mu+\theta}.
$$

Its [variance](../../../../../../variance-split.md) $I_{\theta\theta}$ is finite and positive for finite positive $\mu,\theta$. Thus [negative binomial mean-size parameter orthogonality](../../../../../../negative-binomial-mean-size-parameter-orthogonality.md) makes the expected [Fisher information matrix](../../../../../../fisher-information-matrix.md) diagonal. For an independent identically distributed sample and a regular identifiable interior true parameter, [asymptotic normality of a maximum likelihood estimator](../../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md) gives

$$
\sqrt n\begin{pmatrix}\widehat\mu-\mu\\\widehat\theta-\theta\end{pmatrix}\xrightarrow d N_2\left(0,\begin{pmatrix}\mu+\mu^2/\theta&0\\0&I_{\theta\theta}^{-1}\end{pmatrix}\right).
$$

Hence **the asymptotic correlation is zero**. This is first-order asymptotic independence, not a claim of exact finite-sample independence. Indeed the mean score yields $\widehat\mu=\bar y$ at an interior fit, while the size fit also depends on the observed dispersion. The argument excludes a true boundary such as the Poisson limit $\theta=\infty$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
