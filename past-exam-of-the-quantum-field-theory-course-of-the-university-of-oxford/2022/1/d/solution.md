<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Continue with the cubic [scalar field theory](../../../../scalar-field-theory-split.md) of [c](../c.md), and use precisely its [counterterm](../../../../counterterm.md) signs. Take $m^2>0$ to separate [ultraviolet divergences](../../../../ultraviolet-divergence.md) from [infrared divergences](../../../../infrared-divergence.md). Make a [Wick rotation](../../../../wick-rotation.md) and impose the rotationally invariant [cutoff regularization](../../../../cutoff-regularization.md) $|q_E|<\Lambda$. Put

$$
C=\frac{\operatorname{area}(S^5)}{2(2\pi)^6}
=\frac1{128\pi^3},\qquad L_\Lambda=\log\frac{\Lambda^2}{m^2},\qquad
I_r=\int_{|q_E|<\Lambda}\frac{d^6q_E}{(2\pi)^6}(q_E^2+m^2)^{-r}.
$$

For example, [spherical coordinates](../../../../spherical-coordinate-system.md) give $I_1=C\int_0^{\Lambda^2} t^2/(t+m^2)\,dt$. Polynomial division and then differentiation with respect to $m^2$ give the divergent parts

$$
\begin{aligned}
I_1\big|_{\mathrm{div}}&=C\left(\frac{\Lambda^4}{2}-m^2\Lambda^2+m^4L_\Lambda\right),\\
I_2\big|_{\mathrm{div}}&=C(\Lambda^2-2m^2L_\Lambda),\qquad
I_3\big|_{\mathrm{div}}=CL_\Lambda.
\end{aligned}
$$

The derivative relations are $I_2=-\partial_{m^2}I_1$ and $I_3=\tfrac12\partial_{m^2}^2I_1$; differentiation also generates finite terms, which are irrelevant here. The first supplied integral identity is consistent with these divergent parts after [Wick rotation](../../../../wick-rotation.md).

**The second supplied expansion is incorrect.** Write $A=p^2-m^2$. Direct multiplication of the two denominators gives $(A+k^2)^2-4(p\cdot k)^2$, so the correct [Taylor expansion](../../../../taylor-expansion.md) is

$$
\frac1{[(p-k)^2-m^2][(p+k)^2-m^2]}
=\frac1{A^2}\left(1-\frac{2k^2}{A}+\frac{4(p\cdot k)^2}{A^2}+O(k^4)\right).
$$

A concrete counterexample is $p=0$, $m=1$, $k=(\epsilon,\mathbf0)$: the exact expression is $(1-\epsilon^2)^{-2}=1+2\epsilon^2+O(\epsilon^4)$, whereas the printed expansion gives $1+\epsilon^2/2+O(\epsilon^4)$. We therefore compute the [self-energy](../../../../self-energy.md) without that identity.

For Euclidean external [momentum](../../../../momentum-split.md) $P$, define the [scalar bubble integral](../../../../scalar-bubble-integral.md)

$$
B(P)=\int\frac{d^6q_E}{(2\pi)^6}
\frac1{(q_E^2+m^2)((q_E+P)^2+m^2)}.
$$

A [Feynman parameter](../../../../feynman-parameter.md) $x$ combines its denominators into one squared denominator with $K=m^2+x(1-x)P^2$. Applying the radial result above and integrating $\int_0^1x(1-x)\,dx=1/6$ yields

$$
B(P)\big|_{\mathrm{div}}
=C\left(\Lambda^2-2m^2L_\Lambda-\frac{P^2}{3}L_\Lambda\right).
$$

One can instead expand with the [ultraviolet cutoff](../../../../ultraviolet-cutoff.md) fixed on the unshifted [loop momentum](../../../../loop-momentum.md): the $P^2$ coefficient of the integrand is $-(q_E^2+m^2)^{-3}+\tfrac23q_E^2(q_E^2+m^2)^{-4}$, using rotational averaging in six dimensions. Its leading radial term is $-1/(3q_E^6)$, giving the same logarithm. Shifting a sharp integration boundary changes finite terms in this [scalar bubble integral](../../../../scalar-bubble-integral.md), and does not change the displayed divergent coefficients.

