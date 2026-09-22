<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The gravitational variable and the fields held fixed in a variation must be specified. For bosonic matter a second-order [metric tensor](../../../../../metric-tensor.md) formulation is sufficient. For spinorial matter a [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) and a [spin connection](../../../../../spin-connection.md) are needed to define the local Lorentz representation and its [covariant derivative](../../../../../covariant-derivative.md). “Second order” refers to a connection already expressed through derivatives of the [vierbein](../../../../../orthonormal-coframe-in-spacetime.md); “first order” treats that connection as an independent variable.

For a [metric tensor](../../../../../metric-tensor.md), a [scalar field](../../../../../scalar-field.md) and an Abelian [gauge field](../../../../../gauge-field.md), consider the [Einstein-Hilbert action](../../../../../einstein-hilbert-action.md) with matter,

$$
S=\int d^4x\,e\left[\frac{R-2\Lambda}{2\kappa^2}-\frac12g^{\mu\nu}\partial_\mu\phi\partial_\nu\phi-V(\phi)-\frac14F_{\mu\nu}F^{\mu\nu}\right],\qquad F=dA.
$$

Here $e=\sqrt{-g}$ and the connection in $R$ is Levi-Civita. The [metric tensor](../../../../../metric-tensor.md) variation uses $\delta e=-eg_{\mu\nu}\delta g^{\mu\nu}/2$ and

$$
\delta R=R_{\mu\nu}\delta g^{\mu\nu}+g^{\mu\nu}\delta R_{\mu\nu},\qquad
\delta R_{\mu\nu}=\nabla_\rho\delta\Gamma^\rho{}_{\mu\nu}-\nabla_\nu\delta\Gamma^\rho{}_{\mu\rho}.
$$

[Metric compatibility](../../../../../metric-compatibility.md) makes the last two terms a divergence. Thus

$$
\delta S=\frac12\int e\left[\kappa^{-2}(G_{\mu\nu}+\Lambda g_{\mu\nu})-T_{\mu\nu}\right]\delta g^{\mu\nu}+\text{matter variations}+\text{boundary},\qquad
T_{\mu\nu}=-\frac2e\frac{\delta S_{\rm matter}}{\delta g^{\mu\nu}}.
$$

Stationarity for arbitrary compactly supported variations gives

$$
\boxed{G_{\mu\nu}+\Lambda g_{\mu\nu}=\kappa^2T_{\mu\nu}.}
$$

Explicitly,

$$
T^{\phi}_{\mu\nu}=\partial_\mu\phi\partial_\nu\phi-g_{\mu\nu}\left[\frac12(\partial\phi)^2+V\right],\qquad
T^{A}_{\mu\nu}=F_{\mu\rho}F_\nu{}^\rho-\frac14g_{\mu\nu}F^2.
$$

[Scalar field](../../../../../scalar-field.md) and gauge-potential variations give $\nabla^2\phi-V'=0$ and $\nabla_\mu F^{\mu\nu}=0$. Their equations imply [stress-energy conservation](../../../../../stress-energy-conservation.md), consistently with the contracted [Bianchi identity](../../../../../bianchi-identity.md). If the boundary [metric tensor](../../../../../metric-tensor.md) is fixed instead of using compactly supported variations, add the [Gibbons–Hawking–York boundary term](../../../../../gibbons-hawking-york-boundary-term.md), $\kappa^{-2}\int_{\partial M}\varepsilon_{\partial M}\sqrt{|h|}K$, with the outward-normal orientation. Fixing the [metric tensor](../../../../../metric-tensor.md) alone does not otherwise remove the normal derivatives of its variation.

For spinorial matter, write $g_{\mu\nu}=e_\mu{}^ae_\nu{}^b\eta_{ab}$ and $\nabla_\mu\chi=\partial_\mu\chi+\omega_{\mu ab}\gamma^{ab}\chi/4$. In the second-order theory set $\omega=\omega(e)$ before varying. A symmetrized Dirac [action](../../../../../action.md), in the same no-$i$, mostly-plus convention as the earlier solutions, is

$$
S_\chi=\int e\left[-\frac12\left(\bar\chi\gamma^\mu\nabla_\mu\chi-(\nabla_\mu\bar\chi)\gamma^\mu\chi\right)-m\bar\chi\chi\right].
$$

Varying $\bar\chi$ and integrating by parts gives $(\not\nabla+m)\chi=0$; varying $\chi$ gives the adjoint equation. The spinor components held fixed in a gravitational variation are components in the [Lorentz frame](../../../../../lorentz-frame.md). Both $\gamma^\mu=e_a{}^\mu\gamma^a$ and $\omega(e)$ vary with the [vierbein](../../../../../orthonormal-coframe-in-spacetime.md). The former gives the canonical stress, and integrating the spin-connection variation supplies its spin-current improvement. On the [Dirac equations](../../../../../dirac-equation.md) the resulting symmetric stress [tensor](../../../../../tensor.md) is

$$
T^\chi_{\mu\nu}=\frac14\left[\bar\chi\gamma_\mu\overleftrightarrow\nabla_\nu\chi+\bar\chi\gamma_\nu\overleftrightarrow\nabla_\mu\chi\right],\qquad
\bar\chi\gamma_\mu\overleftrightarrow\nabla_\nu\chi=\bar\chi\gamma_\mu\nabla_\nu\chi-(\nabla_\nu\bar\chi)\gamma_\mu\chi.
$$

The off-shell expression also contains $g_{\mu\nu}\mathcal L_\chi/e$; this vanishes on the matter equations for the displayed symmetrized [action](../../../../../action.md). Treating the coordinate gamma matrices as fixed while varying the [metric tensor](../../../../../metric-tensor.md) would miss the displayed stress. Local Lorentz invariance removes the independent antisymmetric [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) equation, leaving the symmetric [Einstein field equations](../../../../../einstein-field-equations.md) with this matter source.

