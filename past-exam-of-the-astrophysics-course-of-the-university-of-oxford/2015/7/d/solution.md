<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the [isotropic Jeans-Abel mass inversion](../../../../isotropic-jeans-abel-mass-inversion.md), let $J(R)=I(R)\sigma_{\rm los}^2(R)$ and $p_*(r)=\nu(r)\sigma_r^2(r)$. The two preceding projections have the same [Abel integral equation](../../../../abel-integral-equation.md) kernel, giving

$$
\boxed{\nu(r)=-\frac1{\pi L}\int_r^\infty\frac{I'(R)}{\sqrt{R^2-r^2}}\,dR},\qquad
\boxed{p_*(r)=-\frac1{\pi L}\int_r^\infty\frac{J'(R)}{\sqrt{R^2-r^2}}\,dR}.
$$

Their ratio recovers $\sigma_r^2=p_*/\nu$, and the isotropic Jeans equation gives

$$
\boxed{M(\le r)=-\frac{r^2}{G\nu(r)}\frac{dp_*}{dr}}.
$$

Equivalently put $A(r)=\int_r^\infty I'(R)/\sqrt{R^2-r^2}\,dR$ and $B(r)=\int_r^\infty J'(R)/\sqrt{R^2-r^2}\,dR$. Then $M=-r^2B'(r)/(GA(r))$: the common stellar [luminosity](../../../../luminosity.md) cancels from the inferred [mass](../../../../mass.md). Differentiating these singular-kernel integrals is understood through suitable regularity or a nonsingular variable change, not by naively keeping an infinite lower-end boundary term.

The inversion assumes adequate radial coverage, convergence and a smooth spherical equilibrium. In practice derivatives amplify noise and the unobserved outer tail needs treatment or a model. Unknown anisotropy reintroduces a [mass](../../../../mass.md)–anisotropy degeneracy; the uniqueness just derived is conditional on the explicitly isotropic velocity distribution.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
