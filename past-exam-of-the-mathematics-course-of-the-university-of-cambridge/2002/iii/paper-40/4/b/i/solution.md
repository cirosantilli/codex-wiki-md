<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For observed data $x$ and [latent variables](../../../../../../../latent-variable.md) $Z$, let $\ell_c(\theta;x,Z)=\log p_\theta(x,Z)$ be the complete-data [log-likelihood](../../../../../../../log-likelihood.md). From a current parameter $\theta^{(m)}$, the [expectation-maximization algorithm](../../../../../../../expectation-maximization-algorithm.md) computes

$$
Q(\theta\mid\theta^{(m)})=\mathbb E_{\theta^{(m)}}[\ell_c(\theta;x,Z)\mid x]
$$

and then chooses $\theta^{(m+1)}$ maximizing this function in its first argument. Thus the E-step averages the missing information conditional on the current model and observed data; the M-step treats those expectations as fixed while maximizing.

For a short proof of [likelihood function](../../../../../../../likelihood-function.md) monotonicity, let $q_m(Z)=p_{\theta^{(m)}}(Z\mid x)$. Then

$$
\frac{p_\theta(x)}{p_{\theta^{(m)}}(x)}=\mathbb E_{q_m}\frac{p_\theta(x,Z)}{p_{\theta^{(m)}}(x,Z)}.
$$

The [Jensen inequality](../../../../../../../jensen-s-inequality.md) for the logarithm gives $\ell(\theta;x)-\ell(\theta^{(m)};x)\geq Q(\theta\mid\theta^{(m)})-Q(\theta^{(m)}\mid\theta^{(m)})$. The M-step makes the right side nonnegative. Thus observed [likelihood function](../../../../../../../likelihood-function.md) cannot decrease. This proves the usual [EM likelihood monotonicity](../../../../../../../em-likelihood-monotonicity.md), while allowing convergence to local stationary points rather than guaranteeing a global maximum.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
