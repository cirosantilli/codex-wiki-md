<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $\eta_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$ and define the physical electromagnetic source by $\partial_\nu F^{\nu\mu}=J^\mu$. For a constant infinitesimal phase $\delta\varphi=ie\epsilon\varphi$, the matter [Noether current](../../../../noether-current.md) is

$$
\boxed{J^\mu=ie\left[\varphi(D^\mu\varphi)^*-\varphi^*D^\mu\varphi\right]
=ie(\varphi\partial^\mu\varphi^*-\varphi^*\partial^\mu\varphi)-2e^2|\varphi|^2A^\mu.}
$$

A definition using phase parameter $\delta\varphi=i\epsilon\varphi$ instead divides this expression by $e$; the Maxwell source includes the electric coupling shown here. Current signs must be tied to the printed $D_\mu=\partial_\mu-ieA_\mu$ convention.

To verify the equation of motion, vary the matter kinetic term with respect to $A_\mu$:

$$
\delta\mathcal L_{\rm matter}=-J^\mu\delta A_\mu.
$$

Varying $-F^2/4$ and integrating by parts gives $(\partial_\nu F^{\nu\mu})\delta A_\mu$. The stationary action therefore requires

$$
\boxed{\partial_\nu F^{\nu\mu}=J^\mu.}
$$

The potential has no explicit dependence on $A_\mu$ and contributes no extra source term. Antisymmetry of $F^{\nu\mu}$ implies $\partial_\mu J^\mu=0$ on the equations of motion; the same conservation law follows from the scalar equations. The source current is [gauge-invariant](../../../../gauge-invariance.md) although its expanded derivative and vector-potential pieces are not separately invariant.[§§6.1.1 and 6.3.2, gauge symmetry and scalar coupling; the sign here follows the source's minus-sign covariant derivative](../../../../quantum-field-theory-by-david-tong.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
