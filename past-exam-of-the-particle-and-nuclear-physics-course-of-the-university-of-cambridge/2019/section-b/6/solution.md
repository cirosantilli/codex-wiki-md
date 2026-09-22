<h1 id="section-b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

**Conservation laws**. Use [natural units](../../../../natural-units.md) $c=1$ and write $p_i^\mu=(E_i,\mathbf p_i)$ with the $+---$ metric. In the parent's [rest frame](../../../../rest-frame.md), which is the final-state [centre-of-momentum frame](../../../../center-of-momentum-frame.md), $P^\mu=(M,\mathbf0)$. [Four-momentum conservation](../../../../four-momentum-conservation.md) and the [relativistic energy-momentum relation](../../../../energy-momentum-relation.md) give

$$
\boxed{\sum_{i=1}^n E_i=M,\qquad \sum_{i=1}^n\mathbf p_i=\mathbf0,}
\qquad
E_i^2-\mathbf p_i^2=m_i^2,\quad E_i\geq m_i.
$$

A real massless daughter has strictly positive [energy](../../../../energy-split.md). The kinematic threshold is $M\geq\sum_i m_i$; below, no decay satisfying these conditions exists. The endpoint discussion assumes open [phase space](../../../../phase-space.md), $M>\sum_i m_i$, to avoid collapsed threshold configurations.

**Two-body energies**. [Momentum conservation](../../../../momentum-conservation.md) requires $\mathbf p_2=-\mathbf p_1$, so both daughters have the same momentum magnitude $p$. Their on-shell relations imply

$$
E_1^2-p^2=m_1^2,\qquad E_2^2-p^2=m_2^2,
$$

and subtraction eliminates $p$:

$$
(E_1-E_2)(E_1+E_2)=m_1^2-m_2^2.
$$

Since $E_1+E_2=M$, solving the sum and difference equations gives the [relativistic two-body decay](../../../../relativistic-two-body-decay.md) result

$$
\boxed{E_1=\frac{M^2+m_1^2-m_2^2}{2M},\qquad
E_2=\frac{M^2+m_2^2-m_1^2}{2M}.}
$$

As a check, their common momentum magnitude is

$$
p=\frac{\sqrt{[M^2-(m_1+m_2)^2][M^2-(m_1-m_2)^2]}}{2M}
=\frac{\sqrt{\kappa(M^2,m_1^2,m_2^2)}}{2M},
$$

where $\kappa$ is the [Källén function](../../../../kallen-function.md). It vanishes at the massive two-body threshold and is real on the allowed side. If the symbols $M,m_i$ denote [masses](../../../../mass.md) in kilograms rather than rest [energies](../../../../energy-split.md), multiply the displayed energy formulas by $c^2$ and the displayed momentum formula by $c$.

**Minimum energy in three-body decay**. The on-shell inequality already gives $E_1\geq m_1$. For $m_1>0$, the bound is attainable by putting daughter 1 at rest and letting daughters 2 and 3 recoil back to back:

$$
\mathbf p_1=0,\qquad\mathbf p_2=-\mathbf p_3=\mathbf k,\qquad
\sqrt{k^2+m_2^2}+\sqrt{k^2+m_3^2}=M-m_1.
$$

The last equation has a solution because $M-m_1>m_2+m_3$; its left side increases continuously from $m_2+m_3$ to infinity. Thus

$$
\boxed{E_1^{\min}=m_1\quad(c=1),\qquad E_1^{\min}=m_1c^2\quad\text{with units restored}.}
$$

If $m_1=0$, the same formula describes the lower boundary $E_1\to0^+$. It is an [infimum](../../../../infimum.md), not an attained physical zero-energy massless particle: this is a [soft-particle endpoint](../../../../soft-particle-endpoint.md).

**Maximum energy from the recoil mass**. Group daughters 2 and 3 into a recoil system with [four-momentum](../../../../four-momentum.md) $Q=p_2+p_3=P-p_1$ and squared [invariant mass](../../../../invariant-mass.md) $s_{23}=Q^2$. Directly in the parent [rest frame](../../../../rest-frame.md),

$$
s_{23}=(P-p_1)^2=M^2+m_1^2-2ME_1,
\qquad
E_1=\frac{M^2+m_1^2-s_{23}}{2M}.
$$

