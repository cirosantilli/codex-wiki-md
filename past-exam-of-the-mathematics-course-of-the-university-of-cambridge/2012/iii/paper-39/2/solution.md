<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

At an interior [statistical parameter](../../../../../statistical-parameter.md) $\theta$, [local asymptotic normality](../../../../../local-asymptotic-normality.md) means that there are random vectors $\Delta_{n,\theta}$ and a symmetric nonnegative [Fisher information matrix](../../../../../fisher-information-matrix.md) $I_\theta$ such that, for each fixed $h\in\mathbb R^p$,

$$
\log\frac{\prod_{i=1}^n f(\theta+h/\sqrt n,Y_i)}{\prod_{i=1}^n f(\theta,Y_i)}
=h^T\Delta_{n,\theta}-\frac12h^TI_\theta h+o_{P_\theta^n}(1),
\qquad \Delta_{n,\theta}\xrightarrow{d}N_p(0,I_\theta).
$$

A common stronger definition requires this expansion also for $h_n\to h$. The fixed-$h$ version suffices here. A regular identifiable model usually has positive definite [Fisher information](../../../../../fisher-information-matrix.md); nonsingularity is unnecessary for the contiguity conclusion.

Here are sufficient differentiability conditions for a proof by [Taylor's theorem](../../../../../taylor-theorem.md). Suppose the local [probability density functions](../../../../../probability-density-function.md) have common support, $\ell_\vartheta(y)=\log f(\vartheta,y)$ is twice continuously differentiable near $\theta$, differentiation can pass through the normalization integral twice, the [score function](../../../../../informant-function.md) $s_\theta=\nabla\ell_\theta$ has finite second moment, and the local [Hessian matrix](../../../../../hessian-matrix.md) is bounded in [operator norm](../../../../../operator-norm.md) by an [integrable envelope of a function class](../../../../../integrable-envelope-of-a-function-class.md). These hypotheses imply

$$
\mathbb E_\theta s_\theta=0,\qquad
I_\theta=\mathbb E_\theta[s_\theta s_\theta^T]
=-\mathbb E_\theta\nabla^2\ell_\theta.
$$

The first identity differentiates $\int f_\theta=1$ once; the second uses $\nabla^2 f_\theta=f_\theta(\nabla^2\ell_\theta+s_\theta s_\theta^T)$ and differentiates twice. The [central limit theorem](../../../../../central-limit-theorem.md) gives $\Delta_{n,\theta}=n^{-1/2}\sum_i s_\theta(Y_i)\xrightarrow dN_p(0,I_\theta)$. Taylor's integral remainder gives

$$
\sum_i(\ell_{\theta+h/\sqrt n}(Y_i)-\ell_\theta(Y_i))
=h^T\Delta_{n,\theta}+
 h^T\!\left[\frac1n\sum_i\int_0^1(1-t)\nabla^2\ell_{\theta+th/\sqrt n}(Y_i)\,dt\right]h.
$$

The [weak law of large numbers](../../../../../weak-law-of-large-numbers.md) and the [continuity](../../../../../continuous-function.md) and integrable-envelope hypotheses make the bracket converge in probability to $-I_\theta/2$. Indeed, the [expectation](../../../../../expected-value.md) of the supremum of the [Hessian matrix](../../../../../hessian-matrix.md) difference over a shrinking neighborhood tends to zero by [dominated convergence](../../../../../dominated-convergence-theorem.md), and [Markov inequality](../../../../../markov-inequality.md) controls its empirical average. This proves [local asymptotic normality](../../../../../local-asymptotic-normality.md) and explains the role of both [derivatives](../../../../../derivative.md).

Write $Q_n\triangleleft P_n$ for [contiguity of probability measures](../../../../../contiguity-of-probability-measures.md): for every measurable sequence $A_n$, $P_n(A_n)\to0$ implies $Q_n(A_n)\to0$. [Mutual contiguity](../../../../../mutual-contiguity.md) requires this in both directions. A useful form of [Le Cam's first lemma](../../../../../le-cam-s-first-lemma.md) is the following: if the [Radon-Nikodym derivative](../../../../../radon-nikodym-derivative.md) $L_n$ of the absolutely continuous part of $Q_n$ relative to $P_n$ converges in distribution under $P_n$ to $L$, with $L>0$ almost surely and $\mathbb EL=1$, then the two sequences are [mutually contiguous](../../../../../mutual-contiguity.md). This includes the usual case $L_n=dQ_n/dP_n$. The mean-one condition ensures [uniform integrability](../../../../../uniform-integrability.md) of $L_n$ and vanishing mass of any singular part; positivity ensures the reverse implication.

Take $P_n=P_\theta^n$ and $Q_n=P_{\theta+h/\sqrt n}^n$. Their [likelihood ratio](../../../../../likelihood-ratio.md) on the support of $P_n$ satisfies, by [local asymptotic normality](../../../../../local-asymptotic-normality.md) and the [continuous mapping theorem](../../../../../continuous-mapping-theorem.md),

$$
L_n\xrightarrow d L=\exp(W-v/2),\qquad
W\sim N(0,v),\quad v=h^TI_\theta h.
$$

This limit is positive and $\mathbb EL=e^{-v/2}e^{v/2}=1$, including $v=0$. The conditions of [Le Cam's first lemma](../../../../../le-cam-s-first-lemma.md) therefore hold, giving **[mutual contiguity](../../../../../mutual-contiguity.md) of the product sampling laws**. The products, rather than the one-observation laws, are the relevant sequences.

For any $\varepsilon>0$, let $A_n=\{\|\widehat\theta_n-\theta\|>\varepsilon\}$. [Consistency](../../../../../consistency-statistics.md) under $P_\theta^n$ makes $P_\theta^n(A_n)\to0$, and [contiguity](../../../../../contiguity-of-probability-measures.md) gives $Q_n(A_n)\to0$. Thus **the [estimator](../../../../../estimator.md) remains consistent for $\theta$ under each fixed local alternative**. Since $\|\theta+h/\sqrt n-\theta\|\to0$, it is also consistent for the moving parameter in the sense that $\|\widehat\theta_n-(\theta+h/\sqrt n)\|\to0$ in probability under $Q_n$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
