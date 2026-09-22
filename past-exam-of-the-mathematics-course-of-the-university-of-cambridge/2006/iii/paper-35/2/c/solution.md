<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $A_t=\int_0^tH_s^2ds$ and its inverse $\tau_u$ as above. Strict increase and continuity make $u\mapsto\tau_u$ continuous, with $A_{\tau_u}=u$ and $\tau_{A_t}=t$. Thus $W_u=M_{\tau_u}$ is continuous and [adapted](../../../../../../adapted-process.md) to $\mathcal G_u=\mathcal F_{\tau_u}$, with $W_0=0$.

The essential remaining point is independence of increments, which does not follow merely from the [Gaussian](../../../../../../normal-distribution.md) marginal in part (a). Fix $0\le u<v$ and $\lambda\in\mathbb R$. The complex exponential

$$
\exp\left(i\lambda M_{t\wedge\tau_v}
+\frac{\lambda^2}{2}A_{t\wedge\tau_v}\right)
$$

is bounded by $e^{\lambda^2v/2}$ in modulus, hence is a [uniformly integrable](../../../../../../uniform-integrability.md) [martingale](../../../../../../martingale-split.md). The [optional sampling theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) at the finite, possibly unbounded, times $\tau_u\le\tau_v$ gives

$$
\mathbb E\left[e^{i\lambda M_{\tau_v}+\lambda^2v/2}\mid\mathcal F_{\tau_u}\right]
=e^{i\lambda M_{\tau_u}+\lambda^2u/2}.
$$

Divide by the nonzero right-hand exponential. Then

$$
\boxed{\mathbb E[e^{i\lambda(W_v-W_u)}\mid\mathcal G_u]
=e^{-\lambda^2(v-u)/2}.}
$$

This deterministic [conditional characteristic function](../../../../../../conditional-characteristic-function.md) says that $W_v-W_u$ is $N(0,v-u)$ and independent of $\mathcal G_u$. Successively conditioning proves independence of every finite family of increments. Together with continuity and the zero initial value, this proves that $W$ is [Brownian motion](../../../../../../brownian-motion-split.md). The inverse-clock identity gives $W_{A_t}=M_{\tau_{A_t}}=M_t$, completing the requested special-case proof of the [Dubins-Schwarz theorem](../../../../../../dambis-dubins-schwarz-theorem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
