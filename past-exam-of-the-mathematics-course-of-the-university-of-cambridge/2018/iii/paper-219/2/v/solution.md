<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Let $\pi$ be the normalized density $\widetilde\pi$ in the transformed coordinates of (iv). Its fixed Gaussian increment gives a symmetric [proposal distribution](../../../../../../proposal-distribution.md): $q(\theta'\mid\theta)=q(\theta\mid\theta')$. For distinct states, the accepted transition density is $K(\theta,\theta')=q(\theta'\mid\theta)\alpha(\theta,\theta')$, where $\alpha=\min\{1,\pi(\theta')/\pi(\theta)\}$. Then

$$
\pi(\theta)K(\theta,\theta')=q(\theta'\mid\theta)\min\{\pi(\theta),\pi(\theta')\}=\pi(\theta')K(\theta',\theta).
$$

The rejection probability gives a mass on the diagonal, which trivially satisfies the same balance identity. Thus $\boxed{\pi(d\theta)K(\theta,d\theta')=\pi(d\theta')K(\theta',d\theta)}$, the [detailed balance](../../../../../../detailed-balance.md) condition, and integrating it proves invariance of the target.

The transformed density includes its Jacobian, so mapping back preserves the desired posterior law. Warmup adaptation is excluded from this fixed-kernel proof. Independent augmentation with $H_0$ is itself a reversible conditional update; alternatively the original joint augmented space can be sampled directly. This is the [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) balance argument.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
