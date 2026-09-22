<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathbf x'=\mathbf x-\mathbf vt$, $t'=t$ for a constant relative [velocity](../../../../../../velocity.md) $\mathbf v$. The [Galilean transformation](../../../../../../galilean-transformation.md) gives $\nabla'=\nabla$ and $\partial_{t'}=\partial_t+\mathbf v\cdot\nabla$. In the [magnetic Galilean limit of the pre-Maxwell equations](../../../../../../magnetic-galilean-limit-of-the-pre-maxwell-equations.md), take

$$
\boxed{\mathbf B'=\mathbf B,\qquad \mathbf J'=\mathbf J,\qquad \mathbf E'=\mathbf E+\mathbf v\times\mathbf B.}
$$

The [Ampère's law](../../../../../../ampere-s-circuital-law.md) without [displacement current](../../../../../../displacement-current.md) and the solenoidal constraint are immediately unchanged. For [Faraday's law](../../../../../../faraday-s-law-of-induction.md), the constant-[velocity](../../../../../../velocity.md) vector identity is $\nabla\times(\mathbf v\times\mathbf B)=\mathbf v\nabla\cdot\mathbf B-(\mathbf v\cdot\nabla)\mathbf B$. Thus

$$
-\nabla'\times\mathbf E'=-\nabla\times\mathbf E+(\mathbf v\cdot\nabla)\mathbf B=\partial_{t'}\mathbf B'.
$$

These are transformations of the magnetic nonrelativistic approximation. The exact charge-current transformation also contains the convective term $-\rho_e\mathbf v$ in $\mathbf J'$; ignoring it requires the quasineutral magnetic limit. They are not exact transformations of the full [Maxwell equations](../../../../../../maxwell-equations.md).

Since $\mathbf u'=\mathbf u-\mathbf v$, the combination $\mathbf E'+\mathbf u'\times\mathbf B'$ equals $\mathbf E+\mathbf u\times\mathbf B$. For an ideally conducting fluid the rest-frame [electric field](../../../../../../electric-field.md) vanishes, so the ideal [moving-conductor Ohm law](../../../../../../moving-conductor-ohm-law.md) is $\mathbf E+\mathbf u\times\mathbf B=0$. Substitution in [Faraday's law](../../../../../../faraday-s-law-of-induction.md) gives

$$
\boxed{\partial_t\mathbf B=\nabla\times(\mathbf u\times\mathbf B),\qquad\nabla\cdot\mathbf B=0.}
$$

The [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) requires nonrelativistic fluid motion, negligible [displacement current](../../../../../../displacement-current.md), and negligible nonideal terms in the electric-field relation. In particular, [magnetic diffusion](../../../../../../magnetic-diffusion.md) must be slow compared with advection: the [magnetic Reynolds number](../../../../../../magnetic-reynolds-number.md) $\mathrm{Rm}=UL/\eta_m\gg1$, where $\eta_m=(\mu_0\sigma)^{-1}$ is the [magnetic diffusivity](../../../../../../magnetic-diffusivity.md). The single-fluid [moving-conductor Ohm law](../../../../../../moving-conductor-ohm-law.md) must apply on the scales considered, with corrections to that relation negligible; viscosity is not itself excluded by this induction equation.

For a smooth ideal evolution, [magnetic flux freezing](../../../../../../magnetic-flux-freezing.md) states that the [magnetic flux](../../../../../../magnetic-flux.md) through every material surface is conserved and that [magnetic field lines](../../../../../../magnetic-field-line.md) are carried with the fluid. Their connectivity is preserved: ideal smooth advection does not reconnect them. These implications are stated here without proof, as requested.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
