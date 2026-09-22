<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Standard Model](../../../../standard-model-split.md) is a [chiral gauge theory](../../../../chiral-gauge-theory.md): left-chiral quarks and leptons form [SU(2)](../../../../su-2-group.md) weak doublets, while the corresponding right-chiral charged fields are weak singlets. The covariant kinetic term contains $g_W\bar Q_L\gamma^\mu t^aQ_LW_\mu^a$. With $W^\pm=(W^1\mp iW^2)/\sqrt2$, its off-diagonal generators give the [weak charged current](../../../../charged-current.md)

$$
\mathcal L_{\rm cc}\supset\frac{g_W}{\sqrt2}\bar b_L\gamma^\mu V_{tb}^*t_LW_\mu^-
+\mathrm{h.c.}
=\frac{g_W}{2\sqrt2}\bar b\gamma^\mu(1-\gamma^5)V_{tb}^*tW_\mu^-+\mathrm{h.c.}
$$

An overall interaction sign depends on the convention for the [covariant derivative](../../../../covariant-derivative.md) and has no effect on this decay rate. The [chiral projector](../../../../chiral-projector.md) $P_L=(1-\gamma^5)/2$ explains the vector-minus-axial combination. The [Cabibbo-Kobayashi-Maskawa matrix](../../../../cabibbo-kobayashi-maskawa-matrix.md) comes from the different left-handed rotations that diagonalize up- and down-type [fermion mass matrices](../../../../fermion-mass-matrix.md). Set $V_{tb}=1$ and $m_b=0$ as stipulated.

Let $P_{\mu\nu}=-g_{\mu\nu}+p_{3\mu}p_{3\nu}/m_W^2$, the [massive vector polarization sum](../../../../polarization-sum-for-a-massive-vector-boson.md). Sum over final spins and average over the two equally populated initial [top quark](../../../../top-quark.md) spins. The [fermion spin sum](../../../../fermion-spin-sum.md) and the [Dirac adjoint](../../../../dirac-adjoint.md) of the vertex give

$$
\overline{|\mathcal M|^2}
=\frac{g_W^2}{16}P_{\mu\nu}\operatorname{tr}
\left[\not p_2\gamma^\mu(1-\gamma^5)(\not p_1+m_t)\gamma^\nu(1-\gamma^5)\right].
$$

The $m_t$ term vanishes because $(1-\gamma^5)\gamma^\nu(1-\gamma^5)=0$. Anticommuting $\gamma^5$ through the remaining [gamma matrices](../../../../gamma-matrices.md), using $(1-\gamma^5)^2=2(1-\gamma^5)$, then using cyclicity of the [matrix trace](../../../../matrix-trace.md) and the symmetry of $P_{\mu\nu}$ yields

$$
\boxed{\overline{|\mathcal M|^2}
=\frac{g_W^2}{8}P_{\mu\nu}\operatorname{tr}
\left[(1-\gamma^5)\not p_1\gamma^\mu\not p_2\gamma^\nu\right].}
$$

The extra factor two from the chiral algebra compensates the initial spin-average factor. The term with $\gamma^5$ is antisymmetric in $\mu,\nu$ and vanishes upon contraction with $P_{\mu\nu}$. The remaining [gamma-matrix trace](../../../../gamma-matrix-trace.md) is

$$
4\left[p_1^\mu p_2^\nu+p_1^\nu p_2^\mu-(p_1\cdot p_2)g^{\mu\nu}\right].
$$

Its contraction gives

$$
\overline{|\mathcal M|^2}
=\frac{g_W^2}{2}(p_1\cdot p_2)
+\frac{g_W^2}{m_W^2}(p_1\cdot p_3)(p_2\cdot p_3).
$$

Here $p_1=p_2+p_3$, $p_1^2=m_t^2$, $p_2^2=0$ and $p_3^2=m_W^2$, so

$$
p_1\cdot p_2=p_2\cdot p_3=\frac{m_t^2-m_W^2}{2},\qquad
p_1\cdot p_3=\frac{m_t^2+m_W^2}{2}.
$$

Therefore

$$
\overline{|\mathcal M|^2}
=\frac{g_W^2}{4m_W^2}(m_t^2-m_W^2)(m_t^2+2m_W^2).
$$

The [two-body Lorentz-invariant phase space](../../../../two-body-lorentz-invariant-phase-space.md) has rest-frame [momentum](../../../../momentum-split.md) $p^*=(m_t^2-m_W^2)/(2m_t)$. Substitution into $\Gamma=p^*\overline{|\mathcal M|^2}/(8\pi m_t^2)$ gives the [two-body top-quark decay width](../../../../two-body-top-quark-decay-width.md)

$$
\boxed{\Gamma(t\to bW^+)
=\frac{g_W^2m_t^3}{64\pi m_W^2}
\left(1-\frac{m_W^2}{m_t^2}\right)^2
\left(1+2\frac{m_W^2}{m_t^2}\right).}
$$

The squared threshold factor combines the vanishing final [momentum](../../../../momentum-split.md) with the corresponding kinematic factor in the squared [scattering amplitude](../../../../scattering-amplitude.md). The longitudinal [W boson](../../../../w-boson.md) [polarization](../../../../polarization-waves.md) contributes the high-mass enhancement proportional to $m_t^3/m_W^2$. The result is at tree level, for an on-shell [W boson](../../../../w-boson.md) and $m_t>m_W$; finite bottom [mass](../../../../mass.md) and [radiative corrections](../../../../radiative-correction.md) change it. Restoring quark mixing multiplies the width by $|V_{tb}|^2$.

## ↑ Ancestors (13)

1. [2](../2.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the gauge field theory course of the University of Cambridge](../../../split.md)
5. [Gauge Field Theory course of the University of Cambridge](../../../../gauge-field-theory-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
