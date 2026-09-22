<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\Psi=-\Phi=GM(r^p+a^p)^{-1/p}$. The spherical [Poisson equation](../../../../../../poisson-equation.md) gives the [hypervirial model](../../../../../../hypervirial-model.md) density

$$
\boxed{
\rho(r)=\frac{(p+1)Ma^p}{4\pi}
\frac{r^{p-2}}{(r^p+a^p)^{2+1/p}}}
=\frac{(p+1)Ma^p}{4\pi(GM)^{2p+1}}
r^{p-2}\Psi^{2p+1}.
$$

For the proposed [hypervirial distribution function](../../../../../../hypervirial-distribution-function.md), write $\mathcal E=-E=\Psi-v^2/2$ and $n=(3p+1)/2$. Direct velocity integration gives

$$
\begin{aligned}
\rho
&=A r^{p-2}
\int_0^{\sqrt{2\Psi}}v^p
(\Psi-v^2/2)^n\,dv
\int_0^{2\pi}d\varphi
\int_0^\pi\sin^{p-1}\alpha\,d\alpha\\
&=A\,2^{(p+1)/2}\pi^{3/2}
\frac{\Gamma(p/2)\Gamma(3(p+1)/2)}
{\Gamma(2p+2)}
r^{p-2}\Psi^{2p+1}.
\end{aligned}
$$

Matching this expression to the density fixes

$$
\boxed{
A=\frac{(p+1)a^p\Gamma(2p+2)}
{2^{(p+5)/2}\pi^{5/2}G^{2p+1}M^{2p}
\Gamma(p/2)\Gamma(3(p+1)/2)}}.
$$

This coefficient is positive for $0<p\leq2$, so the distribution function self-consistently generates the stated density and potential.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
