<h1 id="section-d/d17/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**[Stokes theorem](../../../../../../stokes-theorem.md) converts [circulation](../../../../../../circulation-physics.md) around an oriented boundary into [curl](../../../../../../curl.md) [flux](../../../../../../flux.md) through a spanning surface.** For a sufficiently smooth [vector field](../../../../../../vector-field.md) on an oriented piecewise smooth surface $S$,

$$
\boxed{\oint_{\partial S}\mathbf A\cdot d\mathbf l=\int_S(\nabla\times\mathbf A)\cdot\mathbf n\,dS.}
$$

The boundary orientation follows the [right-hand rule](../../../../../../right-hand-rule.md) relative to $\mathbf n$. The field must be smooth on the surface, not merely on its boundary; a singularity crossing the surface cannot be ignored. For a fixed loop, applying the theorem to Faraday's differential law gives the [integral](../../../../../../integral-split.md) [flux](../../../../../../flux.md) law of induction.

The planar form is [Green theorem](../../../../../../green-theorem.md). For a region $D$ with positively oriented boundary and sufficiently smooth $P,Q$,

$$
\boxed{\oint_{\partial D}(P\,dx+Q\,dy)=\iint_D(Q_x-P_y)\,dx\,dy.}
$$

The outer boundary is counterclockwise and any holes have clockwise boundaries. For instance $P=-y/2,Q=x/2$ makes the area of $D$ equal to half the [line integral](../../../../../../line-integral.md) of $x\,dy-y\,dx$; the unit circle gives area $\pi$.

A closely related use of “[Green's theorems](../../../../../../green-theorem.md)” in field theory is [Green's identities](../../../../../../green-s-identities.md), obtained by applying the [divergence theorem](../../../../../../divergence-theorem.md) to $\phi\nabla\psi$:

$$
\int_V(\phi\nabla^2\psi+\nabla\phi\cdot\nabla\psi)\,dV=\oint_{\partial V}\phi\,\partial_n\psi\,dS,
$$

and, after subtracting the expression with $\phi,\psi$ exchanged,

$$
\boxed{\int_V(\phi\nabla^2\psi-\psi\nabla^2\phi)\,dV=\oint_{\partial V}(\phi\partial_n\psi-\psi\partial_n\phi)\,dS.}
$$

These relate interior sources to boundary data in [electrostatics](../../../../../../electrostatics-split.md) and other boundary-value problems. For example, a [harmonic potential](../../../../../../harmonic-potential.md) difference vanishing on a [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) has zero [integral](../../../../../../integral-split.md) of its squared [gradient](../../../../../../gradient.md) by the first identity, establishing uniqueness. Both the planar [circulation](../../../../../../circulation-physics.md) theorem and the field identities are included here to make the convention clear.

## ↑ Ancestors (15)

1. [A](../a.md)
2. [D17](../../d17.md)
3. [Section D](../../../section-d.md)
4. [Paper 2A](../../../../paper-2a-split.md)
5. [2010](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
