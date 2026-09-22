<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a bosonic quadratic [action](../../../../../../action.md) $S_2=\tfrac12\int\phi K\phi$, [completing the square](../../../../../../completing-the-square.md) in the [generating functional](../../../../../../generating-functional.md) gives $Z_0[J]/Z_0[0]=\exp(-iJK^{-1}J/2)$. Two [functional derivatives](../../../../../../functional-derivative.md) therefore give the [Feynman propagator](../../../../../../feynman-propagator.md) $\Delta=iK^{-1}$, with boundary conditions and a pole prescription included in the inverse. Zero modes must be removed or fixed before an inverse exists.

Take Minkowski metric $\eta=\operatorname{diag}(1,-1,-1,-1)$, Fourier convention $e^{-ikx}$, and the [Yang-Mills field strength](../../../../../../gauge-field-strength.md) $F_{\mu\nu}^a=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a+gf^{abc}A_\mu^bA_\nu^c$. The interaction terms do not contribute to the quadratic [action](../../../../../../action.md). [Integration by parts](../../../../../../integration-by-parts.md) in $-F^a_{\mu\nu}F^{a\mu\nu}/4-(\partial\cdot A^a)^2/(2\alpha)$ yields

$$
S_2=\frac12\int d^dx\,A_\mu^a\left[\eta^{\mu\nu}\Box-(1-\alpha^{-1})\partial^\mu\partial^\nu\right]A_\nu^a.
$$

The color kernel is diagonal. For $k^2\ne0$, use the [projectors](../../../../../../projection-linear-algebra.md) $P_L^{\mu\nu}=k^\mu k^\nu/k^2$ and $P_T^{\mu\nu}=\eta^{\mu\nu}-P_L^{\mu\nu}$. They obey $P_L^2=P_L$, $P_T^2=P_T$, $P_LP_T=0$, so

$$
K^{ab\mu\nu}(k)=-\delta^{ab}k^2(P_T^{\mu\nu}+\alpha^{-1}P_L^{\mu\nu}),\qquad (K^{-1})_{\mu\nu}^{ab}=-\frac{\delta^{ab}}{k^2}(P_{T\mu\nu}+\alpha P_{L\mu\nu}).
$$

Multiplication explicitly gives the identity on both transverse and longitudinal components. Continuing this inverse with the [Feynman propagator](../../../../../../feynman-propagator.md) prescription gives the [gluon propagator](../../../../../../gluon-propagator.md)

$$
\boxed{\Delta_{\mu\nu}^{ab}(x)=\delta^{ab}\int\frac{d^dk}{(2\pi)^d}e^{-ikx}\left[\frac{-i\eta_{\mu\nu}}{k^2+i0}+\frac{i(1-\alpha)k_\mu k_\nu}{(k^2+i0)^2}\right].}
$$

The second term has the causal double-pole prescription. Away from the pole this is the usual $-i\delta^{ab}[\eta_{\mu\nu}-(1-\alpha)k_\mu k_\nu/k^2]/(k^2+i0)$. For $\alpha=1$ it becomes the [Feynman-gauge adjoint propagator](../../../../../../feynman-gauge-adjoint-propagator.md); $\alpha\to0$ gives a transverse [covariant Landau gauge](../../../../../../landau-gauge-quantum-field-theory.md) [propagator](../../../../../../propagator.md).

**The limit $\alpha\to\infty$ removes [gauge fixing](../../../../../../gauge-fixing.md) and has no finite inverse on the full field space.** The longitudinal eigenvalue $-k^2/\alpha$ tends to zero and its inverse diverges. A contraction with conserved external currents kills the longitudinal term, but that does not define a gauge-unfixed [Gaussian integral](../../../../../../gaussian-integral.md). This massless limit is not the massive-vector unitary-gauge limit: here it exposes the unfixed [gauge orbit](../../../../../../gauge-orbit.md) degeneracy.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
