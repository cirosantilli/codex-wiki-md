<h1 id="section-b/b9/solution">Solution</h1>

↑ **Parent:** [B9](../b9.md)

For a fixed set of bodies in an [inertial frame](../../../../../inertial-frame.md), total [linear momentum](../../../../../momentum-split.md) is constant if the resultant external [force](../../../../../force-split.md) vanishes. Summing [Newton's second law](../../../../../newton-s-second-law.md) cancels internal [force](../../../../../force-split.md) pairs by [Newton's third law](../../../../../newton-s-third-law.md). For an open subsystem, [momentum](../../../../../momentum-split.md) carried across its boundary must also be included.

For an [equal-intake-fuel mass-loading rocket](../../../../../equal-intake-fuel-mass-loading-rocket.md), enclose the original craft and the stationary material collected during $dt$. Its initial [momentum](../../../../../momentum-split.md) is $mu$. At the end, the craft has [mass](../../../../../mass.md) $m-\mu\,dt$ and the exhaust has [mass](../../../../../mass.md) $2\mu\,dt$. To first order,

$$
mu=(m-\mu\,dt)(u+du)+2\mu\,dt(u-u_0),
\qquad
\boxed{m\frac{du}{dt}=2\mu u_0-\mu u.}
$$

The first term is [rocket thrust](../../../../../rocket-thrust.md); the second is the [momentum](../../../../../momentum-split.md) cost of collecting stationary matter. It vanishes in the conventional [rocket equation](../../../../../rocket-equation.md), which therefore has no analogous fixed exhaust-speed ceiling in [Newtonian mechanics](../../../../../newtonian-mechanics-split.md). Here the [acceleration](../../../../../acceleration.md) vanishes at **$u_{\max}=2u_0$**; from rest it stays positive below that value while fuel remains. Relativistic limits are outside this model.

For constant $\mu$, [mass conservation](../../../../../mass-conservation.md) gives $m=m_i-\mu t$. Separating variables,

$$
\int_0^u\frac{dw}{2u_0-w}=\int_0^t\frac{\mu\,d\tau}{m_i-\mu\tau}
\quad\Longrightarrow\quad
\frac{2u_0-u}{2u_0}=\frac{m_i-\mu t}{m_i}.
$$

Therefore

$$
\boxed{u(t)=\frac{2\mu u_0}{m_i}t,\qquad \dot u=\frac{2\mu u_0}{m_i}.}
$$

The formal limiting [speed](../../../../../speed.md) would require $t=m_i/\mu$ and zero remaining craft [mass](../../../../../mass.md). A positive [rocket dry mass](../../../../../rocket-dry-mass.md) and finite carried fuel terminate the burn earlier. Maintaining nonzero collection rate even at rest is an idealization explicitly prescribed by the problem.

## ↑ Ancestors (13)

1. [B9](../b9.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
