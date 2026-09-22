<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Bogomolny equations](../../../../../bogomolny-equations.md) are first-order equations obtained by expressing a static [energy](../../../../../energy.md) as nonnegative squares plus a term fixed by the [topological charge](../../../../../topological-charge.md). Vanishing of the squares minimizes the [energy](../../../../../energy.md) in that [topological sector](../../../../../topological-sector.md). In particular, the solutions satisfy the full second-order field equations, since their first variation vanishes for compactly supported variations preserving the boundary data. Both monopole and vortex realizations illustrate this mechanism.

For a [Yang-Mills theory](../../../../../yang-mills-theory.md) with gauge group [SU(2)](../../../../../su-2-group.md) and an adjoint [Higgs field](../../../../../higgs-field.md) $\Phi^a$, take the static, purely magnetic [energy](../../../../../energy.md)

$$
E=\int_{\mathbb R^3}\left[\frac12 B_i^aB_i^a+
\frac12(D_i\Phi)^a(D_i\Phi)^a+
\frac{\lambda_H}{4}(\Phi^a\Phi^a-v_H^2)^2\right]d^3x.
$$

Here $B_i^a=\frac12\epsilon_{ijk}F_{jk}^a$, and $e$ is the gauge coupling. In the Bogomolny limit $\lambda_H=0$, retain the boundary condition $|\Phi|\to v_H>0$; it breaks [SU(2)](../../../../../su-2-group.md) to [U(1)](../../../../../circle-group.md) at infinity even though the scalar potential has been removed. The normalized [Higgs field](../../../../../higgs-field.md) on the sphere at infinity defines a map $S^2_\infty\to S^2$ of [topological degree](../../../../../topological-degree.md) $n$. In a consistent magnetic orientation the asymptotic flux is $g_m=4\pi n/e$, and

$$
\int_{S^2_\infty}\Phi^a B_i^a\,dS_i=v_Hg_m.
$$

For example, this equality follows by projecting the asymptotic [gauge curvature](../../../../../gauge-field-strength.md) on the Higgs direction: its flux is the integral of the target-sphere area form, divided by $e$.

The [gauge-theory Bianchi identity](../../../../../gauge-theory-bianchi-identity.md) $D_iB_i=0$ makes the cross term a divergence:

$$
B_i^a(D_i\Phi)^a=\partial_i(\Phi^aB_i^a).
$$

For either sign $s=\pm1$, complete the square:

$$
E=\frac12\int_{\mathbb R^3}|B-sD\Phi|^2d^3x+
s\int_{S^2_\infty}\Phi\cdot B\,dS.
$$

Choosing $s=\operatorname{sgn}n$ gives

$$
\boxed{E\geq\frac{4\pi v_H}{e}|n|,
\qquad B_i=sD_i\Phi\ \text{at equality}.}
$$

These are the [Bogomolny-Prasad-Sommerfield monopole](../../../../../bogomolny-prasad-sommerfield-monopole.md) equations. A nonzero scalar potential would add a positive term; a nontrivial smooth monopole with a core cannot generally saturate this same bound at $\lambda_H>0$. The [Bogomolny monopole equations imply Yang-Mills-Higgs equations](../../../../../bogomolny-monopole-equations-imply-yang-mills-higgs-equations.md): the [Bianchi identity](../../../../../bianchi-identity.md) already gives $D_iD_i\Phi=0$, and the square-completion argument gives stationarity with respect to the gauge field as well.

An explicit charge-one solution is furnished by the [hedgehog ansatz for a monopole](../../../../../hedgehog-ansatz-for-a-monopole.md). To fix its signs, use component conventions $D_i\Phi=\partial_i\Phi-eA_i\times\Phi$ and $F_{ij}=\partial_iA_j-\partial_jA_i-eA_i\times A_j$. With $\rho=ev_Hr$ and $\hat x=x/r$, put

$$
\Phi^a=v_HH(\rho)\hat x^a,\qquad
A_i^a=\frac{1-K(\rho)}{er}\epsilon_{iaj}\hat x^j.
$$

The radial and transverse parts of $D_i\Phi$ are $ev_H^2H'\hat x_i\hat x^a$ and $v_HHK(\delta_{ia}-\hat x_i\hat x^a)/r$. The corresponding parts of $B_i^a$ are $(1-K^2)\hat x_i\hat x^a/(er^2)$ and $-v_HK'(\delta_{ia}-\hat x_i\hat x^a)/r$. Therefore $B=D\Phi$ reduces to

$$
\frac{dK}{d\rho}=-KH,\qquad
\frac{dH}{d\rho}=\frac{1-K^2}{\rho^2}.
$$

The [Prasad-Sommerfield radial monopole solution](../../../../../prasad-sommerfield-radial-monopole-solution.md) is

$$
\boxed{K(\rho)=\frac{\rho}{\sinh\rho},\qquad
H(\rho)=\coth\rho-\frac1\rho.}
$$

Direct differentiation verifies both equations. Near $\rho=0$, $K=1-\rho^2/6+O(\rho^4)$ and $H=\rho/3+O(\rho^3)$, so the apparent angular singularities disappear and the fields are smooth. At infinity $K$ decays exponentially while $H=1-1/\rho+O(e^{-2\rho})$, leaving an Abelian $1/(er^2)$ magnetic field and mass $4\pi v_H/e$.

