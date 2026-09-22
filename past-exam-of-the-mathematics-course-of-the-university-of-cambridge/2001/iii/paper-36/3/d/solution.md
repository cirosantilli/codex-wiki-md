<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In a planar cross-section write the [magnetic field](../../../../../../magnetic-field.md) as

$$
\mathbf B=(\psi_y,-\psi_x,0)=\nabla\psi\times\mathbf e_z.
$$

The [Cartesian magnetic flux function](../../../../../../cartesian-magnetic-flux-function.md) $\psi$ labels the [magnetic field lines](../../../../../../magnetic-field-line.md). Ideal induction, with a suitable additive gauge, gives

$$
\partial_t\psi+\mathbf v\cdot\nabla\psi=0.
$$

Thus each flux contour is material. [Incompressibility](../../../../../../incompressible-flow.md) also preserves the area inside any material contour. Neither a [magnetic island](../../../../../../magnetic-island.md)'s flux distribution nor the connections of a [separatrix](../../../../../../separatrix.md) can be freely altered during relaxation.

A configuration with two or more [magnetic islands](../../../../../../magnetic-island.md) separated by an X-type saddle illustrates the mechanism. As the [magnetic islands](../../../../../../magnetic-island.md) reshape to lower [magnetic energy](../../../../../../magnetic-energy.md), the arms of the [separatrix](../../../../../../separatrix.md) can be pressed together. [Magnetic reconnection](../../../../../../magnetic-reconnection.md) would change the topology, so it is excluded in a [perfect conductor](../../../../../../perfect-conductor.md). The X-type structure can instead flatten into an extended interface, with oppositely directed tangential fields on its two sides. The transition shrinks and the [electric current density](../../../../../../current-density.md) concentrates into a [current sheet](../../../../../../current-sheet.md). Such collapse in two-dimensional relaxation is documented in section 4 of [Moffatt's primary discussion](https://www.damtp.cam.ac.uk/user/hkm2/PDFs/Moffatt_1998_InternationalPress_Tdof_465.pdf). It is a possible asymptotic outcome, not a finite-time singularity assertion or a property of every planar field.

The local equations show precisely how the interface can support equilibrium. For the planar field,

$$
j_z=-\frac1{\mu_0}\Delta\psi,\qquad \mathbf j\times\mathbf B=-\frac{\Delta\psi}{\mu_0}\nabla\psi.
$$

On a regular connected flux region, [magnetostatic equilibrium](../../../../../../magnetostatic-equilibrium.md) therefore implies $p=P(\psi)$ and

$$
\Delta\psi=-\mu_0P'(\psi).
$$

Different disconnected flux regions can have different functions $P$. Their limiting fields need not join with continuous first derivatives of $\psi$ across a common [separatrix](../../../../../../separatrix.md); continuity of total [pressure](../../../../../../pressure.md) allows the tangential-field jump.

For an explicit local sheet, take

$$
\mathbf B_\epsilon=B_s\tanh(y/\epsilon)\mathbf e_x,\qquad p_\epsilon=p_T-\frac{B_s^2}{2\mu_0}\tanh^2(y/\epsilon).
$$

These satisfy [magnetostatic equilibrium](../../../../../../magnetostatic-equilibrium.md) exactly, with

$$
j_z=-\frac{B_s}{\mu_0\epsilon}\operatorname{sech}^2(y/\epsilon)\ \longrightarrow\ -\frac{2B_s}{\mu_0}\delta(y).
$$

The finite limiting surface current agrees with the field-jump formula. This is a local equilibrium demonstration of the sheet balance, not a claim that this particular family is the full ideal relaxation trajectory from the given initial data.

Strictly planar fields of the form above have zero [magnetic helicity](../../../../../../magnetic-helicity.md): choose $\mathbf A=\psi\mathbf e_z$, giving $\mathbf A\cdot\mathbf B=0$. Thus this strictly planar example interprets the last part as a separate illustration of topology-constrained relaxation. It still has an energy obstruction: if $\psi=0$ on the cross-sectional boundary, the advected integral $\int\psi^2\,dx\,dy$ is constant and the [Poincaré inequality](../../../../../../poincare-inequality.md) gives $M\geq\lambda_1\int\psi^2\,dx\,dy/(2\mu_0)$ per unit length. If the earlier nonzero-helicity condition is retained instead, a possible extension is a field depending on only two coordinates but permitting an axial component, with periodic boundary conditions in the invariant direction. Write

$$
\mathbf B=(\psi_y,-\psi_x,G(\psi)).
$$

The axial force balance makes the axial component a function of $\psi$ on each regular connected region; the remaining [Cartesian magnetostatic flux-function equilibrium](../../../../../../cartesian-magnetostatic-flux-function-equilibrium.md) is

$$
\Delta\psi+GG'+\mu_0P'=0.
$$

In that periodic extension, with consistent flux and gauge conventions, and $\psi=0$ on the cross-sectional boundary, integration by parts gives helicity per unit length $H_M/L_z=2\int\psi B_z,dx\,dy$. It can be nonzero. The same separatrix-collapse mechanism still concentrates current in a sheet. **Three-dimensional linkage is therefore unnecessary for sheet formation; planar frozen flux-contour topology already supplies the constraint.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
