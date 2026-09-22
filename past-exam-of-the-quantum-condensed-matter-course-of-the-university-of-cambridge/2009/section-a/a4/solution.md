<h1 id="section-a/a4/solution">Solution</h1>

↑ **Parent:** [A4](../a4.md)

For a freely jointed [Gaussian chain](../../../../gaussian-chain.md), independent isotropic segment vectors have zero mean and coordinate variance $\ell^2/3$. The [central limit theorem](../../../../central-limit-theorem.md) gives the end-to-end vector density

$$
p(\mathbf R)=\left(\frac{3}{2\pi N\ell^2}\right)^{3/2}\exp\left[-\frac{3R^2}{2N\ell^2}\right].
$$

The number of conformations in a fixed small vector-volume element is proportional to this density. Taking its logarithm gives the configurational [entropy](../../../../entropy-split.md)

$$
S(\mathbf R)=S_0-\frac{3k_BR^2}{2N\ell^2}.
$$

This is the vector-constrained entropy appropriate to an anchored strand. A density for the scalar length alone also has a $4\pi R^2$ shell factor and is a different constraint. The approximation requires many segments and extensions well below $N\ell$.

If the internal energy has negligible extension dependence, the [Helmholtz free energy](../../../../helmholtz-free-energy.md) is $F=F_0+3k_BTR^2/(2N\ell^2)$. Differentiation gives an [entropic force](../../../../entropic-force.md) with effective spring constant $3k_BT/(N\ell^2)$. In an affine isotropic network, averaging over initially oriented strands gives [rubber elasticity](../../../../rubber-elasticity.md)

$$
G=\nu_s k_BT,\qquad E=3G=3\nu_s k_BT
$$

for an incompressible material; $\nu_s$ is the number of elastically active strands per volume. For example a volume-preserving stretch with principal factors $\lambda,\lambda^{-1/2},\lambda^{-1/2}$ has strain-energy density $W=G(\lambda^2+2/\lambda-3)/2$. Its nominal tensile [stress](../../../../stress.md) is $G(\lambda-\lambda^{-2})=3G(\lambda-1)+O((\lambda-1)^2)$, proving the stated small-strain [Young's modulus](../../../../young-s-modulus.md).

Chemically, increasing the effective [cross-link](../../../../cross-link.md) density, for example by changing vulcanization, generally increases the modulus by shortening strands between cross-links. Dangling ends, loops and changes of network structure mean the chemical junction count need not equal $\nu_s$.

The reference area is $A_0=10^{-5}\ \mathrm{m^2}$. Neglect self-weight, thermal expansion and energetic elasticity, keep the same permanent network, and heat quasistatically in the rubbery regime. Then $G$ increases from $20$ to $22\ \mathrm{MPa}$. With a constant suspended load, the exact affine-network balance is

$$
\frac{mg}{A_0}=G(T)(\lambda-\lambda^{-2}).
$$

It gives $\lambda_{300}=1.01662$ and $\lambda_{330}=1.01509$. Thus

$$
\boxed{\text{the lower end rises by approximately }1.53\ \mathrm{mm}.}
$$

Linear elasticity instead gives extensions $16.35$ and $14.86\ \mathrm{mm}$, a $1.49\ \mathrm{mm}$ rise, consistent at this small strain. Incompressibility makes the area $A_0/\lambda$, already included by using nominal [stress](../../../../stress.md). Heating increases entropic stiffness, so the loaded rubber contracts and performs work on the mass. Strong thermal expansion, changes in cross-linking or leaving the rubbery regime would require additional material data.

## ↑ Ancestors (13)

1. [A4](../a4.md)
2. [Section A](../../section-a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
