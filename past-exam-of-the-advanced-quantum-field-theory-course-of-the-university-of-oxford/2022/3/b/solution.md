<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In [unitary gauge](../../../../unitary-gauge.md) the quadratic [action](../../../../action.md) is that of a [Proca field](../../../../proca-field.md). Use [Minkowski metric](../../../../minkowski-metric.md) $(+---)$ and add a source $J_\mu A^\mu$. [Integration by parts](../../../../integration-by-parts.md), dropping the boundary term, gives

$$
S[A]=\frac12\int d^4x\,A_\mu K^{\mu\nu}A_\nu,\qquad
K^{\mu\nu}=g^{\mu\nu}(\Box+M^2)-\partial^\mu\partial^\nu.
$$

With [Fourier transform](../../../../fourier-transform-split.md) convention $A(x)=\int d^4k\,e^{-ik\cdot x}A(k)/(2\pi)^4$, its kernel is

$$
K^{\mu\nu}(k)=(M^2-k^2)g^{\mu\nu}+k^\mu k^\nu.
$$

For $k^2\ne0$, introduce the [transverse and longitudinal momentum projectors](../../../../transverse-and-longitudinal-momentum-projectors.md)

$$
P_T^{\mu\nu}=g^{\mu\nu}-\frac{k^\mu k^\nu}{k^2},\qquad
P_L^{\mu\nu}=\frac{k^\mu k^\nu}{k^2}.
$$

They obey $P_TP_L=0$ and $P_T+P_L=1$ as mixed-index [linear operators](../../../../linear-operator.md). Hence

$$
K=(M^2-k^2)P_T+M^2P_L,\qquad
K^{-1}=\frac{P_T}{M^2-k^2}+\frac{P_L}{M^2}
=-\frac{g-kk/M^2}{k^2-M^2}.
$$

The final expression is regular at $k^2=0$; the apparent singularities of the individual [projectors](../../../../projection-linear-algebra.md) have cancelled.

The normalized [Gaussian functional integral](../../../../gaussian-functional-integral.md) is evaluated by [completing the square](../../../../completing-the-square.md) with $A\mapsto A+K^{-1}J$:

$$
\frac{Z[J]}{Z[0]}=
\frac{\int\mathcal DA\,\exp\{i(\frac12AKA+JA)\}}{\int\mathcal DA\,\exp\{i\frac12AKA\}}
=\exp\left[-\frac i2\int\frac{d^4k}{(2\pi)^4}J_\mu(-k)(K^{-1})^{\mu\nu}(k)J_\nu(k)\right].
$$

The source-independent [functional determinant](../../../../functional-determinant.md) cancels in this ratio. Two source derivatives insert two fields, so the covariant [Feynman propagator](../../../../feynman-propagator.md) is $iK^{-1}$, with the [Feynman i-epsilon prescription](../../../../feynman-i-epsilon-prescription.md) at the physical pole:

$$
\boxed{D_{\mu\nu}(k)=\frac{-i}{k^2-M^2+i0}\left(g_{\mu\nu}-\frac{k_\mu k_\nu}{M^2}\right),\qquad
D_{\mu\nu}(x-y)=\int\frac{d^4k}{(2\pi)^4}e^{-ik\cdot(x-y)}D_{\mu\nu}(k).}
$$

This is the [Proca propagator](../../../../proca-propagator.md). Its pole residue has the three physical [particle polarizations](../../../../particle-polarization.md) of a massive spin-one [gauge boson](../../../../gauge-boson.md). No additional gauge-fixing term is needed to invert this already gauge-fixed massive quadratic [action](../../../../action.md). In a full interacting [Higgs mechanism](../../../../higgs-mechanism.md) calculation, any field-dependent [unitary gauge](../../../../unitary-gauge.md) measure belongs to the interacting theory; the free quadratic [gauge boson](../../../../gauge-boson.md) [propagator](../../../../propagator.md) above is unaffected.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the advanced quantum field theory course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory course of the University of Oxford](../../../../advanced-quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
