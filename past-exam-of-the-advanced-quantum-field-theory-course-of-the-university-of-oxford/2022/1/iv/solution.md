<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Continue the [loop momentum](../../../../loop-momentum.md) to $D=4-\varepsilon$ dimensions, keeping $\operatorname{tr}1=4$ and the external physical [polarization vectors](../../../../polarization-vector.md) four dimensional. Introduce [Feynman parameters](../../../../feynman-parameter.md) $x,y\geq0$, $x+y\leq1$, denoting this integration triangle by $\mathcal T$. Completing the square gives

$$
\frac1{D_0D_1D_2}=2\int_{\mathcal T}dx\,dy\,\frac1{(k^2-\Delta+i0)^3},\qquad
k=l+xp_1-yp_2,\qquad \Delta=m^2-sxy.
$$

Odd terms in $k$ integrate to zero. [Lorentz invariance](../../../../lorentz-invariance.md) of [dimensional regularization](../../../../dimensional-regularization.md) gives $k_\mu k_\nu\mapsto g_{\mu\nu}k^2/D$. The general projected numerator therefore becomes, under the [Feynman integral](../../../../feynman-integral.md),

$$
g_{\mu\nu}\left[\left(\frac AD-C\right)k^2+C(m^2-s/2+sxy)\right]
+(B-Axy)p_{2,\mu}p_{1,\nu}.
$$

Only the $k^2$ term can give an [ultraviolet divergence](../../../../ultraviolet-divergence.md). Define, with the conventional scale factor implicit,

$$
J_n(\Delta)=\mu_R^{\varepsilon}\int\frac{d^Dk}{(2\pi)^D}(k^2-\Delta+i0)^{-n},\qquad
I_2=J_2+\Delta J_3.
$$

The [gamma function](../../../../gamma-function.md) formula gives

$$
J_2=\frac{i}{16\pi^2}\frac2\varepsilon+O(1),\qquad
J_3=-\frac{i}{32\pi^2\Delta}+O(\varepsilon).
$$

Thus the pole of the numerator integral, including $2\int_{\mathcal T}dx\,dy=1$, is

$$
g_{\mu\nu}\left(\frac A4-C\right)\frac{i}{8\pi^2\varepsilon},
\qquad \boxed{A=4C.}
$$

The coefficients $(4,1,1)$ satisfy this condition. A nonzero local divergence would have to be removed by a [counterterm](../../../../counterterm.md). The [Ward identity](../../../../ward-identity.md) forbids a local $hA_\mu A^\mu$ term, and the first electromagnetic [gauge-invariant](../../../../gauge-invariance.md) coupling with one [Higgs boson](../../../../higgs-boson.md) and two [photons](../../../../photon.md) has the form $hF_{\mu\nu}F^{\mu\nu}$, of [engineering dimension](../../../../engineering-dimension.md) five. It is not an independent [counterterm](../../../../counterterm.md) of the [Standard Model](../../../../standard-model-split.md), a [renormalizable quantum field theory](../../../../renormalizable-quantum-field-theory.md). The [top quark](../../../../top-quark.md) contribution is separately electromagnetic [gauge-invariant](../../../../gauge-invariance.md); no additional [W boson](../../../../w-boson.md) [loop Feynman diagram](../../../../loop-feynman-diagram.md) is needed to cancel this pole.

**The finite remainder must still be retained.** For $A=4C$,

$$
\frac AD-C=\frac{C\varepsilon}{4-\varepsilon},\qquad
\lim_{\varepsilon\to0}\left(\frac AD-C\right)I_2=\frac{iC}{32\pi^2}.
$$

Putting $D=4$ before evaluating the divergent [Feynman integral](../../../../feynman-integral.md) would incorrectly set this finite contribution to zero.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [1](../../1.md)
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

## ← Incoming links (1)

- [Solution](../v/solution.md)