Translations of this [magnetic monopole](../../../../../magnetic-monopole.md) give three [collective coordinates](../../../../../collective-coordinate-of-a-soliton.md); a residual [U(1)](../../../../../circle-group.md) phase provides another in the framed description, where gauge transformations are fixed at infinity. Multimonopole solutions of a common sign also saturate the linear bound. Their widely separated constituents have position and phase parameters, with no static force: the magnetic repulsion and massless-Higgs attraction cancel in this limit. Relative motion is described at low speeds by the [moduli-space approximation](../../../../../moduli-space-approximation-for-solitons.md). An opposite-sign monopole pair does not solve one common sign of the [Bogomolny equations](../../../../../bogomolny-equations.md) and is not protected by that no-force argument.

For the [Abelian Higgs model](../../../../../abelian-higgs-model.md), a second realization occurs in the plane. Let $\psi$ be a complex [Higgs field](../../../../../higgs-field.md), $D_i=\partial_i-ieA_i$, $B=\partial_1A_2-\partial_2A_1$, and choose the critically coupled static [energy](../../../../../energy.md)

$$
E=\int_{\mathbb R^2}\left[\frac12B^2+|D_i\psi|^2+
\frac{e^2}{2}(|\psi|^2-v_H^2)^2\right]d^2x.
$$

Different conventions for the scalar kinetic coefficient change the numerical coefficients of both the bound and the equations. This normalization gives scalar and gauge masses $\sqrt2ev_H$, explaining the critical balance of their long-distance forces. In three spatial dimensions the planar solutions describe straight strings with this [energy](../../../../../energy.md) per unit length.

Finite [energy](../../../../../energy.md) requires $|\psi|\to v_H$ and $D_i\psi\to0$. On a large circle the Higgs phase winds by $2\pi n$, so the [magnetic flux quantization of an Abelian Higgs vortex](../../../../../magnetic-flux-quantization-of-an-abelian-higgs-vortex.md) gives

$$
\Phi_B=\int B\,d^2x=\oint A_i\,dx^i=\frac{2\pi n}{e}.
$$

Writing $J_i=\operatorname{Im}(\bar\psi D_i\psi)$, expansion and integration by parts give

$$
|D_1\psi|^2+|D_2\psi|^2
=|(D_1+iD_2)\psi|^2+eB|\psi|^2+
\partial_1J_2-\partial_2J_1.
$$

The divergence integrates to zero for the usual localized vortex boundary conditions. Thus the [Bogomolny square completion for an Abelian Higgs vortex](../../../../../bogomolny-square-completion-for-an-abelian-higgs-vortex.md) is

$$
E=\int_{\mathbb R^2}\left[
|(D_1+iD_2)\psi|^2+
\frac12\{B-e(v_H^2-|\psi|^2)\}^2\right]d^2x
+ev_H^2\Phi_B.
$$

For $n\geq0$ the [Bogomolny vortex equations](../../../../../bogomolny-vortex-equation.md) and bound are

$$
\boxed{(D_1+iD_2)\psi=0,\quad
B=e(v_H^2-|\psi|^2),\quad E=2\pi v_H^2n.}
$$

For $n<0$, reverse the sign in both first-order equations and obtain $E=2\pi v_H^2|n|$.

For a rotationally symmetric positive [vortex number](../../../../../vortex-number.md), use $\psi=v_H f(r)e^{in\theta}$ and the physical angular component $A_\theta=na(r)/(er)$. The [Bogomolny vortex equations](../../../../../bogomolny-vortex-equation.md) become

$$
f'=\frac{n(1-a)}r f,\qquad
a'=\frac{e^2v_H^2r}{n}(1-f^2),
$$

with $f(0)=a(0)=0$ and $f(\infty)=a(\infty)=1$. The regular core behaves as $f\sim cr^n$ and $a\sim e^2v_H^2r^2/(2n)$. Linearization at infinity gives exponentially decaying massive tails. Unlike the radial monopole, these planar radial profiles have no elementary closed form in general.

The general multi-vortex solution can be encoded by the [Taubes equation](../../../../../taubes-equation.md). Away from zeros, write $\psi=v_He^{h/2+i\chi}$. The first equation gives

$$
A_1=\frac1e\left(\partial_1\chi+\frac12\partial_2h\right),\qquad
A_2=\frac1e\left(\partial_2\chi-\frac12\partial_1h\right).
$$

At zeros $z_a$ of multiplicity $m_a$, the phase contributes circulation $2\pi m_a$. The second equation becomes, including these [Dirac delta](../../../../../dirac-delta-function.md) terms,

$$
\Delta h+2e^2v_H^2(1-e^h)
=4\pi\sum_a m_a\delta^{(2)}(x-z_a),\qquad h\to0\ \text{at infinity}.
$$

For prescribed zeros the planar existence result gives a solution; the [prescribed-zero construction of planar Abelian Higgs vortices](../../../../../prescribed-zero-construction-of-planar-abelian-higgs-vortices.md) reconstructs smooth fields, with $h=2m_a\log|x-z_a|+O(1)$ near each zero. Uniqueness is visible directly: for two solutions with the same zeros, their nonsingular difference $w$ satisfies $\Delta w=2e^2v_H^2(e^{h_1}-e^{h_2})$. Multiplying by $w$ and integrating gives

$$
-\int|\nabla w|^2d^2x
=2e^2v_H^2\int w(e^{h_1}-e^{h_2})\,d^2x\geq0,
$$

hence $w=0$. The [Abelian Higgs vortex moduli space](../../../../../abelian-higgs-vortex-moduli-space.md) has arbitrary unordered positions of the $n$ zeros, giving $2n$ real position parameters. The saturated [energy](../../../../../energy.md) is independent of their positions, so critically coupled vortices have no static interaction energy. Away from critical coupling this cancellation is lost.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
