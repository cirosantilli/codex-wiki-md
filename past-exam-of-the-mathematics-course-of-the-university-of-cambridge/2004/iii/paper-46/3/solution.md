<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [partition function](../../../../../canonical-partition-function.md) sums the [Boltzmann weights](../../../../../boltzmann-factor.md) of all statistical configurations. For discrete states $s$ of energy $E_s$, $Z=\sum_se^{-\beta_{\rm th}E_s}$; for a regulated scalar field it is a [functional integral](../../../../../functional-measure.md), $Z=\int\mathcal D\phi\,e^{-\beta_{\rm th}H[\phi]}$. It normalizes probabilities and generates thermodynamic averages. Its [Helmholtz free energy](../../../../../helmholtz-free-energy.md) is

$$
\boxed{F_{\rm tot}=-k_BT\log Z.}
$$

A quantum version uses $Z=\operatorname{Tr}e^{-\beta_{\rm th}\widehat H}$. In the following identification, $F(M)$ is a constrained free-energy density, so its units match those of a Hamiltonian density rather than a total extensive energy.

Fix a microscopic cutoff $\Lambda_0$. Split the field into retained modes $\phi_<$ with momenta below $\Lambda$ and eliminated modes $\phi_>$ between $\Lambda$ and $\Lambda_0$. Define the [Wilsonian coarse-grained statistical Hamiltonian](../../../../../wilsonian-coarse-grained-statistical-hamiltonian.md) exactly by

$$
e^{-\beta_{\rm th}H_\Lambda[\phi_<]}=\int\mathcal D\phi_>\,e^{-\beta_{\rm th}H_{\Lambda_0}[\phi_<+\phi_>]}.
$$

Its coefficients and additive constant depend on $\Lambda$ so that integrating the retained modes gives precisely the original $Z$. With sources and observables carried along, the same construction preserves long-wavelength responses. Thus changing this intermediate [ultraviolet cutoff](../../../../../ultraviolet-cutoff.md) is a change of description, not a change of the physical system. It is advantageous because one can integrate out fluctuations irrelevant to the observable length scale, organize a local [gradient expansion](../../../../../gradient-expansion.md), and use [renormalization-group flow](../../../../../renormalization-group-flow.md) toward simpler universal fixed-point descriptions. Exact invariance retains all generated operators; truncating them is an approximation.

The quadratic gradient coefficient generally becomes $K_\Lambda$, not a constant. [Field renormalization](../../../../../wave-function-renormalization.md) sets a chosen kinetic normalization, for example $\phi_R=\sqrt{K_\Lambda}\phi$ when this makes the gradient coefficient one in the energy convention. Sources and observables must be transformed inversely so that their physical meaning is preserved. Under rescaled coordinates $x'=x/b$, the critical field scaling is

$$
\phi'(x')=b^{x_\phi}\phi_<(bx'),\qquad x_\phi=\frac{D-2+\eta}{2}.
$$

Its anomalous part is the [anomalous dimension](../../../../../anomalous-dimension.md); it gives $G(r)\sim r^{-2x_\phi}$ and the conjugate-field exponent $y_h=D-x_\phi$. Different conventions for the wave-function factor require corresponding changes in its logarithmic derivative. A fixed physical magnetization must not be confused with a cutoff-dependent dimensionless renormalized field.

To justify the [zero-cutoff identification of constrained free energy](../../../../../zero-cutoff-identification-of-constrained-free-energy.md), work first in a finite periodic volume $V$. Define the physical spatial mean $M=V^{-1}\int\phi(x)d^Dx$ and constrain that mean in the microscopic integral:

$$
Z_M=\int\mathcal D\phi\,\delta\left(V^{-1}\int\phi-M\right)e^{-\beta_{\rm th}H_{\Lambda_0}[\phi]},\qquad
F_c(M)=-\frac{k_BT}{V}\log Z_M.
$$

Retain the constant mode $M$ while eliminating every nonzero mode. When $\Lambda$ is below the smallest nonzero box momentum, the remaining energy is $H_\Lambda[M]=VU_\Lambda(M)$. Consequently $e^{-\beta_{\rm th}VU_\Lambda(M)}=Z_M$ with a consistently fixed, possibly field-independent measure normalization. This proves

$$
\boxed{F_c(M)=\lim_{\Lambda\to0}U_\Lambda(M).}
$$

For a uniform field, $U_\Lambda(M)$ is the Hamiltonian density $\mathcal H(\Lambda,M)$ in the question. The statement assumes that the physical zero mode is retained, all other modes are integrated exactly, field-rescaling factors are undone, and density and additive-normalization conventions agree. Taking the cutoff limit in the finite box before its [thermodynamic limit](../../../../../thermodynamic-limit.md) makes this derivation unambiguous. With an applied uniform source, $Z(h)=\int dM\,e^{-\beta_{\rm th}V[F_c(M)-hM]}$ up to the same measure convention; its large-volume saddle minimizes $F_c(M)-hM$.

The [Landau approximation](../../../../../landau-approximation.md) further assumes that this potential can be approximated by a regular local polynomial on the homogeneous branches, and that the remaining fluctuations are negligible for the observables sought. It is not an assertion that an exact zero-cutoff free energy is the bare polynomial. In a coexistence region the exact constrained density can be convexified by domains, while a nonconvex Landau branch potential describes local phases and their metastability.

For the breakdown criterion use a short-range scalar theory with positive quadratic gradient stiffness. At the [Gaussian fixed point](../../../../../gaussian-fixed-point.md), invariance of $\int(\nabla\phi)^2d^Dx$ gives field dimension $(D-2)/2$. A coupling $g_{2n}$ multiplying $\phi^{2n}$ therefore has engineering scaling exponent

$$
y_{2n}=D-2n\frac{D-2}{2}=2n-(n-1)D.
$$

It is irrelevant only above its [upper critical dimension](../../../../../upper-critical-dimension.md). For the ordinary critical point the leading stabilizing interaction is quartic, while at a tricritical point the renormalized quartic term is tuned away and the leading interaction is sextic. Therefore

$$
\boxed{D_c^{\rm ordinary}=4,\qquad D_c^{\rm tricritical}=3.}
$$

One can also see the failure through the [Ginzburg criterion](../../../../../ginzburg-criterion.md). Long-wavelength fluctuations averaged over a [correlation volume](../../../../../correlation-volume.md) obey $\langle(\delta M)^2\rangle_\xi\sim\xi^{2-D}$, up to temperature and stiffness factors. The quartic saddle has $M^2\sim\xi^{-2}$, giving a fluctuation/mean-square ratio proportional to $\xi^{4-D}$. The tricritical sextic saddle has $M^2\sim\xi^{-1}$, giving a ratio proportional to $\xi^{3-D}$. Both ratios grow without bound below their respective critical dimension, invalidating the fluctuation-free Landau exponents sufficiently close to a transition.

At equality the ratios are marginal, not power-law divergent. The loop expansion resolves this boundary: the quartic vertex correction contains $\int d^Dq/(q^2+\xi^{-2})^2$, logarithmic at $D=4$; the sextic vertex correction contains a two-loop three-propagator integral whose overall degree is $2D-6$, logarithmic at $D=3$. Marginal running therefore generally adds logarithmic corrections at these dimensions. Below them, where the corresponding transition exists, interactions control the long-distance critical behavior. Above them, leading thermodynamic powers are mean-field, although stabilizing [dangerously irrelevant couplings](../../../../../dangerously-irrelevant-coupling.md) explain why naive hyperscaling need not hold.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
