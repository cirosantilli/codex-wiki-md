<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Rearrange the source's condensate-current expression and integrate around a closed path lying in the superconducting material:

$$
\hbar\oint\nabla\theta\cdot d\mathbf l=q\oint\mathbf A\cdot d\mathbf l+\frac{m}{n_sq}\oint\mathbf J_s\cdot d\mathbf l.
$$

Single-valuedness of the superconducting wavefunction requires $\oint\nabla\theta\cdot d\mathbf l=2\pi n$, and [Stokes theorem](../../../../stokes-theorem.md) gives $\oint\mathbf A\cdot d\mathbf l=\Phi$. Thus the exact result is [fluxoid and flux quantization in a superconductor](../../../../fluxoid-and-flux-quantization-in-a-superconductor.md):

$$
\boxed{\Phi+\frac{m}{n_sq^2}\oint\mathbf J_s\cdot d\mathbf l=\frac{nh}{q}.}
$$

Reversing the winding orientation absorbs the sign of $q$. Since a [Cooper pair](../../../../cooper-pair.md) has $|q|=2e$, the positive [superconducting flux quantum](../../../../superconducting-flux-quantum.md) is

$$
\boxed{\Phi_0=\frac{h}{2e}\simeq2.068\times10^{-15}\,\mathrm{Wb}.}
$$

For a thick ring, choose the path deep enough that the supercurrent is negligible; then the enclosed [magnetic flux](../../../../magnetic-flux.md) is $n\Phi_0$. This is the flux quantization usually intended in the question.

**Qualification of the unqualified flux claim:** a thin ring can have a nonzero kinetic contribution around every available path, so it is the [fluxoid](../../../../fluxoid.md) that is exactly quantized. For example, with zero applied flux and geometric and kinetic inductances $L_g=L_k$, a metastable winding-$1$ state has $(L_g+L_k)I=\Phi_0$ but $\Phi=L_gI=\Phi_0/2$. This concrete counterexample satisfies the given current law while its magnetic flux is not an integer multiple of $\Phi_0$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the condensed matter physics major option course of the University of Oxford](../../../split.md)
5. [Condensed matter physics major option course of the University of Oxford](../../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
