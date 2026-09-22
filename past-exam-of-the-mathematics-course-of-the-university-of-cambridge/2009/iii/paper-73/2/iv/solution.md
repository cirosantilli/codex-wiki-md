<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Take constant [Darcy velocity](../../../../../../darcy-velocity.md) $U$ and work locally near a planar [porous thermal front](../../../../../../thermal-front-in-a-porous-medium.md) moving at $V_T=\Gamma U$. Let $\xi=x-V_Tt$ and perturb its position by $\eta=\eta_0e^{\sigma t+ia y}$, with wavelength $\lambda=2\pi/|a|$. Neglect [thermal conduction](../../../../../../thermal-conduction.md) and regard the adjoining layers as semi-infinite on this disturbance scale. In each region, [Darcy's law](../../../../../../darcy-law.md) and [incompressibility](../../../../../../incompressible-flow.md) imply that the [pressure](../../../../../../pressure.md) perturbation is harmonic, so the bounded [normal modes](../../../../../../normal-mode.md) are

$$
p'_- =A_-e^{|a|\xi}e^{\sigma t+iay},\qquad p'_+=A_+e^{-|a|\xi}e^{\sigma t+iay}.
$$

Here the minus side is cold with [dynamic viscosity](../../../../../../dynamic-viscosity.md) $\mu$, and the plus side is hot with [dynamic viscosity](../../../../../../dynamic-viscosity.md) $b\mu$. The base [pressure gradients](../../../../../../pressure-gradient.md) are $p^0_{-,x}=-\mu U/k$ and $p^0_{+,x}=-b\mu U/k$. Linearizing [pressure continuity](../../../../../../pressure-continuity.md) at the displaced front yields

$$
A_--A_+=-\eta_0\frac{(b-1)\mu U}{k}.
$$

Continuity of the perturbed normal [Darcy velocity](../../../../../../darcy-velocity.md) gives

$$
\delta U=-\frac{k|a|}{\mu}A_- =\frac{k|a|}{b\mu}A_+,
$$

so $A_+=-bA_-$. Therefore $\delta U=U|a|(b-1)\eta_0/(b+1)$. The thermal-front kinematic law is $\sigma\eta_0=\Gamma\delta U$, proving the [thermal-front viscous-fingering dispersion relation](../../../../../../thermal-front-viscous-fingering-dispersion-relation.md)

$$
\boxed{\sigma(\lambda)=\frac{2\pi\Gamma U}{\lambda}\frac{b-1}{b+1}=\frac{2\pi V_T}{\lambda}\frac{b-1}{b+1}.}
$$

It is positive for $b>1$, zero for $b=1$, and negative for $b<1$. Without [thermal conduction](../../../../../../thermal-conduction.md) the model has no finite fastest wavelength: the positive growth rate increases without bound as $\lambda\to0$. A resolved thermal transition and diffusion regularize that short-wave limit.

For a material interface the kinematic coefficient would be $1/\phi$ rather than $\Gamma$. Thus, if the interface of interest were instead the hot polymer–oil interface, the same calculation would give $\sigma=2\pi(U/\phi)(\mu_h-b\mu)/[\lambda(\mu_h+b\mu)]$, the usual [planar viscous-fingering dispersion relation](../../../../../../planar-viscous-fingering-dispersion-relation.md). This distinguishes the two interfaces and their speeds. The boxed thermal result uses the local planar approximation; distant wells or the other front modify the [pressure](../../../../../../pressure.md) eigenfunctions for wavelengths comparable to those separations.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
