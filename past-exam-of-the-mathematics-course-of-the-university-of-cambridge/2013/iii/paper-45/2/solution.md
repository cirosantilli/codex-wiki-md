<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use [natural units](../../../../../natural-units.md) and the [Minkowski metric](../../../../../minkowski-metric.md) $(+---)$, and work at tree level with on-shell final particles. Write $M=m_H$ and, for a final particle of mass $m$, $\beta_m=\sqrt{1-4m^2/M^2}$. In the [Higgs boson](../../../../../higgs-boson.md) rest frame the [Lorentz-invariant phase-space measure](../../../../../lorentz-invariant-phase-space-measure.md) reduces to

$$
d\Phi_2=\frac{|\boldsymbol k|}{16\pi^2M}\,d\Omega=\frac{\beta_m}{32\pi^2}\,d\Omega,
\qquad\int d\Phi_2=\frac{\beta_m}{8\pi}.
$$

To obtain this, integrate the momentum delta function to set $\boldsymbol k_2=-\boldsymbol k_1$; the energy delta function is $\delta(M-2\sqrt{k^2+m^2})$, whose radial Jacobian is $E/(2k)$. Hence for an angle-independent final-state [spin sum](../../../../../spin-sum.md) $S=\sum|\mathcal M|^2$,

$$
\Gamma=\frac{\beta_m S}{16\pi M}.
$$

There is no initial-state spin average for a scalar, and neither charged-particle pair here requires an identical-particle factor of $1/2$.

For [Higgs decay to two W bosons](../../../../../higgs-decay-to-two-w-bosons.md), the [Feynman vertex](../../../../../interaction-vertex.md) gives $\mathcal M=(2m_W^2/v)\varepsilon_1^*\!\cdot\varepsilon_2^*$, up to an overall phase. Contracting the two [massive vector polarization sums](../../../../../polarization-sum-for-a-massive-vector-boson.md) gives

$$
S_W=\frac{4m_W^4}{v^2}\left[2+\frac{(k_1\cdot k_2)^2}{m_W^4}\right],\qquad
k_1\cdot k_2=\frac{M^2-2m_W^2}{2}.
$$

The constant 2 follows from $4-1-1$ in the contraction, with the last term coming from the two momentum projectors. Putting $x_W=m_W^2/M^2$, the **full massive result** is

$$
\boxed{\Gamma(H\to W^+W^-)=\frac{M^3}{16\pi v^2}\sqrt{1-4x_W}\,(1-4x_W+12x_W^2),\qquad M\geq2m_W.}
$$

The on-shell two-body width is zero below this threshold; decays through off-shell [W bosons](../../../../../w-boson.md) into more particles are different channels.

For [Higgs decay to a fermion pair](../../../../../higgs-decay-to-a-fermion-pair.md), put $y_b=m_b/v$. The amplitude is $\mathcal M=-y_b\bar u(k_1)v(k_2)$, up to an overall phase and a color Kronecker delta. The [fermion spin sums](../../../../../fermion-spin-sum.md) and [gamma-matrix trace](../../../../../gamma-matrix-trace.md) give

$$
S_b=N_cy_b^2\operatorname{tr}[(\not k_1+m_b)(\not k_2-m_b)]
=4N_cy_b^2(k_1\cdot k_2-m_b^2)
=2N_cy_b^2(M^2-4m_b^2).
$$

The [color multiplicity in a decay width](../../../../../color-multiplicity-in-a-decay-width.md) is $N_c=3$: only a quark and antiquark with matching colors contribute, so the factor is three rather than nine. Therefore

$$
\boxed{\Gamma(H\to\bar b b)=\frac{3m_b^2M}{8\pi v^2}\left(1-\frac{4m_b^2}{M^2}\right)^{3/2},\qquad M\geq2m_b.}
$$

Again the on-shell two-body width is zero below threshold. This is a partonic tree-level answer with every mass retained; [hadronization](../../../../../hadronization.md) is outside the specified calculation.

**The [W boson](../../../../../w-boson.md) channel dominates for large $M$ within the tree-level comparison.** The widths scale as $M^3/v^2$ and $m_b^2M/v^2$, respectively, and

$$
\boxed{\frac{\Gamma(H\to W^+W^-)}{\Gamma(H\to\bar b b)}\sim\frac{M^2}{6m_b^2}.}
$$

The enhancement comes from [longitudinal polarization of a massive vector boson](../../../../../longitudinal-polarization-of-a-massive-vector-boson.md): its polarization vector grows as momentum divided by $m_W$. Thus the longitudinal pair survives the apparently small $m_W^2$ factor in the interaction. At masses so large that the scalar sector is strongly coupled, the tree-level extrapolation itself needs corrections.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
