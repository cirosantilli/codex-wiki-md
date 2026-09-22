<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First fix a convention that is implicit in the source. For the stated free [generating functional](../../../../../generating-functional.md)

$$
Z_0/Z_0[0]=\exp\left(i\bar\eta S\eta+\frac i2J\Delta J\right),
$$

the time-ordered [Wick contractions](../../../../../wick-contraction.md) are $S_F=\langle T\psi\bar\psi\rangle_0=-iS$ and $\Delta_F=\langle TAA\rangle_0=-i\Delta$. These follow directly by the source differentiation rules in part (i). Thus the kernels called [propagators](../../../../../propagator.md) in the question are distinguished here from the contractions, which already include their factors of $i$.

At first order in the [QED](../../../../../quantum-electrodynamics.md) interaction, write $a$ for its integration point. The normalized three-point [correlation function](../../../../../correlation-function.md) is

$$
G_{\nu\alpha\beta}=-ie\int d^4a\,\Delta_{F\nu\mu}(x-a)\gamma^\mu_{rs}\langle T\{\psi_\alpha(y)\bar\psi_\beta(z)\bar\psi_r(a)\psi_s(a)\}\rangle_0+O(e^3).
$$

The zeroth-order term vanishes because the free [photon](../../../../../photon.md) one-point [correlation function](../../../../../correlation-function.md) is zero. There are two nonzero [Wick contractions](../../../../../wick-contraction.md) of the four fields:

$$
\langle T\{\psi_\alpha(y)\bar\psi_\beta(z)\bar\psi_r(a)\psi_s(a)\}\rangle_0
=-S_{F\alpha\beta}(y-z)S_{Fsr}(0)+S_{F\alpha r}(y-a)S_{Fs\beta}(a-z).
$$

The first term pairs the two external [fermions](../../../../../fermion.md) directly and closes the two fields at the interaction into a [fermion loop](../../../../../fermion-loop.md); its minus sign is the [closed fermion loop sign](../../../../../closed-fermion-loop-sign.md). The second term joins the external [fermions](../../../../../fermion.md) through the interaction, giving the connected contribution. This is also obtained by differentiating the quartic term $(i\bar\eta S\eta)^2/2$ in the free [generating functional](../../../../../generating-functional.md); the two choices of bilinear cancel its factor $1/2$.

Insert $S_F=-iS$ and $\Delta_F=-i\Delta$. Since $(-ie)(-i)^3=e$, the result is exactly

$$
\boxed{G_{\nu\alpha\beta}=-e\int d^4a\,\Delta_{\mu\nu}(a-x)\left(\operatorname{tr}[\gamma^\mu S(0)]S_{\alpha\beta}(y-z)-[S(y-a)\gamma^\mu S(a-z)]_{\alpha\beta}\right)+O(e^3).}
$$

The trace term is a disconnected product of a photon [tadpole diagram](../../../../../tadpole-diagram.md) with the free external [fermion](../../../../../fermion.md) [propagator](../../../../../propagator.md); the other term is the connected three-point [correlation function](../../../../../correlation-function.md). In this [QED](../../../../../quantum-electrodynamics.md) calculation the disconnected term vanishes, as established next. With a convention using $S_F,\Delta_F$ themselves as the symbols for the [propagators](../../../../../propagator.md), the equivalent formula retains the prefactor $-ie$ and the connected-minus-trace ordering above; mixing these two conventions would give an erroneous overall phase.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2020](../../../../2020-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
