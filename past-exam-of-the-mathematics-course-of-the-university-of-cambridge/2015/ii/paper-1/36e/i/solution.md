<h1 id="36e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

An isotropic fourth-order tensor has the form $A_{ijkl}=a\delta_{ij}\delta_{kl}+b\delta_{ik}\delta_{jl}+c\delta_{il}\delta_{jk}$. Contracting with the velocity gradient gives $a\delta_{ij}\nabla\cdot u+b\partial_ju_i+c\partial_iu_j$. [Incompressibility](../../../../../../incompressible-flow.md) removes the first term. Symmetry of the stress for arbitrary incompressible velocity gradients, including antisymmetric ones, forces $b=c$. Writing their common value as the [dynamic viscosity](../../../../../../dynamic-viscosity.md) $\mu$ yields

$$
\boxed{A_{ijkl}\partial_lu_k=\mu(\partial_ju_i+\partial_iu_j)=2\mu e_{ij}}.
$$

The asserted constant is the homogeneous material coefficient of this Newtonian constitutive law. Isotropy alone fixes its tensor form, not spatial constancy if the material's viscosity were allowed to vary.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [36E](../../36e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
