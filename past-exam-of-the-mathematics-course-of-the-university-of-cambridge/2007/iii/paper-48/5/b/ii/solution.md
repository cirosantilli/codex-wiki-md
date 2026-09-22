<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The posterior kernel gives two gamma [full conditional distributions](../../../../../../../full-conditional-distribution.md) directly:

$$
\boxed{\lambda\mid\phi,m,x\sim\operatorname{Gamma}(\alpha+S_m,\beta+m),\qquad\phi\mid\lambda,m,x\sim\operatorname{Gamma}(\gamma+S-S_m,\delta+N-m),}
$$

with rates as the second parameters. For the index, terms independent of the proposed value $j$ cancel. Its conditional weights are

$$
\lambda^{S_j}\phi^{S-S_j}e^{-j\lambda-(N-j)\phi}\propto\exp\left[j(\phi-\lambda)+S_j\log\frac{\lambda}{\phi}\right].
$$

Define $\ell_j=j(\phi-\lambda)+S_j\log(\lambda/\phi)$ and $\ell_{\max}=\max_j\ell_j$. The normalized categorical probabilities are

$$
\boxed{P(m=j\mid\lambda,\phi,x)=\frac{e^{\ell_j-\ell_{\max}}}{\sum_{r=1}^Ne^{\ell_r-\ell_{\max}}}.}
$$

Subtracting the largest log weight prevents needless numerical overflow, an application of the [log-sum-exp function](../../../../../../../log-sum-exp-function.md).

Precompute the cumulative counts $S_j$. Initialize any $m\in\{1,\ldots,N\}$ and positive rates. At each iteration, draw $\lambda$ from its gamma conditional given the current index, draw $\phi$ from its gamma conditional given that index, and draw a new index from the categorical probabilities using the newly drawn rates. Repeat and retain the parameter triples after initialization effects have diminished. These are the [Gibbs updates for a Poisson count change point](../../../../../../../gibbs-updates-for-a-poisson-count-change-point.md).

To verify invariance rather than just identify a sampler, a coordinate update integrates the old joint density as $\pi(\lambda,\phi,m\mid x)=\pi(\lambda\mid\phi,m,x)\pi(\phi,m\mid x)$ and replaces the first factor by an independent draw from the same conditional. The joint [posterior distribution](../../../../../../../bayesian-posterior.md) is therefore unchanged. The same argument applies to the other two updates, so their composition preserves the posterior. All gamma densities and all categorical weights are positive on their supports. The full-sweep transition density is consequently positive across the joint support, giving the usual irreducibility and aperiodicity conditions for this proper-posterior [Gibbs sampler](../../../../../../../gibbs-sampler.md). This supports posterior long-run averages under the [ergodic theorem for a positive Harris recurrent Markov chain](../../../../../../../ergodic-theorem-for-a-positive-harris-recurrent-markov-chain.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 48](../../../../paper-48-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
