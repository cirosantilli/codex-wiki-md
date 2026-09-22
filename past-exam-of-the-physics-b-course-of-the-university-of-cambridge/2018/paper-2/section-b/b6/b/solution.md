<h1 id="section-b/b6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**[Integral](../../../../../../integral-split.md) conservation.** [Electric charge](../../../../../../electric-charge-split.md) cannot be created by ordinary transport. For a fixed [volume](../../../../../../volume-thermodynamics.md) $V$, outward current reduces the enclosed charge:

$$
\frac{d}{dt}\int_V\rho_e\,dV=-\oint_{\partial V}\mathbf J\cdot\widehat{\mathbf n}\,dA.
$$

Here $\rho_e$ has units $\mathrm{C\,m^{-3}}$ and $\mathbf J$ has units $\mathrm{A\,m^{-2}}$. Applying the [divergence theorem](../../../../../../divergence-theorem.md) to an arbitrary [volume](../../../../../../volume-thermodynamics.md) gives the local [continuity equation](../../../../../../continuity-equation.md)

$$
\boxed{\frac{\partial\rho_e}{\partial t}+\nabla\cdot\mathbf J=0.}
$$

It is local [charge conservation](../../../../../../charge-conservation.md): a net outflow must be accompanied by depletion. In a steady state, $\nabla\cdot\mathbf J=0$. Integrating over a small circuit junction then gives [Kirchhoff's current law](../../../../../../kirchhoff-node-law.md). During a transient the junction can accumulate charge and the incoming and outgoing conduction currents need not yet match.

**Consistency with [Maxwell's equations](../../../../../../maxwell-equations-split.md).** In [vacuum](../../../../../../vacuum.md), take the [divergence](../../../../../../divergence.md) of the [Ampère-Maxwell equation](../../../../../../ampere-s-circuital-law.md):

$$
\nabla\times\mathbf B=\mu_0\mathbf J+\mu_0\epsilon_0\partial_t\mathbf E,
\qquad
0=\mu_0\nabla\cdot\mathbf J+\mu_0\epsilon_0\partial_t(\nabla\cdot\mathbf E).
$$

[Gauss's law](../../../../../../gauss-s-law.md), $\nabla\cdot\mathbf E=\rho_e/\epsilon_0$, reproduces the [continuity equation](../../../../../../continuity-equation.md). The [displacement current](../../../../../../displacement-current.md) term makes these equations consistent for time-dependent charge distributions, such as a charging [capacitor](../../../../../../capacitor.md). It is not a stream of free charges across the insulating gap. In matter, $\nabla\cdot\mathbf D=\rho_f$ and $\nabla\times\mathbf H=\mathbf J_f+\partial_t\mathbf D$ give the analogous [conservation law](../../../../../../conservation-law.md) for [free charge](../../../../../../free-charge.md); total charge also includes [bound charge](../../../../../../bound-charge.md).

## ↑ Ancestors (15)

1. [B](../b.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
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
