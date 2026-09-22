<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use metric $(+,-,-)$ and the paper's normalization. A static multi-vortex solution is a smooth [finite-energy field configuration](../../../../../finite-energy-field-configuration.md) of [Abelian Higgs vortices](../../../../../nielsen-olesen-vortex.md) whose complex [Higgs field](../../../../../higgs-field.md) has winding at spatial infinity and zeros in the plane. In a positive $N$-vortex sector, the zeros have total multiplicity $N$ and the [magnetic flux](../../../../../magnetic-flux.md) is $2\pi N$; they may be separated or coincident. Finite [energy](../../../../../energy.md) requires $|\phi|\to1$, $D_i\phi\to0$ and $B=f_{12}\to0$ at infinity. Then $a_i$ asymptotically compensates the phase [gradient](../../../../../gradient.md), so Stokes' theorem relates flux to the phase winding. The positive [Bogomolny vortex equations](../../../../../bogomolny-vortex-equation.md) describe this same-sign sector; negative flux uses the opposite signs and is not covered by simply mixing positive and negative zero multiplicities.

For the [critically coupled Abelian Higgs field equations](../../../../../critically-coupled-abelian-higgs-field-equations.md), vary $\phi$ and $\bar\phi$ independently. After covariant integration by parts,

$$
\delta_{\bar\phi}S=\int d^3x\left[-\frac12D_\mu D^\mu\phi+\frac14(1-|\phi|^2)\phi\right]\delta\bar\phi.
$$

Thus the scalar equation and its [complex conjugate](../../../../../complex-conjugate.md) are

$$
\boxed{D_\mu D^\mu\phi+\frac12(|\phi|^2-1)\phi=0.}
$$

Varying the [gauge field](../../../../../gauge-field.md) gives $\partial_\mu f^{\mu\nu}\delta a_\nu$ from the Maxwell term. The matter variation is

$$
\delta_a\mathcal L_{\rm matter}=\frac i2\left(\bar\phi D^\nu\phi-\phi\overline{D^\nu\phi}\right)\delta a_\nu=-\operatorname{Im}(\bar\phi D^\nu\phi)\delta a_\nu.
$$

Consequently

$$
\boxed{\partial_\mu f^{\mu\nu}=j^\nu,\qquad j^\nu=\operatorname{Im}(\bar\phi D^\nu\phi).}
$$

These factors use the scalar kinetic coefficient $1/2$; importing the current from a convention with coefficient one would give an incorrect factor two. The current is invariant under [gauge transformations](../../../../../gauge-transformation.md), and its conservation follows from the field equations and antisymmetry of $f^{\mu\nu}$.

For the static purely magnetic solutions take [temporal gauge](../../../../../temporal-gauge.md) $a_0=0$. The scalar equation reduces to

$$
(D_1^2+D_2^2)\phi+\frac12(1-|\phi|^2)\phi=0.
$$

Since $[D_1,D_2]=-iB$, applying $D_1-iD_2$ to the first [Bogomolny vortex equation](../../../../../bogomolny-vortex-equation.md) gives

$$
0=(D_1-iD_2)(D_1+iD_2)\phi=(D_1^2+D_2^2+B)\phi.
$$

The second equation sets $B=(1-|\phi|^2)/2$, proving the scalar equation, including at smooth vortex cores without dividing by $\phi$.

For the spatial gauge equations, put $k_i=\operatorname{Im}(\bar\phi D_i\phi)$. The first equation implies $D_1\phi=-iD_2\phi$, and $\partial_i|\phi|^2=2\operatorname{Re}(\bar\phi D_i\phi)$. Therefore

$$
k_1=-\frac12\partial_2|\phi|^2,\qquad k_2=\frac12\partial_1|\phi|^2.
$$

With the stated metric, $j^i=-k_i$ and the two static Maxwell equations are $\partial_2B=k_1$ and $\partial_1B=-k_2$. Both follow by differentiating $B=(1-|\phi|^2)/2$. The time component is the [Gauss law constraint in gauge theory](../../../../../gauss-law-constraint-in-gauge-theory.md); it is identically satisfied because both the [electric field](../../../../../electric-field.md) and $j^0$ vanish in this static [temporal gauge](../../../../../temporal-gauge.md). Hence

$$
\boxed{\text{both Bogomolny vortex equations imply every static field equation}.}
$$

As an [energy](../../../../../energy.md) check, the [Bogomolny square completion for an Abelian Higgs vortex](../../../../../bogomolny-square-completion-for-an-abelian-higgs-vortex.md) gives $E\geq\pi N$ in this normalization, saturated by these equations. On the plane, the [Abelian Higgs vortex moduli space](../../../../../abelian-higgs-vortex-moduli-space.md) admits arbitrary vortex positions, including coincidence; its static [energy](../../../../../energy.md) is $\pi N$, so there is no position-dependent static potential. Their slow dynamical interactions are a different question.

The [logarithmic form of a Bogomolny vortex](../../../../../logarithmic-form-of-a-bogomolny-vortex.md) is only local away from zeros. Write $\phi=e^{u+i\chi}$ there, with $u=\log|\phi|$. Then

$$
D_i\phi=\phi\left[\partial_i u+i(\partial_i\chi-a_i)\right].
$$

Separating the real and imaginary parts of $(D_1+iD_2)\phi=0$ yields $u_1-\chi_2+a_2=0$ and $\chi_1-a_1+u_2=0$. Hence

$$
\boxed{a_1=\chi_1+u_2,\qquad a_2=\chi_2-u_1,\qquad \mathbf a=\nabla\chi-J\nabla u,}
$$

where $J(v_1,v_2)=(-v_2,v_1)$ is the positive quarter-turn. Under a [gauge transformation](../../../../../gauge-transformation.md), $\chi\mapsto\chi+\omega$ and $\mathbf a\mapsto\mathbf a+\nabla\omega$, as this relation requires.

At regular contour points, the stipulated orthogonality means $\nabla\chi\cdot\nabla u=0$. Since $J\nabla u$ is also perpendicular to $\nabla u$,

$$
\boxed{\mathbf a\cdot\nabla u=0.}
$$

Thus, in that gauge, the [gauge potential](../../../../../gauge-field.md) is tangent to contours of $u$, equivalently contours of $|\phi|$, and is parallel to the phase [gradient](../../../../../gradient.md) wherever that [gradient](../../../../../gradient.md) is nonzero. This is a gauge-dependent statement about the vector potential, not an assertion that the [magnetic field](../../../../../magnetic-field.md) is tangent to these curves, nor that the potential is a pure [gradient](../../../../../gradient.md) or divergence-free. The two [gradient](../../../../../gradient.md) magnitudes are not fixed by contour orthogonality.

On a phase patch $B=\partial_1a_2-\partial_2a_1=-\Delta u$. Combining with the second equation gives $\Delta u+(1-e^{2u})/2=0$ away from the cores. At a zero of multiplicity $n_j$, $u\sim n_j\log|x-X_j|$, and the phase has winding $2\pi n_j$; $u$ is not a finite real smooth field there. Distributionally, the full equality is

$$
\Delta u+\frac12(1-e^{2u})=2\pi\sum_jn_j\delta^{(2)}(x-X_j).
$$

This is the [Taubes equation](../../../../../taubes-equation.md) in the paper's amplitude logarithm, rather than the often-used $\log|\phi|^2=2u$ convention. No single smooth globally defined phase or regular contour description at every zero has been assumed.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 308](../../paper-308-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
