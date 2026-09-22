<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a constant [unitary matrix](../../../../../unitary-matrix.md) $h$, $\phi'=h\phi$ gives $\phi'^\dagger\phi'=\phi^\dagger h^\dagger h\phi=\phi^\dagger\phi$. Also $\partial_\mu\phi'=h\partial_\mu\phi$, so the kinetic contraction is unchanged. The mass term and the squared norm in the potential are unchanged for the same reason. **The original scalar action has the stated global symmetry.** For a spacetime-dependent $h$, however, $\partial_\mu(h\phi)=h\partial_\mu\phi+(\partial_\mu h)\phi$, and the extra term prevents local invariance of the ordinary-derivative kinetic term.

Choose the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) $D_\mu=\partial_\mu+igA_\mu$, with $A_\mu=A_\mu^\alpha T_\alpha$ Hermitian. Demand $D'_\mu(h\phi)=hD_\mu\phi$. Expanding both sides yields

$$
(\partial_\mu h)\phi+igA'_\mu h\phi=ighA_\mu\phi,
$$

so the necessary [Yang-Mills gauge transformation](../../../../../yang-mills-gauge-transformation.md) is

$$
\boxed{A'_\mu=hA_\mu h^{-1}+\frac ig(\partial_\mu h)h^{-1}.}
$$

Unitarity makes the transformed connection Hermitian. This formula includes the inhomogeneous derivative term; mere conjugation would be insufficient for a local transformation.

Define the [Yang-Mills field strength](../../../../../gauge-field-strength.md) by $[D_\mu,D_\nu]=igF_{\mu\nu}$. Direct expansion gives

$$
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+ig[A_\mu,A_\nu],
\qquad F'_{\mu\nu}=hF_{\mu\nu}h^{-1}.
$$

Choose an orthonormal Hermitian generator basis with $\operatorname{tr}(T_\alpha T_\beta)=\kappa\delta_{\alpha\beta}$. The compact simple Lie algebra has an invariant positive trace metric, so this basis can be chosen; its structure constants are totally antisymmetric. With these conventions a locally invariant dynamical action is

$$
\mathcal L_{\rm inv}=(D^\mu\phi)^\dagger D_\mu\phi-m_0^2\phi^\dagger\phi-\lambda_0(\phi^\dagger\phi)^2
-\frac1{4\kappa}\operatorname{tr}(F_{\mu\nu}F^{\mu\nu}).
$$

Each matter contraction is invariant because $D\phi$ transforms like $\phi$, and the gauge kinetic term is invariant by cyclicity of the trace. It is $-\tfrac14 F^\alpha_{\mu\nu}F_\alpha^{\mu\nu}$ in components. Choosing $\kappa=1/2$ gives the familiar $-\tfrac12\operatorname{tr}F^2$ convention.

Formally introduce a gauge-field source $J_\alpha^\mu$ and a normalized [generating functional](../../../../../generating-functional.md)

$$
Z[J]=\frac1{\mathcal N}\int\mathcal DA\,\mathcal D\phi\,\mathcal D\phi^\dagger
\exp\left(iS_{\rm inv}+i\int d^4x\,J_\alpha^\mu A^\alpha_\mu\right).
$$

A gauge-field [Green function](../../../../../green-s-function.md) is obtained by source differentiation:

$$
\langle T A^{\alpha_1}_{\mu_1}(x_1)\cdots A^{\alpha_r}_{\mu_r}(x_r)\rangle
=\left.\frac1{i^r}\frac{\delta^r Z[J]}{\delta J_{\alpha_1}^{\mu_1}(x_1)\cdots\delta J_{\alpha_r}^{\mu_r}(x_r)}\right|_{J=0}.
$$

Here $\mathcal N$ is the unnormalized integral at zero source, so the normalized functional obeys $Z[0]=1$. This expression needs [gauge fixing](../../../../../gauge-fixing.md): the integral repeats every physical configuration over its whole [gauge orbit](../../../../../gauge-orbit.md), producing an irrelevant but divergent gauge-group volume, and the free gauge kinetic operator has longitudinal zero modes, so it has no inverse propagator on that unrestricted space. Ordinary gauge-field Green functions are gauge-dependent; physical gauge-invariant quantities must be obtained consistently from the gauge-fixed theory.

Use the Lorenz condition $\chi^\alpha[A]=\partial^\mu A^\alpha_\mu$. To keep signs explicit, parametrize a small transformation by $h=1-ig\omega^\alpha T_\alpha+O(\omega^2)$, equivalently the original parameter is $\theta^\alpha=g\omega^\alpha$. The finite transformation above gives the [adjoint gauge variation for a positive-sign covariant derivative](../../../../../adjoint-gauge-variation-for-a-positive-sign-covariant-derivative.md):

$$
\delta A_\mu=\partial_\mu\omega+ig[A_\mu,\omega]
=\mathscr D_\mu\omega,
\qquad
(\mathscr D_\mu\omega)^\alpha=\partial_\mu\omega^\alpha-gf_{\alpha\beta\gamma}A_\mu^\beta\omega^\gamma.
$$

Therefore $\delta\chi^\alpha=\partial^\mu\mathscr D_\mu^{\alpha\beta}\omega^\beta$. Define the [Faddeev-Popov operator](../../../../../faddeev-popov-operator.md) as $\mathcal M=-\partial^\mu\mathscr D_\mu$, absorbing the field-independent minus sign of its determinant into normalization.

In a perturbative gauge patch, with residual zero modes removed by boundary conditions, the [Faddeev-Popov gauge-orbit identity](../../../../../faddeev-popov-gauge-orbit-identity.md) is

$$
1=\Delta_{\rm FP}[A]\int\mathcal D\omega\,
\delta[\chi(A^\omega)-f],\qquad
\Delta_{\rm FP}[A]=\det\mathcal M[A].
$$

It follows by changing coordinates from the gauge parameter to the gauge condition: the functional Jacobian is precisely the determinant of its linearization. Insert the identity into the integral and change variables along the orbit. The action and measure are invariant, so the gauge-group volume factors out and is divided away. Averaging the gauge-slice value $f$ with Gaussian weight $\exp[-i\int f^2/(2\xi)]$ changes the delta-functional restriction to the covariant gauge-fixing term

$$
\boxed{\mathcal L_{\rm gf}=-\frac1{2\xi}(\partial^\mu A^\alpha_\mu)^2.}
$$

The remaining determinant depends on $A$ through $\mathscr D_\mu$. Omitting it while adding only $\mathcal L_{\rm gf}$ would weight different orbits incorrectly.

For a finite matrix $M$, expansion of a [Grassmann integral](../../../../../berezin-integral.md) selects the product containing every $c$ and $\bar c$. Anticommuting the variables into a fixed order attaches the sign of each permutation, giving $\int d\bar c\,dc\,e^{i\bar cMc}$ proportional to $\det M$, with only a matrix-independent phase. The regulated functional version therefore represents the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) as

