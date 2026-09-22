<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The distributional identity $\partial_{\bar z}(1/(\pi z))=\delta$ gives the [Cauchy-Green operator](../../../../../../cauchy-green-operator.md) solution

$$
\boxed{\mu(z,\lambda)=\frac1{\pi\nu(r)}\int_{\mathbb C}\frac{\widetilde f(z')}{z-z'}d^2z',}
$$

where $\widetilde f$ is $f$ in the changed real coordinates. The singularity $1/(z-z')$ is locally integrable. For [Schwartz functions](../../../../../../schwartz-function.md), splitting the integral into a region near the origin and a rapidly decaying far region proves $\mu=O(|z|^{-1})$. If two solutions obey this decay, their difference has zero [Wirtinger derivative](../../../../../../wirtinger-derivatives.md) and is an entire [holomorphic function](../../../../../../holomorphic-function.md) tending to zero; the [Liouville theorem](../../../../../../liouville-theorem.md) proves uniqueness.

The change-of-variables Jacobian has absolute value $a_r/|b_r|$. Therefore an equivalent form of the [complexified transport Cauchy kernel](../../../../../../complexified-transport-cauchy-kernel.md) is

$$
\mu=\frac{i\,\operatorname{sgn}b_r}{2\pi}\int_{\mathbb R^2}
\frac{F(\tau',\rho',\theta)}{a_r(\rho-\rho')+ib_r(\tau-\tau')}d\tau'd\rho'.
$$

In the original complex coordinate $w=x_1+ix_2$, it is

$$
\mu(w,\lambda)=\frac{\operatorname{sgn}(|\lambda|-1)}\pi\int_{\mathbb R^2}
\frac{f(w')}{\lambda(\bar w-\bar w')-\lambda^{-1}(w-w')}d^2w'.
$$

For $|\lambda|<1$ the denominator can be rewritten to give the kernel $\lambda/[\pi((w-w')-\lambda^2(\bar w-\bar w'))]$. For $|\lambda|>1$ it is $\lambda^{-1}/[\pi((\bar w-\bar w')-\lambda^{-2}(w-w'))]$. Consequently the spectral solution is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) separately inside and outside the unit circle, with $\mu=O(\lambda)$ at zero and $\mu=O(\lambda^{-1})$ at infinity. These normalizations will determine its jump reconstruction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
