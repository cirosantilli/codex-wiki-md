<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the forward field is sufficiently differentiable in maturity to differentiate its deterministic and [stochastic integrals](../../../../../../stochastic-integral.md). Moving along the diagonal adds the maturity derivative to the fixed-maturity dynamics:

$$
\boxed{dr_t=\left[\left.\partial_Tf(t,T)\right|_{T=t}+\alpha_Q(t,t)\right]dt+\sigma(t,t)dW_t^Q.}
$$

The [Heath-Jarrow-Morton model](../../../../../../heath-jarrow-morton-model.md) no-arbitrage drift is $\alpha_Q(t,T)=\sigma(t,T)\int_t^T\sigma(t,u)du$, so $\alpha_Q(t,t)=0$. Equivalently, from the integrated forward equation,

$$
\left.\partial_Tf(t,T)\right|_{T=t}
=f_0'(t)+\int_0^t\partial_T\alpha_Q(s,t)ds+\int_0^t\partial_T\sigma(s,t)dW_s^Q.
$$

That drift can depend on the entire previous forward curve or driving path, rather than on the current scalar rate.

**The [short rate](../../../../../../short-rate.md) need not be [Markov](../../../../../../markov-property.md).** For a concrete [One Brownian factor does not imply a Markov short rate](../../../../../../one-brownian-factor-does-not-imply-a-markov-short-rate.md) example, take the deterministic volatility $\sigma(t,T)=T-t$. Its admissible risk-neutral drift is $(T-t)^3/2$, and

$$
r_t=f_0(t)+\frac{t^4}{8}+\int_0^t(t-s)dW_s
=f_0(t)+\frac{t^4}{8}+\int_0^tW_sds.
$$

Subtracting the deterministic part leaves $I_t=\int_0^tW_sds$. The past of $I$ reveals its derivative $W_t$, and $\mathbb E[I_{t+h}-I_t\mid\mathcal F_t^I]=hW_t$. Yet $W_t$ is not determined by $I_t$: the [Gaussian](../../../../../../normal-distribution.md) covariance calculation gives

$$
\operatorname{Var}I_t=t^3/3,\qquad \operatorname{Cov}(W_t,I_t)=t^2/2,\qquad
\operatorname{Var}(W_t\mid I_t)=t/4>0.
$$

Consequently the conditional law of the future depends on more than $I_t$, proving failure of the [Markov property](../../../../../../markov-property.md) for the scalar [short rate](../../../../../../short-rate.md). The enlarged pair $(I_t,W_t)$ is [Markov](../../../../../../markov-property.md). Special maturity-volatility structures, such as those producing a Vasicek-type short-rate diffusion, can instead admit a scalar [Markov](../../../../../../markov-property.md) realization.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
