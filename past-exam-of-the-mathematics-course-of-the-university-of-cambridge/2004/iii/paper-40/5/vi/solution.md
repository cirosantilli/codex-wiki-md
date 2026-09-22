<h1 id="5/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Under the reference convention $\alpha_1=0$, the hypothesis becomes absence of the free group contrast $\alpha_2$. Introduce an inclusion indicator $J$: set $\alpha_2=0$ when $J=0$, and use its stated proper normal prior when $J=1$. Assign positive prior [probabilities](../../../../../../probability.md) $q_0,q_1$ to those models, and retain $\mu,\beta_2$ in both.

A birth draws $u$ from a proposal [probability density function](../../../../../../probability-density-function.md) $g(u)$ and appends it as $\alpha_2'=u$; the reverse death deletes it. The Jacobian is one. At fixed $\theta,\beta_2$, the [likelihood](../../../../../../likelihood-function.md) ratio is

$$
\frac{L(\alpha_2=u)}{L(\alpha_2=0)}
=\exp\{Ru-I\theta(1+e^{\beta_2})(e^u-1)\}.
$$

Thus the birth acceptance ratio before capping is

$$
\frac{q_1p_\alpha(u)d_1}{q_0b_0g(u)}
\exp\{Ru-I\theta(1+e^{\beta_2})(e^u-1)\},
$$

where $p_\alpha$ is the normalized $N(0,\sigma_1^2)$ prior. Again, taking $g=p_\alpha$ cancels that factor. Use the reciprocal death rule and ordinary within-model parameter updates.

After warm-up, the [Markov chain Monte Carlo](../../../../../../markov-chain-monte-carlo.md) occupation fraction estimates the desired [probability](../../../../../../probability.md):

$$
\boxed{\mathbb P(\alpha_1=\alpha_2=0\mid\mathbf x)
\approx\frac1N\sum_{s=1}^N\mathbf1_{\{J^{(s)}=0\}}.}
$$

This requires the chain to explore both models and satisfy its usual ergodic convergence conditions. Under the original continuous normal prior alone, the equality event has posterior [probability](../../../../../../probability.md) zero; the explicit model indicator supplies the necessary prior atom. If intercept selection from part (v) is also performed, use two indicators and count all sampled states with $J=0$, regardless of the intercept indicator.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
