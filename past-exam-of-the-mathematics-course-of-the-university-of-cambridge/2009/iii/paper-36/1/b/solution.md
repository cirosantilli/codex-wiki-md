<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the $m$ independent [Bernoulli trials](../../../../../../bernoulli-trial.md), the log [likelihood function](../../../../../../likelihood-function.md), apart from its constant, is $\ell(\theta)=x\log\theta+(m-x)\log(1-\theta)$. Its negative expected second derivative, the [Fisher information](../../../../../../fisher-information-matrix.md), is

$$
I_m(\theta)=\frac{\mathbb E[X]}{\theta^2}+\frac{m-\mathbb E[X]}{(1-\theta)^2}
=\frac{m}{\theta(1-\theta)}.
$$

For $m>0$, the [Jeffreys prior](../../../../../../jeffreys-prior.md) is proportional to its square root. Since $\mathrm B(1/2,1/2)=\pi$, its normalized form is

$$
\boxed{\pi_J(\theta)=\frac1{\pi\sqrt{\theta(1-\theta)}},\qquad
\theta\sim\operatorname{Beta}(1/2,1/2).}
$$

The [Jeffreys prior](../../../../../../jeffreys-prior.md) is invariant under smooth one-to-one reparameterization as a measure. If $\phi=h(\theta)$, then $I_\phi(\phi)=I_\theta(\theta)(d\theta/d\phi)^2$, so $\sqrt{I_\phi}\,d\phi=\sqrt{I_\theta}\,|d\theta|$. Thus recomputing it in the new coordinate gives precisely the transformed prior, rather than a new prior. In several dimensions the corresponding density is $\sqrt{\det I(\theta)}$, with the same Jacobian transformation property.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