In a first-order [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) formulation, $e^a$ and an antisymmetric Lorentz connection $\omega^{ab}$ are independent. Define

$$
T^a=de^a+\omega^a{}_b\wedge e^b,\qquad R^{ab}=d\omega^{ab}+\omega^a{}_c\wedge\omega^{cb},
$$

and use $R(e,\omega)=e_a{}^\mu e_b{}^\nu R_{\mu\nu}{}^{ab}$. The [curvature form of a connection](../../../../../curvature-form.md) variation is $\delta R^{ab}=D_\omega\delta\omega^{ab}$. For the Einstein-Hilbert term, [integration by parts](../../../../../integration-by-parts.md) in form notation gives a connection equation proportional to

$$
\varepsilon_{abcd}\,T^c\wedge e^d=0
$$

when matter has no connection dependence. For an invertible [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) this forces $T^a=0$, so $\omega=\omega(e)$. The [vierbein](../../../../../orthonormal-coframe-in-spacetime.md) equation then becomes the second-order [Einstein field equations](../../../../../einstein-field-equations.md). This applies to the scalar and Maxwell examples: use $F=dA$, which is independent of $\omega$ and remains gauge invariant even if torsion is present.

A [Dirac field](../../../../../dirac-field.md) changes the connection equation. Directly varying its two [covariant derivatives](../../../../../covariant-derivative.md) gives

$$
\delta_\omega\mathcal L_\chi=-\frac e8\bar\chi\{\gamma^\mu,\gamma^{ab}\}\chi\,\delta\omega_{\mu ab}
=-\frac e4\bar\chi\gamma^{\mu ab}\chi\,\delta\omega_{\mu ab}.
$$

Thus its [spin](../../../../../spin.md) density sources totally antisymmetric torsion. This is [Einstein-Cartan theory](../../../../../einstein-cartan-theory.md), and the connection equation is algebraic rather than a propagation equation for an extra field. To see both its solution and its effect, write

$$
\omega_{\mu ab}=\omega(e)_{\mu ab}+K_{\mu ab},\qquad K_{abc}=e_a{}^\mu K_{\mu bc},\qquad B^{abc}=\bar\chi\gamma^{abc}\chi.
$$

For the totally antisymmetric component sourced by this field, the [Ricci scalar](../../../../../ricci-scalar.md) is $R(e,\omega)=R(e)-K_{abc}K^{abc}$ up to a divergence. The other irreducible contorsion components have no spinor source and their connection equations set them to zero. The auxiliary part of the [Lagrangian](../../../../../lagrangian.md) is therefore

$$
\mathcal L_K=-\frac e{2\kappa^2}K_{abc}K^{abc}-\frac e4K_{abc}B^{abc}.
$$

Its algebraic variation gives the [algebraic torsion of a Dirac field](../../../../../algebraic-torsion-of-a-dirac-field.md),

$$
\boxed{K_{abc}=-\frac{\kappa^2}{4}B_{abc},\qquad T_{abc}=-2K_{abc}=\frac{\kappa^2}{2}B_{abc}.}
$$

Here the first index of $K_{abc}$ labels the derivative, and the torsion convention is $T_{abc}=K_{bac}-K_{cab}$; specifying this convention fixes the sign. Eliminating $K$ leaves the second-order effective [action](../../../../../action.md) with contact interaction

$$
\boxed{\mathcal L_{\rm contact}=\frac{e\kappa^2}{32}(\bar\chi\gamma^{abc}\chi)(\bar\chi\gamma_{abc}\chi).}
$$

It is a local axial-current four-fermion interaction. Hence first-order gravity with Dirac [spin](../../../../../spin.md) density is equivalent to torsion-free second-order gravity with this additional interaction. It is not equivalent to simply declaring the [spin connection](../../../../../spin-connection.md) torsion-free and dropping the contact term. In the effective formulation the [Einstein field equations](../../../../../einstein-field-equations.md) have the stress [tensor](../../../../../tensor.md) of the full effective matter [action](../../../../../action.md). Before eliminating the connection, the antisymmetric stress and its [spin](../../../../../spin.md) current are related by the local Lorentz Noether identity.

Finally, the [1.5-order formalism](../../../../../1-5-order-formalism.md) is a convenient way to vary this effective [action](../../../../../action.md). Let $\widehat\omega(e,\chi)$ solve the algebraic connection equation and let $S_2(e,\chi)=S_1(e,\widehat\omega(e,\chi),\chi)$. The chain rule gives

$$
\delta S_2=\left.\frac{\delta S_1}{\delta e}\right|_{\widehat\omega}\delta e+\left.\frac{\delta S_1}{\delta\chi}\right|_{\widehat\omega}\delta\chi+\left.\frac{\delta S_1}{\delta\bar\chi}\right|_{\widehat\omega}\delta\bar\chi+\underbrace{\left.\frac{\delta S_1}{\delta\omega}\right|_{\widehat\omega}}_{0}\delta\widehat\omega.
$$

Thus **vary as in first order, then insert the solved connection**. One does not need to calculate the complicated induced connection variation. This procedure is justified by its connection equation, not by discarding that variation arbitrarily. In [supergravity](../../../../../supergravity.md) the [gravitino](../../../../../gravitino.md) sources a contorsion quadratic in [fermions](../../../../../fermion.md); substituting it generates the four-fermion terms, while the 1.5-order method simplifies the local [supersymmetry](../../../../../supersymmetry-split.md) cancellation through the lower orders considered above.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
