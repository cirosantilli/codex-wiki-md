<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Factor the forward carrier as $E=e^{ikx}U$. Substitution into the scalar [Helmholtz equation](../../../../../../../helmholtz-equation.md) gives the exact envelope equation

$$
U_{xx}+2ikU_x+\nabla_\perp^2U+k^2(\epsilon_{\rm rel}-1)U=0.
$$

If $|U_{xx}|\ll2k|U_x|$, drop the second longitudinal derivative to obtain the [parabolic wave equation](../../../../../../../parabolic-wave-equation.md)

$$
\boxed{2ikU_x+\nabla_\perp^2U+k^2(\epsilon_{\rm rel}-1)U=0,\qquad U_x=iLU,\qquad
L=\frac1{2k}\nabla_\perp^2+\frac k2(\epsilon_{\rm rel}-1).}
$$

Typical sufficient conditions are a transverse width $w$ with $kw\gg1$, longitudinal envelope and material variation on scales much longer than $k^{-1}$, and weak refractive contrast so that factoring out the free-space carrier leaves a slowly varying envelope. A paraxial ordering has transverse propagation angles $O(\eta)$ and $\epsilon_{\rm rel}-1=O(\eta^2)$, with $U_x=O(k\eta^2U)$ and $U_{xx}$ higher order. A large refractive contrast may require a different, medium-adapted carrier even when the ray direction is nearly axial.

The [paraxial approximation](../../../../../../../paraxial-approximation.md) retains transverse diffraction and slowly accumulated refraction, but neglects backward propagation, strong reflection from rapid material changes, wide-angle propagation and, in this scalar model, polarization coupling. The supplied vector Helmholtz equation is itself a model assumption: in a source-free inhomogeneous dielectric, [Maxwell equations](../../../../../../../maxwell-equations.md) additionally require $\nabla\cdot(\epsilon\mathbf E)=0$, and generally supply a longitudinal-gradient term when the vector wave equation is expanded. An independent scalar component is justified only with a compatible polarization and the relevant small-gradient approximation.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 78](../../../../paper-78-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
