<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The integral printed in the text can be evaluated without reconstructing Figure 1. Put $A=l^2-m^2+i0$ and $B=(l+k)^2-m^2+i0$, and let $I^\mu$ denote that integral without its factor $\xi$. The numerator contraction responsible for its [covariant gauge](../../../../covariant-gauge.md) dependence is

$$
l_\alpha\left(g^{\alpha\beta}-(1-\xi)\frac{l^\alpha l^\beta}{l^2}\right)(l+2k)_\beta
=\xi(l^2+2l\cdot k).
$$

With the [scalar electrodynamics three-point vertex](../../../../scalar-electrodynamics-three-point-vertex.md) $-ie(p+p')^\mu$, three such vertices, two [scalar propagators](../../../../scalar-propagator.md) and one [photon propagator](../../../../photon-propagator.md) have overall factor $(-ie)^3i^2(-i)=-e^3$. Thus the supplied integrand gives $V_{\mathrm{supplied}}^\mu=-e^3\xi I^\mu$.

First isolate the numerator term $l^2$. Its contribution is

$$
I_0^\mu=\int\frac{d^dl}{(2\pi)^d}\frac{(2l+k)^\mu}{AB}.
$$

Under $l\mapsto-l-k$ the two denominators exchange and the numerator changes sign. A shift-invariant [dimensional regularization](../../../../dimensional-regularization.md) therefore gives $\boxed{I_0^\mu=0}$, including the finite part.

For the remaining numerator $2(l\cdot k)(2l+k)^\mu$, only its term $4l^\mu(l\cdot k)$ contributes to the [ultraviolet pole](../../../../ultraviolet-pole.md). Corrections from expanding the denominators, and the numerator $2k^\mu(l\cdot k)$, are [ultraviolet finite](../../../../ultraviolet-finiteness.md) by [power counting](../../../../power-counting-in-quantum-field-theory.md). Use [auxiliary-mass extraction of ultraviolet poles](../../../../auxiliary-mass-extraction-of-ultraviolet-poles.md) with any $M>0$ rather than literally integrating a massless [scaleless integral](../../../../scaleless-integral.md). [Lorentz covariance](../../../../lorentz-covariance.md) then gives

$$
\begin{aligned}
I^\mu\big|_{\mathrm{UV}}
&=\frac4d k_\nu g^{\mu\nu}\int\frac{d^dl}{(2\pi)^d}\frac1{(l^2-M^2+i0)^2}\bigg|_{\mathrm{UV}}\\
&=iC_\epsilon k^\mu,\\
\boxed{V_{\mathrm{supplied}}^\mu\big|_{\mathrm{UV}}}&=\boxed{-ie^3\xi C_\epsilon k^\mu}.
\end{aligned}
$$

**TODO (source gap):** The algebra of the supplied expression is complete, but its graphical identification with Figure 1(b), including the routing at each internal vertex, cannot be visually verified from the unreadable panel.

The complete [renormalization constant](../../../../renormalization-constant.md) can nevertheless be obtained independently. Here is a short [scalar QED wave-function pole](../../../../scalar-qed-wave-function-pole.md) calculation, to avoid assuming either missing panel's value. For an external [four-momentum](../../../../four-momentum.md) $p$, the exchange contribution to the [scalar self-energy](../../../../scalar-self-energy.md) has numerator

$$
N=(2p-l)^2-(1-\xi)\frac{[(2p-l)\cdot l]^2}{l^2}
=4p^2-4\xi p\cdot l+\xi l^2-4(1-\xi)\frac{(p\cdot l)^2}{l^2}.
$$

Its denominator is $l^2[(p-l)^2-m^2+i0]$. The necessary [ultraviolet poles](../../../../ultraviolet-pole.md), with the measure $d^dl/(2\pi)^d$, are respectively

$$
\int\frac1{l^2D}\bigg|_{\mathrm{UV}}=iC_\epsilon,\quad
\int\frac{l^\mu}{l^2D}\bigg|_{\mathrm{UV}}=\frac{p^\mu}2iC_\epsilon,\quad
\int\frac1D\bigg|_{\mathrm{UV}}=m^2iC_\epsilon,\quad
\int\frac{l^\mu l^\nu}{(l^2)^2D}\bigg|_{\mathrm{UV}}=\frac{g^{\mu\nu}}4iC_\epsilon,
\qquad D=(p-l)^2-m^2+i0.
$$

The first two follow by a [Feynman parameter](../../../../feynman-parameter.md) and a shift of $l$; the third is a [tadpole integral](../../../../tadpole-integral.md); the last follows by the same large-$l$ extraction used above. The [seagull vertex](../../../../seagull-vertex.md) contributes only a [photon](../../../../photon.md) [tadpole integral](../../../../tadpole-integral.md), which is a [scaleless integral](../../../../scaleless-integral.md), and in any case cannot affect the coefficient of $p^2$. Multiplication by the exchange graph's factor $-e^2$ gives the [scalar self-energy](../../../../scalar-self-energy.md) insertion

$$
-i e^2 C_\epsilon[(3-\xi)p^2+\xi m^2].
$$

The kinetic [counterterm](../../../../counterterm.md) $i\delta_2p^2$ therefore requires $\delta_2=e^2(3-\xi)C_\epsilon$. The [scalar QED Ward identity](../../../../scalar-quantum-electrodynamics-ward-identity.md) sets $\delta_1=\delta_2$, so

$$
\boxed{Z_1=1+\frac{e^2(3-\xi)}{16\pi^2\epsilon}+O(e^4).}
$$

Indeed the full unrenormalized [scalar electrodynamics three-point vertex](../../../../scalar-electrodynamics-three-point-vertex.md) has [ultraviolet pole](../../../../ultraviolet-pole.md) $ie^3(3-\xi)C_\epsilon k^\mu$, which is cancelled by $-ie\delta_1k^\mu$. Subtracting the supplied contribution gives the gauge-independent sum stated in part (ii), without assigning either unreadable panel an integrand.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
