<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [Non-Abelian gauge theory](../../../../../yang-mills-theory.md) describes fields with a local redundancy, not an independent physical degree of freedom for each component of its [gauge field](../../../../../gauge-field.md). Take a compact [gauge group](../../../../../gauge-group.md) with Hermitian generators $T^a$ and [Lie algebra structure constants](../../../../../structure-constant-of-a-lie-algebra.md) defined by $[T^a,T^b]=if^{abc}T^c$. In a mostly-plus [metric signature](../../../../../metric-signature.md), the pure [Yang-Mills theory](../../../../../yang-mills-theory.md) has

$$
\mathcal L_{\rm YM}=-\frac14F^a_{\mu\nu}F^{a\mu\nu},\qquad F^a_{\mu\nu}=\partial_\mu A^a_\nu-\partial_\nu A^a_\mu+g f^{abc}A^b_\mu A^c_\nu.
$$

With the matter [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) $D_\mu=\partial_\mu-igA_\mu$, a finite [gauge transformation](../../../../../gauge-transformation.md) acts as $A_\mu\mapsto UA_\mu U^{-1}-(i/g)(\partial_\mu U)U^{-1}$. Expanding $U=e^{ig\omega^aT^a}$ gives

$$
\delta A^a_\mu=(D_\mu\omega)^a=\partial_\mu\omega^a+g f^{abc}A^b_\mu\omega^c.
$$

The [Yang-Mills action](../../../../../yang-mills-action.md) is constant along each [gauge orbit](../../../../../gauge-orbit.md). Consequently a naive [functional integral](../../../../../functional-measure.md) $\int\mathcal DA\,e^{iS[A]}$ repeatedly integrates the same physical configuration and contains the infinite formal volume of the local [gauge group](../../../../../gauge-group.md). At quadratic order the same problem appears as noninvertibility: the free kinetic operator annihilates $A_\mu=\partial_\mu\omega$, so no unique [gauge-boson propagator](../../../../../gauge-boson-propagator.md) exists. In canonical language the [Gauss law constraint in gauge theory](../../../../../gauss-law-constraint-in-gauge-theory.md) and the absence of an independent momentum for the time component show that the field components cannot all be independent oscillators. In covariant quantization, time-like and longitudinal polarizations must not be counted as additional physical states.

The [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) implements a local quotient by the [gauge orbit](../../../../../gauge-orbit.md). Choose $G^a[A]=\partial^\mu A^a_\mu$ and first impose $G^a[A]=f^a(x)$ for a specified function $f$. This is the [Lorenz gauge](../../../../../lorenz-gauge-condition.md) condition when $f=0$. Its infinitesimal change is

$$
\delta G^a=\partial^\mu(D_\mu\omega)^a,\qquad (D_\mu)^{ab}=\delta^{ab}\partial_\mu+g f^{acb}A^c_\mu.
$$

The direct [Faddeev-Popov operator](../../../../../faddeev-popov-operator.md) is therefore $M_0^{ab}=\partial^\mu(D_\mu)^{ab}$. Locally, if the condition cuts each orbit once and residual zero modes have been removed by boundary conditions, changing variables from $\omega$ to $G[A^\omega]-f$ proves the [Faddeev-Popov gauge-orbit identity](../../../../../faddeev-popov-gauge-orbit-identity.md)

$$
1=\Delta_{\rm FP}[A]\int\mathcal D\omega\,\delta\big(G[A^\omega]-f\big),\qquad \Delta_{\rm FP}[A]=\det M_0[A].
$$

