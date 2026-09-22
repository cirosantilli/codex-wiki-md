<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Orient the [unit normal](../../../../unit-normal.md) $\mathbf n$ from $R_1$ to $R_2$ and write $\mathbf H$ for the [magnetic field strength](../../../../magnetic-field-strength.md). For static [electric fields](../../../../electric-field-split.md), $\mathbf E=-\nabla\phi$; the static [Ampère's law](../../../../ampere-s-circuital-law.md) gives $\nabla\times\mathbf H=\mathbf J_f$. The [curl](../../../../curl.md) product rule therefore gives the local [Poynting flux and terminal power](../../../../poynting-flux-and-terminal-power.md) identity

$$
\boldsymbol{\mathcal P}=-\nabla\phi\times\mathbf H
=\phi\mathbf J_f-\nabla\times(\phi\mathbf H).
$$

Integrate over an oriented piece $\Sigma_R$ of the separating surface and apply [Stokes theorem](../../../../stokes-theorem.md):

$$
\int_{\Sigma_R}\boldsymbol{\mathcal P}\cdot\mathbf n\,dS
=\int_{\Sigma_R}\phi\mathbf J_f\cdot\mathbf n\,dS
-\oint_{\partial\Sigma_R}\phi\mathbf H\cdot d\boldsymbol\ell.
$$

Once all the wires are included, the first [surface integral](../../../../surface-integral.md) is $\sum_k\phi_kI_k$: the [electric potential](../../../../electric-potential.md) is constant on each [perfect conductor](../../../../perfect-conductor.md) and the integral of its normal [current density](../../../../current-density.md) is its signed [electric current](../../../../electric-current.md). Equivalently, remove the wire cross-sections and apply [Stokes theorem](../../../../stokes-theorem.md) in the surrounding insulator. Each resulting hole has negative boundary orientation, and the [magnetostatic Ampère law](../../../../magnetostatic-ampere-law.md) around it gives the positive contribution $\phi_kI_k$.

For a closed separating surface the boundary term is absent. For a noncompact separating surface, take $R\to\infty$ with the usual isolated-circuit condition $\oint_{\partial\Sigma_R}\phi\mathbf H\cdot d\boldsymbol\ell\to0$. In either case,

$$
\boxed{\int_\Sigma\boldsymbol{\mathcal P}\cdot\mathbf n\,dS=\sum_{k=1}^N\phi_kI_k.}
$$

For a steady closed circuit the signed [electric currents](../../../../electric-current.md) sum to zero, so shifting the reference of [electric potential](../../../../electric-potential.md) does not change the terminal power.

For a fully general noncompact surface, the hypotheses as printed need an additional condition at infinity. The exact result before imposing it is

$$
\boxed{P_{1\to2}=\sum_{k=1}^N\phi_kI_k-
\lim_{R\to\infty}\oint_{\partial\Sigma_R}\phi\mathbf H\cdot d\boldsymbol\ell.}
$$

Time independence alone does not remove this boundary term or ensure a finite [Poynting flux](../../../../poynting-flux.md); for example, spatially constant crossed [electric fields](../../../../electric-field-split.md) and [magnetic fields](../../../../magnetic-field-split.md) carry a constant [Poynting vector](../../../../poynting-vector.md) through an infinite plane. The stated terminal-power formula holds with the boundary condition specified above.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the electromagnetism course of the University of Oxford](../../../split.md)
5. [Electromagnetism course of the University of Oxford](../../../../electromagnetism-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
