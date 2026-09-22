<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Insert a [Fourier mode](../../../../../../fourier-mode.md) $U_m^n=G^ne^{im\theta}$. With $r=1-2\mu$ and $\eta=e^{i\theta}$, the [amplification polynomial](../../../../../../amplification-polynomial-of-a-multistep-method.md) is

$$
G^2-r(1-\eta)G-\eta=0.
$$

Its two roots have product $-\eta$, of modulus one. Thus if both roots are bounded by one, both must have modulus exactly one. Set $G=e^{i\theta/2}\lambda$. The equation becomes

$$
\lambda^2+2ir\sin(\theta/2)\lambda-1=0,
\qquad
\lambda_\pm=-ir\sin(\theta/2)\pm\sqrt{1-r^2\sin^2(\theta/2)}.
$$

When $|r|<1$, both roots have modulus one and their separation obeys $|G_+-G_-|\geq2\sqrt{1-r^2}>0$ for every frequency. The companion [matrix](../../../../../../matrix.md) has bounded entries and can be diagonalized with the two [eigenvectors](../../../../../../eigenvector.md) $(G_+,1)^T,(G_-,1)^T$. The uniform separation bounds the inverse [eigenvector](../../../../../../eigenvector.md) [matrix](../../../../../../matrix.md). Hence every [matrix](../../../../../../matrix.md) power is bounded uniformly in $n$ and $\theta$, and the [Parseval identity](../../../../../../parseval-identity.md) proves [L2 norm](../../../../../../l2-norm.md) [stability](../../../../../../stability-of-a-numerical-method.md) for the two starting levels on the whole grid.

If $|r|>1$, frequencies near $\theta=\pi$ give one root outside the unit circle, so the scheme is unstable. If $|r|=1$, the Nyquist [polynomial](../../../../../../polynomial-split.md) is $(G-r)^2$, a repeated unit root. The corresponding companion [matrix](../../../../../../matrix.md) has a nontrivial [Jordan block](../../../../../../jordan-block.md) and solutions containing $nr^n$. Thus the endpoints are unstable as well. On the whole line the individual Nyquist plane wave is not square-summable, but Fourier packets localized arbitrarily close to that frequency realize the unbounded power norm by continuity. Therefore the [uniform stability of a shifted two-level advection scheme](../../../../../../uniform-stability-of-a-shifted-two-level-advection-scheme.md) criterion is

$$
\boxed{0<\mu<1.}
$$

In particular $\mu=1/2$ is stably exact with compatible starts, whereas $\mu=1$ is formally exact but unstable under arbitrary perturbations. Checking only the moduli of the roots and retaining both endpoints would miss this essential distinction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
