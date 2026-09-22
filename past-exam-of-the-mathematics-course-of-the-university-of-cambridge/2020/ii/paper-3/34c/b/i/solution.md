<h1 id="34c/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [S-wave scattering](../../../../../../../s-wave-quantum-scattering.md), write the radial wavefunction as $R_0(r)=u(r)/r$. In the attractive shell $a<r\leq2a$, the hard-core boundary condition $u(a)=0$ gives

$$
u_{\mathrm{in}}(r)=A\sin[\kappa(r-a)],
\qquad
\kappa^2=k^2+\frac{2mV_0}{\hbar^2}.
$$

Outside the potential, choose

$$
u_{\mathrm{out}}(r)=B\sin(kr+\delta_0).
$$

Continuity of the logarithmic derivative at $r=2a$ yields

$$
\kappa\cot(\kappa a)
=k\cot(2ka+\delta_0).
$$

Put $C=\kappa\cot(\kappa a)$. The [tangent addition formula](../../../../../../../tangent-addition-formula.md) gives

$$
\tan(2ka+\delta_0)=\frac{k}{C},
$$

and solving for $\tan\delta_0$ gives

$$
\tan\delta_0
=\frac{k-C\tan(2ka)}{C+k\tan(2ka)}
=\boxed{
\frac{k\cos(2ka)-\kappa\cot(\kappa a)\sin(2ka)}
{k\sin(2ka)+\kappa\cot(\kappa a)\cos(2ka)}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [34C](../../../34c.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