Maximizing $E_1$ therefore means minimizing the recoil [invariant mass](../../../../invariant-mass.md). This approach does not assume a recoil rest frame when that system is null.

If both recoil daughters have positive [masses](../../../../mass.md), use their pair [rest frame](../../../../rest-frame.md). Their total [energy](../../../../energy-split.md) there is at least $m_2+m_3$, with equality when both are at rest relative to one another. Equivalently, their future-directed [four-velocities](../../../../four-velocity.md) satisfy $p_2\cdot p_3\geq m_2m_3$, giving

$$
s_{23}=m_2^2+m_3^2+2p_2\cdot p_3\geq(m_2+m_3)^2.
$$

Equality means the two recoil daughters have a common [velocity](../../../../velocity.md) in the parent frame: their momenta are parallel and $\mathbf p_2/m_2=\mathbf p_3/m_3$. Daughter 1 recoils in the opposite direction. Hence

$$
\boxed{E_1^{\max}=\frac{M^2+m_1^2-(m_2+m_3)^2}{2M}.}
$$

At this endpoint their total [energy](../../../../energy-split.md) and its sharing are

$$
E_{23}=\frac{M^2-m_1^2+(m_2+m_3)^2}{2M},\qquad
E_2=\frac{m_2}{m_2+m_3}E_{23},\qquad
E_3=\frac{m_3}{m_2+m_3}E_{23}.
$$

These explicitly exhibit a permitted configuration attaining the bound when both recoil [masses](../../../../mass.md) are positive.

If exactly one recoil daughter is massless, say $m_3=0$ and $m_2>0$, work in the [rest frame](../../../../rest-frame.md) of daughter 2. For any positive photon-like daughter energy there,

$$
s_{23}=m_2^2+2m_2E_3^{(2)}>m_2^2.
$$

The lower recoil-mass bound is approached only as $E_3^{(2)}\to0^+$. Thus the same general formula with $m_3=0$ is the **[supremum](../../../../supremum.md)** of $E_1$ for a genuine three-body event, rather than an attained maximum. Interchanging 2 and 3 covers the other mixed case. The distinction is important because the paper's category “at least one has mass” includes this [soft-particle endpoint](../../../../soft-particle-endpoint.md) as well as the attainable two-massive-particle case.

If both recoil daughters are massless, instead compute

$$
s_{23}=2E_2E_3(1-\cos\theta_{23})\geq0.
$$

It can be exactly zero at nonzero $E_2,E_3$ when their momenta are parallel. Then $|\mathbf Q|=E_2+E_3$, and [momentum conservation](../../../../momentum-conservation.md) makes $|\mathbf p_1|=|\mathbf Q|$. Solving $E_1+|\mathbf p_1|=M$ and $E_1^2-|\mathbf p_1|^2=m_1^2$ gives

$$
\boxed{E_1^{\max}=\frac{M^2+m_1^2}{2M},\qquad
|\mathbf p_1|=E_2+E_3=\frac{M^2-m_1^2}{2M}.}
$$

Both recoil daughters can have positive [energies](../../../../energy-split.md): set $E_2=x|\mathbf p_1|$ and $E_3=(1-x)|\mathbf p_1|$ for any $0<x<1$. This endpoint is attained without a soft daughter, even though their combined [four-momentum](../../../../four-momentum.md) is null and has no [rest frame](../../../../rest-frame.md).

Combining the [three-body decay energy endpoints](../../../../three-body-decay-energy-endpoints.md), the closed kinematic range is

$$
\boxed{m_1\leq E_1\leq\frac{M^2+m_1^2-(m_2+m_3)^2}{2M}\quad(c=1).}
$$

For [masses](../../../../mass.md) in ordinary units, multiply both endpoint expressions by $c^2$. Open endpoints occur precisely in the soft limits described above. These bounds specify kinematic possibilities; the [decay amplitude](../../../../decay-amplitude.md) can still vanish at a boundary, so a possible endpoint need not have a nonzero event density.

## ↑ Ancestors (13)

1. [6](../6.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the particle and nuclear physics course of the University of Cambridge](../../../split.md)
5. [Particle and Nuclear Physics course of the University of Cambridge](../../../../particle-and-nuclear-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
