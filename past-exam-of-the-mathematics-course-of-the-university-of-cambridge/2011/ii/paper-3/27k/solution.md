<h1 id="27k/solution">Solution</h1>

↑ **Parent:** [27K](../27k.md)

Given the complete stopped sample $(x_1,\ldots,x_n)$, the [likelihood function](../../../../../likelihood-function.md) is

$$
L(\theta;\mathbf x)=\theta^ne^{-\theta S}\alpha(x_n)\prod_{i=1}^{n-1}[1-\alpha(x_i)],\qquad S=\sum_{i=1}^nx_i.
$$

The stopping factor is positive and independent of $\theta$. The [Fisher-Neyman factorization theorem](../../../../../fisher-neyman-factorization-theorem.md) makes $(N,S)$ sufficient. For two possible stopped samples of lengths $n,m$ and sums $S,S'$, their likelihood ratio is a parameter-free factor times $\theta^{n-m}e^{-\theta(S-S')}$. This is independent of $\theta$ exactly when $n=m$ and $S=S'$: differentiating its logarithm gives $(n-m)/\theta-(S-S')=0$ for all $\theta>0$. By the likelihood-ratio criterion,

$$
\boxed{(N,\sum_{i=1}^NX_i)\text{ is a minimal sufficient statistic}.}
$$

The [likelihood principle](../../../../../likelihood-principle.md) says proportional likelihoods give the same evidence about the parameter. Thus with the full sample observed, this parameter-free stopping rule adds no likelihood evidence beyond the realized values and length; it gives the same likelihood-based inference as a fixed-length sample with those values. This statement does not assert that frequentist sampling distributions are unchanged.

Let $q(\theta)=\int_0^\infty\alpha(x)\theta e^{-\theta x}\,dx\in(0,1)$ be the chance of stopping at a given stage. Independence of successive stages gives

$$
p_Y(y\mid\theta)=\sum_{n\geq1}(1-q(\theta))^{n-1}\alpha(y)\theta e^{-\theta y}=\frac{\alpha(y)e^{-\theta y}}{\int_0^\infty\alpha(x)e^{-\theta x}\,dx}.
$$

Therefore $a(y)=\log\alpha(y)$ and $k(\theta)=\log\int_0^\infty e^{a(y)-\theta y}\,dy$ give the requested [exponential family](../../../../../exponential-family-split.md) form.

Writing $p=p_Y$, differentiation in $y$ gives $p'=(a'-\theta)p$. Integrating and using $p(0)=p(\infty)=0$ shows $\mathbb E_\theta a'(Y)=\theta$. Likewise

$$
p''=[a''+(a'-\theta)^2]p.
$$

The stipulated vanishing of $p'$ at both boundaries gives

$$
\boxed{\operatorname{Var}_\theta(a'(Y))=-\mathbb E_\theta a''(Y).}
$$

These integrations require the displayed moments and integrals to exist, the usual regularity interpretation of the question; when establishing a finite variance this assumption should be explicit.

Differentiating the normalization in $\theta$ gives $k'(\theta)=-\mathbb E_\theta Y$ and $k''(\theta)=\operatorname{Var}_\theta Y$. The [score function](../../../../../informant-function.md) is $-k'(\theta)-Y$, so the [Fisher information](../../../../../fisher-information-matrix.md) is $I(\theta)=k''(\theta)$. The [Cramér-Rao bound](../../../../../cramer-rao-bound.md) states that a regular unbiased estimator of $\theta$ has variance at least $1/I(\theta)$. Apply it to $a'(Y)$:

$$
\boxed{-k''(\theta)\,\mathbb E_\theta a''(Y)\geq1.}
$$

Equivalently differentiate $\mathbb E_\theta a'(Y)=\theta$ and use the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) to get $1\leq\sqrt{\operatorname{Var}(a'(Y))\operatorname{Var}(Y)}$, which gives the same conclusion.

## ↑ Ancestors (10)

1. [27K](../27k.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
