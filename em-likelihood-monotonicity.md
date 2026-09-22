# EM likelihood monotonicity

↑ **Parent:** [Expectation-maximization algorithm](expectation-maximization-algorithm.md)

For $Q(\theta\mid\theta_0)=\mathbb E_{\theta_0}[\log p_\theta(Y,Z)\mid Y]$, the [Jensen inequality](jensen-s-inequality.md) gives

$$
\log p_\theta(Y)-\log p_{\theta_0}(Y)\geq Q(\theta\mid\theta_0)-Q(\theta_0\mid\theta_0).
$$

Thus any [expectation-maximization algorithm](expectation-maximization-algorithm.md) [M-step](em-maximization-step.md) that increases $Q$ cannot decrease the observed-data [likelihood function](likelihood-function.md).[Section 3, printed pp. 6-7, Lemma 1 and Theorem 1, especially equation (3.10)](maximum-likelihood-from-incomplete-data-via-the-em-algorithm-by-arthur-pentland-dempster-and-others.md)

For a short proof, assume common support and finite expressions, and keep the [E-step](em-expectation-step.md) [conditional distribution](conditional-distribution.md) $q_t(z)=p_{\theta^{(t)}}(z\mid y)$ fixed. The [concavity](concave-function.md) of the [logarithm](logarithm.md) and [Jensen's inequality](jensen-s-inequality.md) give

$$
\ell(\theta)=\log\mathbb E_{q_t}\left[\frac{p_\theta(y,Z)}{q_t(Z)}\right]\geq\mathbb E_{q_t}[\log p_\theta(y,Z)-\log q_t(Z)]=F(q_t,\theta).
$$

This [evidence lower bound](evidence-lower-bound.md) equals $Q(\theta\mid\theta^{(t)})-\mathbb E_{q_t}\log q_t(Z)$. At $\theta=\theta^{(t)}$, the ratio inside the [expectation](expected-value-split.md) is the constant $p_{\theta^{(t)}}(y)$, so equality holds. During the [M-step](em-maximization-step.md), the second term is constant; increasing $Q$ raises a lower bound that touches the current [log-likelihood](log-likelihood.md). Hence

$$
\ell(\theta^{(t+1)})\geq F(q_t,\theta^{(t+1)})\geq F(q_t,\theta^{(t)})=\ell(\theta^{(t)}).
$$

Increasing [likelihood](likelihood-function.md) values alone do not establish convergence of the [statistical parameters](statistical-parameter.md) or attainment of a global maximum. In a differentiable finite [mixture model](mixture-model.md), the [gradient](gradient.md) of $\ell$ equals the candidate-parameter [gradient](gradient.md) of $Q$ evaluated at the current fit. Thus an interior [fixed point](fixed-point.md) of an exact [M-step](em-maximization-step.md) is a [stationary point](stationary-point.md), which need not be a [local maximum](local-maximum.md); the [Identical-mean EM trap](identical-mean-em-trap.md) is an explicit counterexample. Small changes in [log-likelihood](log-likelihood.md) can also occur before the [means](expected-value-split.md) have settled, so inspecting both is useful.

## ↑ Ancestors (8)

1. [Expectation-maximization algorithm](expectation-maximization-algorithm.md)
2. [Latent variable](latent-variable-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (11)

- [EM for Gaussian mixtures with a common variance](em-for-gaussian-mixtures-with-a-common-variance.md)
- [Known-variance Gaussian mixture EM example](known-variance-gaussian-mixture-em-example.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/4/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/4/c/solution.md)
