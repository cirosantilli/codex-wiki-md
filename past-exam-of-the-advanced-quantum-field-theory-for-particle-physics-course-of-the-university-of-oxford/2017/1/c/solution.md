<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Route the [photon](../../../../photon.md) [momentum](../../../../momentum-split.md) as $l$ and the internal [scalar](../../../../scalar-field.md) [momentum](../../../../momentum-split.md) as $l+k$. The [transverse projector](../../../../transverse-projector-of-a-vector-field.md) obeys $P_{\alpha\beta}l^\beta=0$, so the two [cubic vertices](../../../../interaction-term.md) give

$$
(2k+l)^\alpha P_{\alpha\beta}(l)(2k+l)^\beta=4k^\alpha P_{\alpha\beta}(l)k^\beta.
$$

Multiplying the two [vertices](../../../../vertex-graph-theory.md) and propagators therefore gives

$$
\boxed{i\Pi_{\mathrm{ex}}(k)=4e^2\mu^\epsilon\int\frac{d^dl}{(2\pi)^d}\frac{k^2-(k\cdot l)^2/l^2}{l^2[(l+k)^2+m^2]}.}
$$

For the [seagull](../../../../seagull-vertex.md), $g^{\alpha\beta}P_{\alpha\beta}=d-1$. Including the photon-loop [symmetry factor](../../../../feynman-diagram-symmetry-factor.md) gives instead

$$
\boxed{i\Pi_{\mathrm{sg}}=\frac12(-2ie^2)\mu^\epsilon\int\frac{d^dl}{(2\pi)^d}\frac{-i(d-1)}{l^2+m_\gamma^2}
=-(d-1)e^2\mu^\epsilon\int\frac{d^dl}{(2\pi)^d}\frac1{l^2+m_\gamma^2}.}
$$

**The printed [seagull](../../../../seagull-vertex.md) coefficient is twice this result.** The [vertex](../../../../vertex-graph-theory.md)'s factor two differentiates the two [photon](../../../../photon.md) fields; closing them into one line requires the compensating [symmetry factor](../../../../feynman-diagram-symmetry-factor.md). Direct expansion of the [action](../../../../action.md) gives the same check: the [interaction density](../../../../lagrangian-density.md) $-e^2A^2\phi^\dagger\phi$ has one [photon](../../../../photon.md) [contraction](../../../../wick-contraction.md), yielding coefficient $-e^2$, not $-2e^2$. The identical-photon origin of the [vertex](../../../../vertex-graph-theory.md) factor is also explicit in the standard scalar-electrodynamics rules.[§6.5.1, charged scalars: the seagull vertex factor two comes from the two identical photon fields](../../../../quantum-field-theory-by-david-tong.md) This discrepancy does not affect the massless-photon limit in part d or the [ultraviolet pole](../../../../ultraviolet-divergence.md) in part f.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
