<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The authoritative PDF has $m_Z^2/v$, not the dimensionally incorrect $m_Z^2/v^2$ in the TeX conversion. The two identical [Z bosons](../../../../../../z-boson.md) give the vertex factor two, so the [scattering amplitude](../../../../../../scattering-amplitude.md) for the decay is

$$
\mathcal M=\frac{2m_Z^2}{v}\,\epsilon_1^*\cdot\epsilon_2^*,
$$

up to an irrelevant overall phase. Apply the [massive vector polarization sum](../../../../../../polarization-sum-for-a-massive-vector-boson.md), identifying the hint's $M_Z$ with $m_Z$:

$$
\sum_{s_1,s_2}|\epsilon_1\cdot\epsilon_2|^2=\left(-g_{\mu\nu}+\frac{k_{1\mu}k_{1\nu}}{m_Z^2}\right)\left(-g^{\mu\nu}+\frac{k_2^\mu k_2^\nu}{m_Z^2}\right)=2+\frac{(k_1\cdot k_2)^2}{m_Z^4}.
$$

Since $k_1\cdot k_2=(m_H^2-2m_Z^2)/2$, putting $x=m_Z^2/m_H^2$ gives

$$
\sum_{\mathrm{spins}}|\mathcal M|^2=\frac{m_H^4}{v^2}(1-4x+12x^2).
$$

No initial-spin average is needed for a [Higgs boson](../../../../../../higgs-boson.md). In its rest frame the two-body momentum is $|\boldsymbol k|=(m_H/2)\sqrt{1-4x}$. Integrating the energy and momentum delta functions in the [Lorentz-invariant phase-space measure](../../../../../../lorentz-invariant-phase-space-measure.md) gives $d\Phi_2=\sqrt{1-4x}\,d\Omega/(32\pi^2)$, hence $\int d\Phi_2=\sqrt{1-4x}/(8\pi)$.

The printed generic width formula treats the daughters as labelled. Here the [identical final-state symmetry factor](../../../../../../identical-particle-factor-in-a-final-state-phase-space-integral.md) is $1/2!$, without which the same physical configuration is counted twice. Thus the [Higgs decay to two Z bosons](../../../../../../higgs-decay-to-two-z-bosons.md) has

$$
\boxed{\Gamma(H\to ZZ)=\frac{m_H^3}{32\pi v^2}\sqrt{1-4x}(1-4x+12x^2),\qquad m_H>2m_Z.}
$$

Equivalently, $1/v^2=\sqrt2G_F$ gives the prefactor $G_Fm_H^3/(16\sqrt2\pi)$. The threshold limit is zero and the large-mass limit is $m_H^3/(32\pi v^2)$. The additional factor for identical daughters is a required specialization of the PDF's generic phase-space formula, not an extra factor in the vertex.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
