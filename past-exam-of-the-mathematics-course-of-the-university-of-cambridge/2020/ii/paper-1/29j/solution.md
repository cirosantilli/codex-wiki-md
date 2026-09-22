<h1 id="29j/solution">Solution</h1>

↑ **Parent:** [29J](../29j.md)

Let $X$ have regular density $p_\theta$, let

$$
S_\theta(X)=\frac{\partial}{\partial\theta}\log p_\theta(X)
$$

be its [score function](../../../../../informant-function.md), and let

$$
I(\theta)=\mathbb E_\theta[S_\theta(X)^2]
$$

be its [Fisher information](../../../../../fisher-information-matrix.md). Regularity gives the [mean-zero score identity](../../../../../mean-zero-score-identity.md) $\mathbb E_\theta S_\theta=0$.

Suppose an estimator $T$ has mean $\mathbb E_\theta T=\psi(\theta)$. Differentiating under the integral gives

$$
\psi'(\theta)
=\mathbb E_\theta[T S_\theta]
=\operatorname{Cov}_\theta(T,S_\theta).
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) therefore yields

$$
\psi'(\theta)^2
\le\operatorname{Var}_\theta(T)\,I(\theta),
$$

and hence the [Cramér-Rao bound](../../../../../cramer-rao-bound.md)

$$
\boxed{\operatorname{Var}_\theta(T)
\ge\frac{\psi'(\theta)^2}{I(\theta)}}.
$$

In particular, an unbiased estimator of $\theta$ has variance at least $1/I(\theta)$. For an independent sample, the information is the sum of the individual informations.

In a decision problem with [risk of a decision rule](../../../../../risk-of-a-decision-rule.md) $R(\theta,\delta)$, a rule $\delta^*$ is [minimax](../../../../../minimax-decision-rule.md) when

$$
\boxed{
\sup_{\theta\in\Theta}R(\theta,\delta^*)
=\inf_\delta\sup_{\theta\in\Theta}R(\theta,\delta).
}
$$

Now let $X_1,\ldots,X_n$ be independent $N(\theta,1)$ variables with $\theta\ge0$, under [squared-error loss](../../../../../squared-error-loss.md). The [sample mean](../../../../../sample-mean.md) is unbiased with variance $1/n$, so

$$
R(\theta,\overline X_n)
=\mathbb E_\theta(\overline X_n-\theta)^2
=\frac1n
$$

for every $\theta\ge0$. Thus the minimax value is at most $1/n$.

For the matching lower bound, choose a continuously differentiable density $\pi$ on $(0,1)$ that vanishes at both endpoints and has finite prior information

$$
J=\int_0^1\frac{\pi'(u)^2}{\pi(u)}\,du;
$$

for example, $\pi(u)=30u^2(1-u)^2$. For $L>0$, define the prior

$$
\pi_L(\theta)=\frac1L\pi(\theta/L),
\qquad 0<\theta<L.
$$

It is supported inside the parameter space, and its information is $J/L^2$.

Here the likelihood score is

$$
S_\theta(X)=\sum_{i=1}^n(X_i-\theta),
$$

whose Fisher information is $n$. For any decision rule $\delta(X)$, combine it with the prior score to form the joint score

$$
U=S_\theta(X)+\frac{\pi_L'(\theta)}{\pi_L(\theta)}.
$$

Integration by parts in $\theta$, with no boundary term because $\pi_L$ vanishes there, gives

$$
\mathbb E_{\pi_L}\bigl[(\delta(X)-\theta)U\bigr]=1.
$$

The likelihood score has conditional mean zero, so its cross term with the prior score vanishes and

$$
\mathbb E_{\pi_L}U^2=n+\frac{J}{L^2}.
$$

Cauchy--Schwarz now proves the [Van Trees inequality](../../../../../van-trees-inequality.md) in this case:

$$
\int_0^L R(\theta,\delta)\pi_L(\theta)\,d\theta
\ge\frac1{n+J/L^2}.
$$

The worst-case risk dominates every integrated risk, and therefore

$$
\sup_{\theta\ge0}R(\theta,\delta)
\ge\frac1{n+J/L^2}.
$$

Letting $L\to\infty$ shows that every rule has worst-case risk at least $1/n$. Since $\overline X_n$ attains that value, the result on the [minimax sample mean for a nonnegative normal location](../../../../../minimax-sample-mean-for-a-nonnegative-normal-location.md) is

$$
\boxed{\overline X_n\text{ is minimax on }[0,\infty)}.
$$

## ↑ Ancestors (10)

1. [29J](../29j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
