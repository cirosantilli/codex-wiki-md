<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the paper's positive binding-energy convention $U>0$; the physical [Newtonian gravitational potential energy](../../../../../newtonian-gravitational-potential-energy.md) is $-U$. Assume positive [masses](../../../../../mass.md), an isolated system, and no collision during the time interval under consideration. Differentiate half the scalar [moment of inertia](../../../../../moment-of-inertia.md), $I$, twice:

$$
\dot I=\sum_km_k\boldsymbol r_k\cdot\boldsymbol v_k,
\qquad
\ddot I=\sum_km_kv_k^2+\sum_k\boldsymbol r_k\cdot\boldsymbol F_k.
$$

Group the [force](../../../../../force.md) term into unordered pairs. The [force](../../../../../force.md) on particle $j$ from $k$ is $-Gm_jm_k(\boldsymbol r_j-\boldsymbol r_k)/r_{jk}^3$; the two contributions to the virial sum are therefore

$$
\boldsymbol r_j\cdot\boldsymbol F_{jk}
+\boldsymbol r_k\cdot\boldsymbol F_{kj}
=-\frac{Gm_jm_k}{r_{jk}}.
$$

Adding them proves the instantaneous [virial theorem](../../../../../virial-theorem.md) identity

$$
\boxed{\ddot I=2T-U=T+E,\qquad E=T-U.}
$$

No time average is needed for this form. A vanishing average of $\ddot I$ would require additional boundedness assumptions.

For the [pairwise moment-of-inertia identity](../../../../../pairwise-moment-of-inertia-identity.md), expand the squared pair distances:

$$
\sum_{j<k}m_jm_k|\boldsymbol r_j-\boldsymbol r_k|^2
=M\sum_km_k r_k^2-\left|\sum_km_k\boldsymbol r_k\right|^2.
$$

The last term vanishes in the [centre of mass](../../../../../center-of-mass.md) frame, giving

$$
\boxed{I=\frac1{2M}\sum_{j<k}m_jm_k r_{jk}^2.}
$$

Let $C=\sum_{j<k}m_jm_k$, and label the two smallest [masses](../../../../../mass.md) $m_{(1)},m_{(2)}$. If $r=\min r_{jk}$, every term in $U$ is at most $Gm_jm_k/r$, so $U\leq GC/r$. One pair attains $r$, and its [mass](../../../../../mass.md) product is at least $m_{(1)}m_{(2)}$, so $U\geq Gm_{(1)}m_{(2)}/r$. Hence

$$
\boxed{B_0\leq rU\leq A_0,\qquad
B_0=Gm_{(1)}m_{(2)},\quad A_0=GC.}
$$

These constants show the [minimum-separation binding-energy bounds](../../../../../minimum-separation-binding-energy-bounds.md): inverse binding [energy](../../../../../energy.md) is comparable to the nearest-pair distance, independently of configuration.

Similarly, every separation is at most $R=\max r_{jk}$ and at least one pair attains $R$. The pairwise identity gives the [maximum-separation inertia bounds](../../../../../maximum-separation-inertia-bounds.md)

$$
\boxed{B_1R^2\leq I\leq A_1R^2,\qquad
B_1=\frac{m_{(1)}m_{(2)}}{2M},\quad A_1=\frac C{2M}.}
$$

Both lower bounds rely on actual extremal separations, rather than an arbitrary numerical lower or upper estimate for all the pair distances.

**Negative [energy](../../../../../energy.md) does not imply a positive lower bound on the minimum separation.** The printed request is false if it is meant to exclude close approaches or collisions; the trivial bound $r\geq0$ says nothing of that kind. In fact $E<0$ and $T\geq0$ give $U=T-E\geq|E|$, which, combined with $rU\leq A_0$, proves the [negative-energy minimum-separation upper bound](../../../../../negative-energy-minimum-separation-upper-bound.md)

$$
\boxed{r\leq\frac{A_0}{|E|}.}
$$

This ensures at least one close pair, not confinement of every particle or prevention of collision.

An explicit [negative-energy gravitational collision](../../../../../negative-energy-gravitational-collision.md) is a pair initially at rest with separation $a$. Its total [energy](../../../../../energy.md) is $E=-Gm_1m_2/a<0$. For [reduced mass](../../../../../reduced-mass.md) $\mu=m_1m_2/(m_1+m_2)$, its relative radial equation is

$$
\frac12\mu\dot r^2-\frac{Gm_1m_2}{r}=-\frac{Gm_1m_2}{a},\qquad
\dot r=-\sqrt{2G(m_1+m_2)\left(\frac1r-\frac1a\right)}.
$$

The separation decreases to zero in the finite time

$$
t_{\mathrm{coll}}=\int_0^a\frac{dr}{\sqrt{2G(m_1+m_2)(1/r-1/a)}}
=\pi\sqrt{\frac{a^3}{8G(m_1+m_2)}}.
$$

Before that time the motion is a regular Newtonian solution, yet its separation has no positive infimum. Even at fixed negative [energy](../../../../../energy.md), bound [Kepler orbits](../../../../../kepler-orbit.md) with eccentricity approaching one have arbitrarily small [pericentre distance](../../../../../pericentre-distance.md). Thus a missing [angular momentum](../../../../../angular-momentum.md) or collision-exclusion hypothesis cannot be supplied by the [energy](../../../../../energy.md) sign alone.

For $E>0$, the instantaneous [virial theorem](../../../../../virial-theorem.md) gives $\ddot I=T+E\geq E$. Integrating twice from any regular time $t_0$ gives

$$
I(t)\geq I(t_0)+\dot I(t_0)(t-t_0)+\frac E2(t-t_0)^2.
$$

Using $I\leq A_1R^2$, obtain the [positive-energy linear diameter growth](../../../../../positive-energy-linear-diameter-growth.md) bound

$$
\boxed{R(t)\geq
\sqrt{\frac{I(t_0)+\dot I(t_0)(t-t_0)+E(t-t_0)^2/2}{A_1}}}
$$

whenever the numerator is nonnegative. Consequently, for a solution existing for arbitrarily large future times,

$$
\liminf_{t\to\infty}\frac{R(t)}{t-t_0}\geq\sqrt{\frac E{2A_1}}>0.
$$

This is the precise at-least-linear expansion statement. It does not assert that $R$ is monotone at every instant, nor that all individual particles escape. The large-time conclusion presupposes continued existence of the trajectory; the inequality itself holds on every nonsingular time interval.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
