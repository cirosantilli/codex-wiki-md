<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $u$ for the effective unloaded addition rate and $w$ for the removal rate of the same elementary tip step $a$. If the supplied on-rate is a bimolecular rate constant, then $u=k_{\rm on}c_m$, with monomer concentration $c_m$; if it already denotes an event rate, use $u=k_{\rm on}$. Assume gap [diffusion](../../../../../../diffusion.md) is much faster than chemical events, removal is [force](../../../../../../force.md)-independent, and the monomer bath is maintained.

Under a positive constant resisting [force](../../../../../../force.md), the load equilibrates in the potential $Fh$ above a reflecting tip. The normalized [Boltzmann distribution](../../../../../../boltzmann-distribution.md) is $p(h)=\beta F e^{-\beta Fh}$ for $h\ge0$, where $\beta=1/(k_BT)$. The fraction of time with room to insert is

$$
\int_a^\infty p(h)\,dh=e^{-\beta Fa}.
$$

Steric gating reduces addition to $ue^{-\beta Fa}$; each addition advances by $a$ and each removal retreats by $a$. The [reaction-limited polymerization Brownian ratchet](../../../../../../reaction-limited-polymerization-brownian-ratchet.md) therefore has

$$
\boxed{V(F)=a\left(ue^{-Fa/(k_BT)}-w\right),\qquad V(0)=a(u-w).}
$$

For $u>w>0$, the stall [force](../../../../../../force.md) is **$F_s=(k_BT/a)\log(u/w)$**. Equivalently, the available chemical free [energy](../../../../../../energy.md) per effective step is $\Delta\mu=k_BT\log(u/w)$, and stall balances $F_sa=\Delta\mu$. A half-monomer step requires rates defined for that half-step, not automatically single-strand monomer rates with a gratuitous factor of two.

At exactly zero [force](../../../../../../force.md) a load on an unbounded half-line has no normalizable equilibrium gap density. The unloaded expression is the $F\downarrow0$ limit, or the usual freely available-gap approximation with a weak positional confinement. For a positive load the equilibration time must remain short compared with reaction times. Load [inertia](../../../../../../inertia.md), filament bending, monomer depletion, and [force](../../../../../../force.md)-dependent bond rupture have been excluded. For arbitrary finite reaction and [diffusion](../../../../../../diffusion.md) rates one must solve the joint gap dynamics rather than attach $-aw$ to the [diffusion](../../../../../../diffusion.md)-limited first-passage formula: a removal changes the gap and the distribution from which the next addition starts.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