The determinant is the [functional Jacobian](../../../../../functional-jacobian.md) of this change of variables. A finite-dimensional version is $\int d\omega\,\delta(G(\omega)-f)=1/|\det(\partial G/\partial\omega)|$ near a unique root; the perturbative determinant has a fixed sign or phase, absorbed into normalization. This is the same change-of-variables mechanism used in [Bastianelli's derivation of the Faddeev–Popov construction](https://www-th.bo.infn.it/people/bastianelli/AdQFT-2-Path-integral-and-gauge-fixing-24-25.pdf).

Insert the identity into the normalized [functional integral](../../../../../functional-measure.md) for a [gauge-invariant](../../../../../gauge-invariance.md) observable $\mathcal O[A]$:

$$
Z\langle\mathcal O\rangle=\frac1{\operatorname{Vol}\mathcal G}\int\mathcal DA\,\mathcal O[A]e^{iS[A]}\Delta_{\rm FP}[A]\int\mathcal D\omega\,\delta(G[A^\omega]-f).
$$

For each fixed $\omega$, change the integration variable from $A$ to $A^\omega$. The action, observable and measure are invariant, and the determinant is the orbit Jacobian at the resulting gauge slice. The integrand is now independent of the separately integrated orbit parameter. Its integral is $\operatorname{Vol}\mathcal G$, canceling the denominator. Thus, up to normalization,

$$
Z\langle\mathcal O\rangle=\int\mathcal DA\,\Delta_{\rm FP}[A]\delta(G[A]-f)\,\mathcal O[A]e^{iS[A]}.
$$

This assumes an anomaly-free measure and a local perturbative gauge slice; it is not an assertion of a globally unique representative on every [gauge orbit](../../../../../gauge-orbit.md).

Average over $f$ with weight $\exp[-i\int d^4x\,f^af^a/(2\xi)]$. The delta functional sets $f=G[A]$, so the average produces the [covariant gauge](../../../../../covariant-gauge.md) term

$$
\mathcal L_{\rm gf}=-\frac1{2\xi}(\partial^\mu A^a_\mu)^2.
$$

Next represent the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) by a [Grassmann Gaussian integral](../../../../../grassmann-gaussian-integral.md). Choose $M=-M_0=-\partial^\mu D_\mu$; changing $M_0$ to $-M_0$ changes the regulated determinant by a field-independent factor that is absorbed in normalization. For a [Faddeev-Popov ghost field](../../../../../faddeev-popov-ghost.md) $c$ and independent [antighost field](../../../../../faddeev-popov-antighost-field.md) $\bar c$,

$$
\det M\ \propto\ \int\mathcal D\bar c\,\mathcal Dc\,\exp\left(i\int d^4x\,\bar c^a M^{ab}c^b\right).
$$

To see why it is a determinant rather than its reciprocal, diagonalize a finite-dimensional quadratic form formally: for each Grassmann pair only the term proportional to $\bar c_jc_j$ survives integration, supplying one eigenvalue. Multiplying the surviving eigenvalues gives $\det M$, with an overall factor of $i$ per pair. The functional version is defined with the same regulator as the rest of the theory.

Combining these steps gives the **gauge-fixed Yang–Mills Lagrangian**

$$
\boxed{\mathcal L_{\rm tot}=-\frac14F^a_{\mu\nu}F^{a\mu\nu}-\frac1{2\xi}(\partial^\mu A^a_\mu)^2-\bar c^a\partial^\mu(D_\mu c)^a.}
$$

This is the [gauge-fixed Yang-Mills Lagrangian in a covariant gauge](../../../../../gauge-fixed-yang-mills-lagrangian-in-a-covariant-gauge.md). Integrating its ghost term by parts gives

$$
\mathcal L_{\rm gh}=(\partial^\mu\bar c^a)(\partial_\mu c^a)+g f^{abc}(\partial^\mu\bar c^a)A^b_\mu c^c.
$$

The second term is the [ghost-gluon vertex](../../../../../ghost-gluon-vertex.md) in the antighost convention chosen here. The [Faddeev-Popov ghosts](../../../../../faddeev-popov-ghost.md) are anticommuting Lorentz scalars introduced to represent a determinant; they are not extra asymptotic particles. A closed [ghost loop](../../../../../ghost-loop.md) has a minus sign from their [Grassmann parity](../../../../../grassmann-parity.md). In a [Non-Abelian gauge theory](../../../../../yang-mills-theory.md) the determinant depends on $A$, so these loops are essential. In an Abelian gauge theory $D_\mu$ in the adjoint sector reduces to $\partial_\mu$, the determinant is field independent, and its ghost sector decouples.

The quadratic [gauge field](../../../../../gauge-field.md) kernel at non-null momentum is

$$
K^{\mu\nu}_{ab}(k)=\delta_{ab}\left[-k^2\eta^{\mu\nu}+(1-\xi^{-1})k^\mu k^\nu\right].
$$

