<h1 id="1/1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Put $A_t=\int_0^tH_s^2ds$. It is continuous and tends to infinity almost surely, so $A_{T_\sigma}=\sigma^2$. Define the right-continuous inverse $T(u)=\inf\{t:A_t>u\}$ and

$$
W_u=\int_0^{T(u)}H_s\,dB_s.
$$

The time-change theorem for local martingales shows that $W$ is a continuous local martingale in the time-changed filtration, and

$$
\langle W\rangle_u=A_{T(u)}=u.
$$

For completeness, this proves the required case of the [Dambis-Dubins-Schwarz theorem](../../../../../../../dambis-dubins-schwarz-theorem.md): for every $\theta\in\mathbb R$, [Itô formula](../../../../../../../ito-s-lemma.md) makes $\exp(i\theta W_u+\theta^2u/2)$ a local martingale; stopping and conditioning show that $W_v-W_u$ has conditional characteristic function $e^{-\theta^2(v-u)/2}$. Hence the increments are independent centered normal variables with the Brownian variances, and continuity makes $W$ a [Brownian motion](../../../../../../../brownian-motion-split.md). Consequently

$$
X_\sigma=W_{\sigma^2}\sim N(0,\sigma^2).
$$

Thus **$X_\sigma$ is centered Gaussian with variance $\sigma^2$**.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