$$
\det\mathcal M\ \propto\int\mathcal D\bar c\,\mathcal Dc\,
\exp\left(i\int d^4x\,\bar c_\alpha\mathcal M^{\alpha\beta}c_\beta\right).
$$

The independent [Faddeev-Popov ghost fields](../../../../../faddeev-popov-ghost.md) and [antighost fields](../../../../../faddeev-popov-antighost-field.md) obey $c_\alpha c_\beta=-c_\beta c_\alpha$, with the corresponding mixed and antighost anticommutation. A commuting complex Gaussian integral instead gives an inverse determinant, so it cannot supply this Jacobian. The required local ghost term is

$$
\boxed{\mathcal L_{\rm gh}=-\bar c_\alpha\partial^\mu(\mathscr D_\mu c)^\alpha.}
$$

After integration by parts,

$$
\mathcal L_{\rm gh}=(\partial^\mu\bar c_\alpha)(\partial_\mu c_\alpha)
-gf_{\alpha\beta\gamma}(\partial^\mu\bar c_\alpha)A^\beta_\mu c_\gamma.
$$

This exhibits the free ghost kinetic term and the [ghost-gluon vertex](../../../../../ghost-gluon-vertex.md). Ghosts are Grassmann-valued scalar auxiliary fields in the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md), not physical fermionic particles or external asymptotic states. Their loop signs arise from anticommutation. In an Abelian theory the adjoint derivative loses the field-dependent part, so the determinant is field-independent and the ghosts decouple; in the non-Abelian theory they must be retained.

The correctly gauge-fixed source functional thus uses $S_{\rm inv}+S_{\rm gf}+S_{\rm gh}$ and integrates over $A,\phi,\phi^\dagger,c,\bar c$. Expanding its interaction terms gives the gauge, matter and ghost vertices, and differentiating its source functional computes the gauge-field [Green functions](../../../../../green-s-function.md). For example, at non-null momentum the quadratic gauge kernel is

$$
K=-k^2P_T-\frac{k^2}{\xi}P_L,
\qquad K^{-1}=-\frac1{k^2}(P_T+\xi P_L),
$$

where $P_T$ and $P_L$ are the [transverse projector of a vector field](../../../../../transverse-projector-of-a-vector-field.md) and [longitudinal projector of a vector field](../../../../../longitudinal-projector-of-a-vector-field.md). With the Feynman prescription this gives the [gauge-boson propagator](../../../../../gauge-boson-propagator.md)

$$
\langle T A_\mu^\alpha A_\nu^\beta\rangle(k)
=\frac{-i\delta^{\alpha\beta}}{k^2+i0}
\left[\eta_{\mu\nu}-(1-\xi)\frac{k_\mu k_\nu}{k^2+i0}\right].
$$

For the chosen ghost normalization the quadratic kernel is $-\partial^2$, so the [ghost propagator](../../../../../ghost-propagator.md) is $i\delta^{\alpha\beta}/(k^2+i0)$. Redefining the antighost sign changes ghost propagator and vertex signs together, without changing the determinant or physical conclusions. **Gauge fixing requires the accompanying determinant, and its local representation requires anticommuting ghost and antighost fields.** The gauge-orbit argument is local/perturbative: global gauge copies, the [Gribov ambiguity](../../../../../gribov-ambiguity.md), prevent interpreting it as a globally unique gauge slice without further treatment.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