To fix all signs and [symmetry factors](../../../../feynman-diagram-symmetry-factor.md) together, expand the one-loop [Euclidean effective action](../../../../euclidean-effective-action.md) around a background [scalar field](../../../../scalar-field.md):

$$
\Gamma_{1,E}[\phi]=\frac12\operatorname{Tr}\log(D+g\phi),\qquad D=-\partial_E^2+m^2,
$$



$$
\Gamma_{1,E}[\phi]-\Gamma_{1,E}[0]
=\frac g2\operatorname{Tr}(D^{-1}\phi)
-\frac{g^2}{4}\operatorname{Tr}(D^{-1}\phi D^{-1}\phi)
+\frac{g^3}{6}\operatorname{Tr}(D^{-1}\phi)^3+\cdots.
$$

These terms are the [tadpole diagram](../../../../tadpole-diagram.md), the two-point [bubble diagram](../../../../bubble-diagram.md), and the [triangle Feynman diagram](../../../../triangle-feynman-diagram.md). The [tadpole diagram](../../../../tadpole-diagram.md) has factor $1/2$; the two-point [bubble diagram](../../../../bubble-diagram.md) also has factor $1/2$ after two differentiations with respect to the background [scalar field](../../../../scalar-field.md). The local three-point [interaction vertex](../../../../interaction-vertex.md) is $g^3I_3$. Thus their divergent contributions to the one-, two-, and three-point Euclidean [one-particle irreducible](../../../../one-particle-irreducible-feynman-diagram.md) vertices are respectively

$$
\frac g2 I_1,\qquad -\frac{g^2}{2}B(P),\qquad g^3I_3.
$$

The Euclidean [counterterm Lagrangian](../../../../counterterm-lagrangian.md) is $\delta_Z(\partial_E\phi)^2/2+\delta_m\phi^2/2+\delta_g\phi^3/6+\delta_h\phi+\delta_\mathcal E$. Cancelling each divergent [one-particle irreducible](../../../../one-particle-irreducible-feynman-diagram.md) vertex therefore gives

$$
\boxed{\begin{aligned}
\delta_h\big|_{\mathrm{div}}&=-\frac{Cg}{2}\left(\frac{\Lambda^4}{2}-m^2\Lambda^2+m^4L_\Lambda\right),\\
\delta_m\big|_{\mathrm{div}}&=\frac{Cg^2}{2}(\Lambda^2-2m^2L_\Lambda),\\
\delta_Z\big|_{\mathrm{div}}&=-\frac{Cg^2}{6}L_\Lambda,\\
\delta_g\big|_{\mathrm{div}}&=-Cg^3L_\Lambda.
\end{aligned}}
$$

For example, the two-point sum is $\delta_ZP^2+\delta_m-g^2B(P)/2$ and its divergent coefficients cancel separately. Finite [counterterms](../../../../counterterm.md) depend on the chosen [renormalization conditions](../../../../renormalization-condition.md). The zero-[mass](../../../../mass.md) limit can use a positive subtraction scale in the logarithms after [infrared regularization](../../../../infrared-regularization.md).

If unnormalized [vacuum functionals](../../../../vacuum-functional.md) are retained, specify the determinant measure by

$$
V_{1,E}(0)=\frac12\int_{|q_E|<\Lambda}\frac{d^6q_E}{(2\pi)^6}
\log\frac{q_E^2+m^2}{\mu^2}.
$$

Expanding its radial integrand at large $q_E$ fixes the additional [vacuum energy density](../../../../vacuum-energy-density.md) [counterterm](../../../../counterterm.md):

$$
\boxed{\delta_\mathcal E\big|_{\mathrm{div}}=-\frac C2\left[
\frac{\Lambda^6}{3}\log\frac{\Lambda^2}{\mu^2}-\frac{\Lambda^6}{9}
+\frac{m^2\Lambda^4}{2}-\frac{m^4\Lambda^2}{2}
+\frac{m^6}{3}L_\Lambda\right].}
$$

The purely [mass](../../../../mass.md)-independent terms depend on the determinant normalization. Normalized [Green functions](../../../../green-s-function-split.md) eliminate this entire constant.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
