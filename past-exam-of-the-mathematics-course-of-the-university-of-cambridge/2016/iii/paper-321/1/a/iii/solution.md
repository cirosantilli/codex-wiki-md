<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the finite-mass [similarity solution](../../../../../../../similarity-solution.md) above, the total disk [mass](../../../../../../../mass.md) is

$$
M_d=2\pi\Sigma_0r_0^2 C\int_0^\infty x^{-3/2}e^{-1/(\tau\sqrt x)}\,dx.
$$

Substitute $\xi=1/(\tau\sqrt x)$, so $x=\tau^{-2}\xi^{-2}$ and $x^{-3/2}|dx|=2\tau\,d\xi$. This gives

$$
\boxed{M_d=4\pi C\Sigma_0r_0^2\tau=M_d(0)+3\pi C\bar\nu_0\Sigma_0t.}
$$

The requested linear increase of [mass](../../../../../../../mass.md) is therefore correct. It is supplied by the infinite-radius boundary, rather than by a source-free isolated finite disk. The inward [mass accretion rate](../../../../../../../mass-accretion-rate.md) is

$$
\dot M(r)=6\pi r^{1/2}\partial_r(r^{1/2}\bar\nu\Sigma)=3\pi C\bar\nu_0\Sigma_0(1+\xi)e^{-\xi},
$$

which tends to zero at the origin and to $3\pi C\bar\nu_0\Sigma_0$ at infinity.

For [Keplerian rotation](../../../../../../../keplerian-disk.md), the [specific angular momentum](../../../../../../../specific-angular-momentum.md) is $\ell=\sqrt{GM_\star r}$. The total disk [angular momentum](../../../../../../../angular-momentum.md) would be

$$
J_d=2\pi C\Sigma_0\sqrt{GM_\star}\,r_0^{5/2}\int_0^\infty x^{-1}e^{-1/(\tau\sqrt x)}\,dx
=4\pi C\Sigma_0\sqrt{GM_\star}\,r_0^{5/2}\int_0^\infty\frac{e^{-\xi}}\xi\,d\xi.
$$

**This integral diverges at $\xi=0$, corresponding to infinite radius. There is no finite constant total angular momentum for the nonzero printed similarity solution.** The seemingly time-independent last expression is an infinite quantity; it cannot prove a finite [conservation law](../../../../../../../conservation-law.md).

The problem remains visible under a cutoff. With $r\le r_0R$, write $J_R=J_*E_1(1/(\tau\sqrt R))$, where $J_*=4\pi C\Sigma_0\sqrt{GM_\star}\,r_0^{5/2}$ and $E_1$ is the [exponential integral](../../../../../../../exponential-integral.md). Then

$$
\frac{dJ_R}{d\tau}=\frac{J_*}{\tau}e^{-1/(\tau\sqrt R)}>0,\qquad \lim_{R\to\infty}[J_R(\tau)-J_R(1)]=J_*\log\tau.
$$

Even the finite change after subtracting a common logarithmic divergence is not zero. Direct integration of the disk [diffusion equation](../../../../../../../diffusion-equation-split.md) gives the boundary identity

$$
\frac{dJ_d}{dt}=6\pi\sqrt{GM_\star}\left[r^{3/2}\partial_r(\bar\nu\Sigma)\right]_0^\infty;
$$

for this profile the outer expression has a nonzero limit, giving the same finite change rate. An inner zero torque alone does not impose zero outer [angular-momentum flux](../../../../../../../angular-momentum-flux.md).

More generally, the printed family $A+B e^{-\xi}$ can have finite [angular momentum](../../../../../../../angular-momentum.md) at both ends only if $A=0$ and $A+B=0$, hence it is trivial. Thus the request for a nonzero finite constant $J_d$ is incompatible with the stated viscosity exponent, similarity ansatz and infinite radial domain. A physical finite-domain or altered similarity problem would need different boundary data or assumptions; silently assigning a finite value to the divergent integral does not repair it.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 321](../../../../paper-321-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
