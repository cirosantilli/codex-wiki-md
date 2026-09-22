<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

[Newton's first law](../../../../../newton-s-first-law.md) identifies [inertial frames](../../../../../inertial-frame.md) in which a force-free body maintains constant [velocity](../../../../../velocity.md). The second is $\dot{\mathbf P}=\mathbf F_{\rm net}$ for a closed system; for fixed [mass](../../../../../mass.md) it becomes $m\mathbf a=\mathbf F$. The third gives equal and opposite pair [forces](../../../../../force-split.md). Summing the second law over a closed collection cancels internal [force](../../../../../force-split.md) pairs, so total [momentum](../../../../../momentum-split.md) is conserved when the resultant external [force](../../../../../force-split.md) vanishes. A rocket alone is an open variable-mass subsystem, so one must include the [momentum](../../../../../momentum-split.md) carried by exhaust before applying this reasoning.

Choose downward [velocity](../../../../../velocity.md) as positive and write $M(t)=M_0-\alpha t$. During $dt$, exhaust [mass](../../../../../mass.md) $dm=\alpha dt$ leaves downward with [speed](../../../../../speed.md) $v+v_E$ in the surface frame. To first order, [momentum](../../../../../momentum-split.md) balance for rocket plus this exhaust gives

$$
Mv+Mg\,dt=(M-dm)(v+dv)+dm(v+v_E),\qquad \dot v=g-\frac{\alpha v_E}{M_0-\alpha t}.
$$

Integration, with $v(0)=v_0$, yields

$$
\boxed{v(t)=v_0+gt+v_E\log\frac{M_0-\alpha t}{M_0}.}
$$

Setting $g=0$ gives the gravity-free result. This assumes a constant downward relative exhaust [speed](../../../../../speed.md), constant mass-loss rate and $M_0-\alpha t>0$ throughout the burn; the negative logarithm supplies the upward thrust effect.

Height satisfies $\dot h=-v$. Put $u(t)=1-\alpha t/M_0$. Integrating the logarithm and choosing $h(0)=h_0$ gives

$$
\boxed{h(t)=h_0-v_0t-\frac12gt^2+\frac{M_0v_E}{\alpha}[u\log u-u+1].}
$$

Equivalently, the last term is $v_E[t+(M_0-\alpha t)\log u/\alpha]$. Differentiating either form recovers $-v$ and checks the sign.

For this [constant-rate retro-rocket landing](../../../../../constant-rate-retro-rocket-landing.md), at touchdown $u_L=3/4$ and $v_L=0$, hence

$$
\boxed{t_L=\frac{v_E\log(4/3)-v_0}{g}=12.481\,\mathrm s.}
$$

The fuel condition gives $\alpha=M_0/(4t_L)=200.30$ kg/s. Requiring $h(t_L)=0$ then gives

$$
\boxed{h_0=v_0t_L+\frac12gt_L^2-v_Et_L[1+3\log(3/4)]=275.4\,\mathrm m.}
$$

In this burn the downward [speed](../../../../../speed.md) decreases monotonically to zero: the initial thrust acceleration already exceeds [gravity](../../../../../gravity.md) and increases as fuel is consumed. The result is the idealized vertical landing, without atmospheric drag, changing [gravity](../../../../../gravity.md) or a separate terminal burn [phase](../../../../../phase-waves.md).

## ↑ Ancestors (13)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
