<h1 id="35c/solution">Solution</h1>

↑ **Parent:** [35C](../35c.md)

Use SI units and normalize the condensate [wavefunction](../../../../../wave-function.md) so $|\psi|^2=n$. With [mechanical momentum](../../../../../mechanical-momentum.md) operator $-i\hbar\nabla-qA$, the charge [current density](../../../../../current-density.md) is

$$
\boxed{j=\frac{q\hbar}{2mi}(\psi^*\nabla\psi-\psi\nabla\psi^*)-\frac{q^2}{m}|\psi|^2A.}
$$

For uniform $n$ and $\psi=\sqrt n\,e^{i\vartheta}$, this becomes $j=(nq/m)(\hbar\nabla\vartheta-qA)$.

Under the [gauge transformation](../../../../../gauge-transformation.md) $A\mapsto A+\nabla\chi$, the [wavefunction](../../../../../wave-function.md) transforms as $\psi\mapsto e^{iq\chi/\hbar}\psi$, so $\vartheta\mapsto\vartheta+q\chi/\hbar$. The two added gradients cancel in $\hbar\nabla\vartheta-qA$, while $|\psi|^2$ stays fixed. Thus **the superconducting current is gauge invariant**. The same cancellation in the full displayed current proves it without requiring a constant amplitude.

For uniform carrier density in a region with smooth single-valued phase, taking a curl gives the [London equation](../../../../../london-equations.md) $\nabla\times j=-nq^2B/m$. In the time-independent setting [Ampère's circuital law](../../../../../ampere-s-circuital-law.md) gives $\nabla\times B=\mu_0j$, and [Gauss's law for magnetism](../../../../../gauss-s-law-for-magnetism.md) gives $\nabla\cdot B=0$. Therefore

$$
-\nabla^2B=\nabla\times(\nabla\times B)=\mu_0\nabla\times j=-\frac{\mu_0nq^2}{m}B,
$$

so the [Helmholtz equation](../../../../../helmholtz-equation.md) and [London penetration depth](../../../../../london-penetration-depth.md) are

$$
\boxed{\nabla^2B=\frac{B}{\ell^2},\qquad\ell=\sqrt{\frac{m}{\mu_0nq^2}}.}
$$

The equation has the modified, exponentially decaying Helmholtz sign. For a planar surface at $x=0$ with material in $x>0$, the bounded solution is $B(x)=B(0)e^{-x/\ell}$; the exponentially growing solution is excluded in the bulk. Hence a macroscopic region far from the surface has negligible field: **magnetic flux is expelled from the bulk**, the [Meissner effect](../../../../../meissner-effect.md). The literal assertion of zero flux everywhere is the bulk limit: finite penetration remains within distance $\ell$ of a surface. Vortices or flux trapped through a hole require different phase or topology assumptions and are not ruled out by this smooth-phase derivation.

## ↑ Ancestors (10)

1. [35C](../35c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
