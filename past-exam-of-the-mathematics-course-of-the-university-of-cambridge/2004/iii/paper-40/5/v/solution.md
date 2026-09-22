<h1 id="5/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Introduce a model indicator $M\in\{0,1\}$. In $M=0$, set $\mu=0$, hence $\theta=1$, and retain the two group effects. In $M=1$, include $\mu$ with the prior induced by the gamma baseline. Choose positive prior model [probabilities](../../../../../../probability.md) $p_0,p_1$ summing to one; the supplied within-model parameter priors alone do not specify these [probabilities](../../../../../../probability.md).

Let $r=(a_2,b_2)$, use the same proper prior $p(r)$ in both models, and denote their likelihoods by $L_0(r)$ and $L_1(\mu,r)$. The unnormalized joint model targets are

$$
t_0(r)=p_0p(r)L_0(r),\qquad
t_1(\mu,r)=p_1p(r)p_\mu(\mu)L_1(\mu,r),
\qquad
p_\mu(u)=\frac{b^a}{\Gamma(a)}e^{au-be^u}.
$$

For a birth move, draw an auxiliary $u$ from a positive [probability density function](../../../../../../probability-density-function.md) $q(u)$ and map $(r,u)$ to $(\mu'=u,r'=r)$. The reverse death move simply deletes $\mu$. This is a dimension-matching bijection with absolute Jacobian one. If the birth and death selection [probabilities](../../../../../../probability.md) are $b_0$ and $d_1$, respectively, the [birth and death moves for Bayesian variable selection](../../../../../../birth-and-death-moves-for-bayesian-variable-selection.md) rule gives

$$
\boxed{A_{0\to1}=\min\!\left(1,
\frac{p_1p_\mu(u)L_1(u,r)d_1}{p_0L_0(r)b_0q(u)}\right).}
$$

The reverse acceptance is the reciprocal ratio, capped at one, evaluated at the current $\mu$. Choosing $q=p_\mu$ cancels the added-parameter prior; a data-informed proposal may mix better but must retain its proposal factor. Within each model, also update its continuous parameters to ensure exploration.

For an explicit [likelihood](../../../../../../likelihood-function.md) ratio, with $E$ and $T$ from part (ii),

$$
\frac{L_1(u,r)}{L_0(r)}=\exp\{Tu-(e^u-1)E\}.
$$

This supplies a complete [reversible-jump Markov chain Monte Carlo](../../../../../../reversible-jump-markov-chain-monte-carlo.md) move. Its acceptance [probabilities](../../../../../../probability.md) enforce [detailed balance](../../../../../../detailed-balance.md) between the two dimensions. The lower-dimensional state is a separate point-mass model, not a zero-probability equality test inside the continuous full-model prior.

## ↑ Ancestors (11)

1. [V](../v.md)
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
