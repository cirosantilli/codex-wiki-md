<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $k_a=k$ ahead of the front and $k_b=k+\Delta k$ behind. With viscosity $\mu$, [Darcy's law](../../../../../../darcy-law.md) gives the planar pressure gradients $p_{a0}'=-\mu U/k_a$ and $p_{b0}'=-\mu U/k_b$. Write the displacement as $\eta e^{\sigma t+i\alpha y}$ with $\alpha>0$, and take the unperturbed interface to be $x=0$ in its translating frame.

The liquid flux is divergence-free away from the interface, so the pressure perturbations are [harmonic](../../../../../../harmonic-function.md). The decaying [normal modes](../../../../../../normal-mode.md) are

$$
\delta p_b=B e^{\alpha x}e^{\sigma t+i\alpha y},\qquad \delta p_a=A e^{-\alpha x}e^{\sigma t+i\alpha y}.
$$

Expanding [pressure continuity](../../../../../../pressure-continuity.md) at the displaced interface and matching normal [Darcy flux](../../../../../../darcy-velocity.md) gives

$$
B-A=\mu U\left(\frac1{k_b}-\frac1{k_a}\right)\eta=-\frac{\mu U\Delta k}{k_ak_b}\eta,\qquad -k_bB=k_aA.
$$

Hence

$$
B=-\frac{\mu U\Delta k}{k_b(k_a+k_b)}\eta,\qquad A=\frac{\mu U\Delta k}{k_a(k_a+k_b)}\eta.
$$

The common normal-flux perturbation is $\delta u_n=-k_b\alpha B/\mu=\alpha U\Delta k\,\eta/(k_a+k_b)$. The local [enthalpy](../../../../../../enthalpy.md) balance converts it into a front-speed perturbation, $\sigma\eta=\delta u_n/(1+S\Delta\phi)$. Thus the [melting-front instability due to permeability contrast](../../../../../../melting-front-instability-due-to-permeability-contrast.md) has

$$
\boxed{\sigma=\frac{\alpha U}{1+S\Delta\phi}\frac{\Delta k}{2k+\Delta k}.}
$$

For a signed transverse [wavenumber](../../../../../../wavenumber.md), replace $\alpha$ by $|\alpha|$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
