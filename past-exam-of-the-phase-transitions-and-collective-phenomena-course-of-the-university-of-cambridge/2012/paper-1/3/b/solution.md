<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Renormalization](../../../../../renormalization.md) compares the same long-distance physics at different observation scales. The starting object is a microscopic or cutoff [statistical Hamiltonian](../../../../../statistical-hamiltonian.md) $\mathcal H_g$ with every symmetry-allowed coupling $g$. Because a critical [correlation length](../../../../../correlation-length.md) is much larger than a lattice spacing, repeatedly eliminating short-distance detail can reveal scale-invariant behavior.

In a real-space transformation choose a [normalized blocking kernel](../../../../../normalized-blocking-kernel.md) $B(S|s)$ for retained variables. Define

$$
e^{-\mathcal H_{g'}(S)}=\sum_sB(S|s)e^{-\mathcal H_g(s)},\qquad\sum_SB(S|s)=1.
$$

Summing over $S$ proves exact preservation of $Z$ before truncation. The transformed [Hamiltonian](../../../../../hamiltonian.md) generally gains longer-range and many-body interactions and a field-independent constant. Observables must be blocked consistently. In momentum-shell language split $\phi=\phi_<+\phi_>$, integrate $\Lambda/b<|q|<\Lambda$, then use $x'=x/b$ and a field rescaling to restore cutoff and kinetic normalization. **Coarse-graining, rescaling and tracking generated interactions are distinct steps.**

Repeated transformations generate a flow $g'=R_b(g)$ with composition $R_bR_c=R_{bc}$ when the same exact coarse-graining family is used. Losing degrees of freedom generally makes this a semigroup, despite its conventional group name. A [renormalization-group fixed point](../../../../../renormalization-group-fixed-point.md) is invariant after rescaling. At a continuous transition the large-distance theory approaches a critical [renormalization-group fixed point](../../../../../renormalization-group-fixed-point.md); finite [correlation length](../../../../../correlation-length.md) instead eventually flows into an ordinary [thermodynamic phase](../../../../../thermodynamic-phase.md) regime.

Linearize in scaling coordinates $u_i$:

$$
u'_i=b^{y_i}u_i.
$$

For increasing observation [length](../../../../../length.md), $y_i>0$ is relevant and must be tuned, $y_i<0$ is irrelevant, and $y_i=0$ is marginal and needs nonlinear analysis. Discrete multipliers $b^{y_i}$ must be compared with one, not with zero. The stable manifold forms the [critical surface](../../../../../critical-surface.md) after relevant directions have been set to zero.

After subtracting regular additive contributions, ordinary [hyperscaling](../../../../../hyperscaling-relation.md) gives

$$
f_s(t,h)=b^{-d}f_s(b^{y_t}t,b^{y_h}h).
$$

Choosing $b=|t|^{-1/y_t}$ or choosing the field as scale yields

$$
\boxed{\nu=1/y_t,\quad\Delta=y_h/y_t,\quad
2-\alpha=d/y_t,\quad\beta=(d-y_h)/y_t,\quad
\gamma=(2y_h-d)/y_t,\quad\delta=y_h/(d-y_h).}
$$

For a critical two-point function $G(r)\sim r^{-(d-2+\eta)}$, the [order parameter](../../../../../order-parameter.md) [scaling dimension](../../../../../scaling-dimension.md) is $x_m=(d-2+\eta)/2$, and its [conjugate field](../../../../../field-conjugate-to-an-order-parameter.md) has $y_h=d-x_m=(d+2-\eta)/2$. This recovers the Q1 identities while distinguishing the gap exponent $\Delta$ from the field's [scaling dimension](../../../../../scaling-dimension.md) $y_h$.

As a concrete dimensional check, start from a scalar [gradient](../../../../../gradient.md) action. Restoring its coefficient uses $\phi'(x')=b^{(d-2)/2}\phi_<(bx')$, so at the [Gaussian fixed point](../../../../../gaussian-fixed-point.md)

$$
r'=b^2r,\qquad u'=b^{4-d}u,\qquad h'=b^{(d+2)/2}h.
$$

Quartic interactions are relevant below four dimensions. They can produce an interacting [Wilson-Fisher fixed point](../../../../../wilson-fisher-fixed-point.md), whose exponents differ from naive [Gaussian](../../../../../normal-distribution.md) counting. Above four, the quartic coupling is irrelevant at the [Gaussian fixed point](../../../../../gaussian-fixed-point.md) but dangerous for ordered observables: $\phi_0^2=-r/u$ is singular when $u$ is dropped. Thus the simple two-variable [hyperscaling](../../../../../hyperscaling-relation.md) formula is not universal above the [upper critical dimension](../../../../../upper-critical-dimension.md).

Different microscopic systems can flow to the same long-distance [renormalization-group fixed point](../../../../../renormalization-group-fixed-point.md), explaining [universality](../../../../../universality-of-critical-phenomena.md) of exponents and normalized scaling forms. [Critical temperatures](../../../../../critical-temperature.md), metric factors and regular [free energies](../../../../../thermodynamic-free-energy.md) remain nonuniversal. Dimension, [order parameter](../../../../../order-parameter.md) [symmetry](../../../../../symmetry-physics.md), interaction range and additional soft variables constrain the [universality class](../../../../../universality-class.md). Truncations, perturbative expansions and numerics approximate the flow; they must not be confused with the exact elimination definition.[§3.1–§3.3: coarse-graining, scaling, relevance and dangerously irrelevant interactions](../../../../../statistical-field-theory-by-david-tong.md)

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the phase transitions and collective phenomena course of the University of Cambridge](../../../../split.md)
6. [Phase Transitions and Collective Phenomena course of the University of Cambridge](../../../../../phase-transitions-and-collective-phenomena-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