Define the mixed-index [longitudinal projector of a vector field](../../../../../longitudinal-projector-of-a-vector-field.md) $P_L{}^\mu{}_\nu=k^\mu k_\nu/k^2$ and [transverse projector of a vector field](../../../../../transverse-projector-of-a-vector-field.md) $P_T=1-P_L$. The kernel is $-k^2(P_T+\xi^{-1}P_L)$ and hence has inverse $-k^{-2}(P_T+\xi P_L)$. Multiplying by $i$ gives the [gauge-boson propagator](../../../../../gauge-boson-propagator.md), off its poles,

$$
\boxed{D^{ab}_{\mu\nu}(k)=-\frac{i\delta^{ab}}{k^2}\left[\eta_{\mu\nu}-(1-\xi)\frac{k_\mu k_\nu}{k^2}\right].}
$$

The vacuum [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md) completes this off-pole formula; with the mostly-plus convention its physical transverse denominator is $k^2-i0$. The choice $\xi=1$ is [Feynman gauge](../../../../../feynman-gauge.md); $\xi\to0$ is [covariant Landau gauge](../../../../../landau-gauge-quantum-field-theory.md). The invertible quadratic kernel supplies perturbation theory, while the ghost determinant ensures the gauge-orbit measure has been accounted for.

The consistency of the unphysical sector is organized by [BRST symmetry](../../../../../brst-symmetry.md). Introduce a bosonic [Nakanishi-Lautrup field](../../../../../nakanishi-lautrup-field.md) $B^a$ and a [left-acting BRST differential](../../../../../left-acting-brst-differential.md)

$$
sA^a_\mu=(D_\mu c)^a,\qquad sc^a=-\frac g2f^{abc}c^bc^c,\qquad s\bar c^a=B^a,\qquad sB^a=0.
$$

The [graded Leibniz rule](../../../../../graded-leibniz-rule.md) and the [Jacobi identity](../../../../../jacobi-identity.md) give $s^2=0$: for example $s^2A=D(sc)+g[Dc,c]=0$ since $D[c,c]=2[Dc,c]$, and $s^2c$ vanishes by the [graded Jacobi identity](../../../../../graded-jacobi-identity.md). Nilpotence on $\bar c$ and $B$ is immediate. Using the odd [antighost field](../../../../../faddeev-popov-antighost-field.md), the same [graded Leibniz rule](../../../../../graded-leibniz-rule.md) gives

$$
s\left[\bar c^a\left(G^a+\frac\xi2B^a\right)\right]=B^aG^a+\frac\xi2B^aB^a-\bar c^a\partial^\mu(D_\mu c)^a.
$$

Eliminating $B^a$ by its algebraic field equation $B^a=-G^a/\xi$ recovers the displayed gauge-fixing and ghost terms. Thus they are [BRST-exact](../../../../../brst-exact-operator.md) together, and the total action preserves [BRST symmetry](../../../../../brst-symmetry.md). At the level of states, the [BRST charge](../../../../../brst-charge.md) $Q$ implements physical states as the ghost-number-zero [BRST cohomology](../../../../../brst-cohomology.md) $\ker Q/\operatorname{im}Q$. This prescription removes longitudinal, time-like and ghost excitations from physical amplitudes while allowing them on internal lines. For a [BRST-closed](../../../../../brst-closed-operator.md) observable, changing $\xi$ inserts $s(\bar c^aB^a/2)$; its expectation vanishes by the BRST change-of-variables identity when the measure preserves the symmetry. This explains the independence of physical quantities from the arbitrary gauge parameter.

Finally, a local condition such as [Lorenz gauge](../../../../../lorenz-gauge-condition.md) can have several solutions on the same [gauge orbit](../../../../../gauge-orbit.md), the [Gribov ambiguity](../../../../../gribov-ambiguity.md). The preceding [Faddeev-Popov gauge-orbit identity](../../../../../faddeev-popov-gauge-orbit-identity.md) and perturbative [gauge fixing](../../../../../gauge-fixing.md) construction apply in a neighborhood where the linearized operator is invertible after residual modes are excluded. They resolve perturbative gauge overcounting and supply consistent covariant [Feynman rules](../../../../../feynman-rule.md); they do not by themselves prove a globally unique nonperturbative gauge fixing.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
