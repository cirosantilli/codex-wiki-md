<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Adding $40000$ monovalent [counterions](../../../../counterion.md) makes the combined genome-plus-ion [electric charge](../../../../electric-charge-split.md) nominally zero. It does **not** make the local [electric field](../../../../electric-field-split.md) or [free energy](../../../../thermodynamic-free-energy.md) vanish: opposite charges have spatial distributions, and confining mobile [ions](../../../../ion.md) costs [entropy](../../../../entropy-split.md).

A definite screened continuation of [b](../b.md) replaces the bare [Coulomb potential](../../../../coulomb-potential-energy.md) by $e^{-\kappa r}/(4\pi\epsilon r)$, with $\kappa=1/\lambda_D$ and $\lambda_D=1\,\mathrm{nm}$. In the [Debye–Hückel approximation](../../../../debye-huckel-approximation.md), a uniformly distributed fixed [charge density](../../../../charge-density.md) $\rho=Q/V_c$ satisfies $(\nabla^2-\kappa^2)\varphi=-\rho/\epsilon$ inside, with zero fixed charge outside and matching potential and radial field at $R$. Its interior solution is

$$
\varphi(r)=\frac{\rho}{\epsilon\kappa^2}\left[1-(1+x)e^{-x}\frac{\sinh(\kappa r)}{\kappa r}\right],\qquad x=\kappa R.
$$

The screened charging [free energy](../../../../thermodynamic-free-energy.md) $U_\kappa=\tfrac12\int\rho\varphi\,dV$ is therefore

$$
\boxed{U_\kappa=\frac{Q^2\lambda_D^2}{2\epsilon V_c}
\left\{1-\frac{3(x+1)}{2x^3}\left[(x-1)+(x+1)e^{-2x}\right]\right\}.}
$$

For $R\gg\lambda_D$, the bracket approaches one: only charges within roughly a screening length contribute appreciably, yielding the local estimate $U_\kappa\simeq Q^2\lambda_D^2/(2\epsilon V_c)$. With the same $\epsilon_r=80$ as before, $x=20$ gives bracket $0.92519$ and

$$
\boxed{U_\kappa\simeq8.00\times10^5\,\mathrm{pN\,nm},}
$$

about $173$ times smaller than the unscreened packed-sphere self-energy. This is a specified continuum estimate of packed-state charging [free energy](../../../../thermodynamic-free-energy.md); a full packaging [free energy](../../../../thermodynamic-free-energy.md) also subtracts the screened unpacked reference and includes ion redistribution. It should not be presented as a unique exact packaging [work](../../../../work.md) fixed by the problem's few inputs.

The supplied [counterion](../../../../counterion.md) count also permits an independent estimate of the entropic contribution. For $N$ ideal confined [ions](../../../../ion.md), $F_{\rm ion}=-Nk_BT\ln V+\text{constant}$, so compression from an accessible reference [volume](../../../../volume.md) $V_0$ to $V_f$ costs

$$
\boxed{\Delta F_{\rm ion}=Nk_BT\ln\frac{V_0}{V_f},\qquad Nk_BT=1.66\times10^5\,\mathrm{pN\,nm}\quad(T=300\,\mathrm K).}
$$

For example, approximate the original screening atmosphere as an annulus of thickness $\lambda_D$ around a rod. With $a=0.5\,\mathrm{nm}$, $V_0=\pi[(a+\lambda_D)^2-a^2]L=4.27\times10^4\,\mathrm{nm^3}$. Taking $V_f=V_c-V_D=1.35\times10^4\,\mathrm{nm^3}$ gives $\Delta F_{\rm ion}\simeq1.91\times10^5\,\mathrm{pN\,nm}$. This useful order-of-magnitude ion-entropy model is distinct from the screened charging model; the two estimates must not simply be added as independent terms without a consistent ionic [free energy](../../../../thermodynamic-free-energy.md) functional. The rod cutoff, fixed [DNA](../../../../deoxyribonucleic-acid.md) volume and screening-atmosphere geometry are rough geometric assumptions, not a microscopic reconstruction of the source sketch.

There is a further consistency limit. The nominal ion [number density](../../../../number-density.md) is $n=N/V_c=1.19\,\mathrm{nm^{-3}}$. For a uniform ideal monovalent screening gas, $\lambda_D^2=\epsilon k_BT/(ne^2)$ would give $\lambda_D\simeq0.309\,\mathrm{nm}$ at $300\,\mathrm K$, rather than $1\,\mathrm{nm}$; added salt would shorten it further. Thus the stated ion inventory and screening length cannot both be interpreted as a self-consistent dilute uniform screening gas with this dielectric. Bound [counterions](../../../../counterion.md), nonuniform distributions and an effective phenomenological screening length can change that interpretation. Linear screening is itself only an estimate near highly charged [DNA](../../../../deoxyribonucleic-acid.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
