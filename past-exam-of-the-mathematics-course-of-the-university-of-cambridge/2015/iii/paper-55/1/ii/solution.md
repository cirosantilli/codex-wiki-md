<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\mathcal D=\bar N^{-1}\partial_t$, $\bar\Pi=\mathcal D\bar\phi$ and $\Delta=a^{-2}\nabla^2$. Since the background scalar has no spatial gradient,

$$
\delta\Pi=\mathcal D\delta\phi-\bar\Pi\Psi,\qquad
\boxed{\delta\rho=\bar\Pi\mathcal D\delta\phi-\bar\Pi^2\Psi+V_{,\phi}\delta\phi,
\quad u=\bar\Pi\delta\phi,\quad J_i=-\partial_i u.}
$$

Also $\delta P=\bar\Pi\mathcal D\delta\phi-\bar\Pi^2\Psi-V_{,\phi}\delta\phi$. These are the linearized [scalar-field matter projections](../../../../../../scalar-field-matter-projections.md); gradient energy first contributes quadratically.

There is a source convention defect in the shear formula. For the stated positive shift $N_i=a^2B_{,i}$ and spatial metric with $+2E_{,ij}$, direct substitution into the [extrinsic curvature](../../../../../../extrinsic-curvature.md) gives the [positive-shift scalar shear convention](../../../../../../positive-shift-scalar-shear-convention.md)

$$
\chi_+=\frac{a^2}{\bar N}(B-\dot E),\qquad
K^i{}_j=-H\delta^i{}_j+(\mathcal D\Phi+H\Psi)\delta^i{}_j+\partial^i\partial_j\chi_+,
$$



$$
\boxed{\kappa=\delta K=3(\mathcal D\Phi+H\Psi)+\Delta\chi_+.}
$$

There is no extra Laplacian in the definition of $\chi_+$. Equivalently use $\chi=-\chi_+$: then the trace-free term has the printed minus sign and $\kappa=3(\mathcal D\Phi+H\Psi)-\Delta\chi$. This latter convention retains the printed momentum-constraint form. The source mixes these two choices.

At first order $\delta(K^2)=-6H\kappa$ and $\delta(K^i{}_jK^j{}_i)=-2H\kappa$. Combining their difference with $\delta{}^{(3)}R=4\Delta\Phi$ gives

$$
\boxed{\Delta\Phi-H\kappa=4\pi G\delta\rho.}
$$

For the [momentum constraint](../../../../../../momentum-constraint.md), differentiating the tensor above gives

$$
\partial_j\delta K^j{}_i-\partial_i\delta K
=-\frac23\partial_i(\kappa-\Delta\chi_+)
=-8\pi G\partial_i u.
$$

For nonzero Fourier wavenumber, and absorbing the homogeneous integration mode into the background, **the consistent [momentum constraint](../../../../../../momentum-constraint.md) is**

$$
\boxed{\kappa-\Delta\chi_+=12\pi Gu,
\qquad\text{or}\qquad\kappa+\Delta\chi=12\pi Gu.}
$$

Linearizing the scalar equation, the shift-advection term and lapse-gradient times scalar-gradient term vanish at this order because the background is spatially homogeneous. The remaining equation is

$$
\mathcal D\delta\Pi-\Psi\mathcal D\bar\Pi+3H\delta\Pi-\kappa\bar\Pi-\Delta\delta\phi+V_{,\phi\phi}\delta\phi=0.
$$

Insert $\delta\Pi$, differentiate its lapse term, and use $\mathcal D\bar\Pi+3H\bar\Pi=-V_{,\phi}$. The two background-acceleration terms combine into $2\Psi V_{,\phi}+3H\bar\Pi\Psi$. Hence **the [perturbed Klein-Gordon equation with background lapse](../../../../../../perturbed-klein-gordon-equation-with-background-lapse.md) is**

$$
\boxed{\frac{\delta\ddot\phi}{\bar N^2}
+\left(3H-\frac{\dot{\bar N}}{\bar N^2}\right)\frac{\delta\dot\phi}{\bar N}
-\Delta\delta\phi+V_{,\phi\phi}\delta\phi
-\frac{\dot{\bar\phi}}{\bar N}\left(\kappa+\frac{\dot\Psi}{\bar N}-3H\Psi\right)
+2\Psi V_{,\phi}=0.}
$$

This scalar evolution equation and the [Hamiltonian constraint](../../../../../../hamiltonian-constraint.md) agree with the displayed targets after the shear conventions are repaired.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
