<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use units $\hbar=c=1$, the [Minkowski metric](../../../../../minkowski-metric.md) $\eta_{ab}=\operatorname{diag}(1,-1,-1,-1)$, and the [Fourier transform](../../../../../fourier-transform.md) convention $f(x)=\int d^4p\,e^{-ip\cdot x}\widetilde f(p)/(2\pi)^4$. Here [gamma matrices](../../../../../gamma-matrices.md) satisfy $\{\gamma^a,\gamma^b\}=2\eta^{ab}I_4$, and $\bar\psi=\psi^\dagger\gamma^0$ is the [Dirac adjoint](../../../../../dirac-adjoint.md). A single [Dirac field](../../../../../dirac-field.md) describes both [Electrons](../../../../../electron.md) and [Positrons](../../../../../positron.md); these are the particle and [antiparticle](../../../../../antiparticle.md) sectors of that field.

The free [Maxwell Lagrangian](../../../../../maxwell-lagrangian.md) and [Dirac action](../../../../../dirac-action.md), with a linear [covariant gauge](../../../../../covariant-gauge.md) condition for the [photon](../../../../../photon.md), give

$$
S_0=\int d^4x\left[-\frac14F_{ab}F^{ab}-\frac1{2\alpha}(\partial_aA^a)^2+\bar\psi(i\gamma^a\partial_a-m)\psi\right],\qquad F_{ab}=\partial_aA_b-\partial_bA_a.
$$

Before [gauge fixing](../../../../../gauge-fixing.md), the [Maxwell Lagrangian](../../../../../maxwell-lagrangian.md) has [zero modes in field theory](../../../../../zero-mode-in-field-theory.md) along $A_a\mapsto A_a+\partial_a\lambda$, so its quadratic operator cannot be inverted on all potentials. In the linear [Lorenz gauge](../../../../../lorenz-gauge-condition.md), the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) is $\det\Box$. It is independent of $A$ and may be absorbed into the normalization; the corresponding [Faddeev-Popov ghost fields](../../../../../faddeev-popov-ghost.md) have no interacting vertices in this Abelian linear gauge. A residual [gauge symmetry](../../../../../gauge-invariance.md) is removed by the specified [boundary conditions](../../../../../boundary-condition.md).

The free [generating functional](../../../../../generating-functional.md) is

$$
Z_0[J,\bar\eta,\eta]=\mathcal N\int\mathcal DA\,\mathcal D\bar\psi\,\mathcal D\psi\;
\exp\!\left(iS_0+i\int d^4x\,[J_aA^a+\bar\eta\psi+\bar\psi\eta]\right),\qquad Z_0[0]=1.
$$

The [Dirac field](../../../../../dirac-field.md) variables and their sources are independent [Grassmann fields](../../../../../grassmann-field.md) in this [path integral](../../../../../path-integral.md). They anticommute; replacing them by ordinary commuting fields would give the wrong statistics and the wrong [functional determinant](../../../../../functional-determinant.md). The bosonic [Gaussian functional integral](../../../../../gaussian-functional-integral.md) contributes an inverse square root of a determinant, and the [Grassmann Gaussian integral](../../../../../grassmann-gaussian-integral.md) contributes a determinant. If $K_A$ is the photon quadratic operator and $K_D=i\gamma^a\partial_a-m$, completing the square gives

$$
Z_0=\exp\!\left[-\frac i2\int J K_A^{-1}J-i\int\bar\eta K_D^{-1}\eta\right]
=\exp\!\left[-\frac12\int J D_F J-\int\bar\eta S_F\eta\right].
$$

In the last expression $D_F=iK_A^{-1}$ and $S_F=iK_D^{-1}$ are the [photon propagator](../../../../../photon-propagator.md) and [Dirac propagator](../../../../../dirac-propagator.md), with [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md). The products include the appropriate spacetime integrals and index contractions. [Functional derivatives](../../../../../functional-derivative.md) with respect to $J$, and consistently ordered left or right [Grassmann derivatives](../../../../../grassmann-derivative.md) with respect to the fermionic sources, generate the [time ordering](../../../../../time-ordering.md) of the corresponding fields. In [Feynman gauge](../../../../../feynman-gauge.md), $\alpha=1$, the momentum-space two-point functions are

$$
\boxed{D_F^{ab}(p)=\frac{-i\eta^{ab}}{p^2+i0},\qquad
S_F(p)=\frac{i(\not p+m)}{p^2-m^2+i0}},\qquad \not p=\gamma^ap_a.
$$

The [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md) specifies vacuum boundary conditions rather than an arbitrary inverse of the differential operator.

The covariant [photon propagator](../../../../../photon-propagator.md) uses four potential components. Its [operator formalism](../../../../../operator-formalism.md) counterpart is [Gupta-Bleuler quantization](../../../../../gupta-bleuler-formalism.md): impose $(\partial_aA^a)^{(+)}|\mathrm{phys}\rangle=0$ and take the [Gupta-Bleuler null-state quotient](../../../../../gupta-bleuler-null-state-quotient.md). This leaves a positive physical state space with two transverse [photon](../../../../../photon.md) [polarization vectors](../../../../../polarization-vector.md). The temporal and longitudinal oscillator components occur in intermediate covariant expressions; the [Ward identity](../../../../../ward-identity.md) removes their dependence from physical amplitudes. The free [Dirac field](../../../../../dirac-field.md) uses the [canonical anticommutation relations](../../../../../canonical-anticommutation-relations.md), producing the same [fermionic signs](../../../../../fermionic-sign.md) as its [Grassmann fields](../../../../../grassmann-field.md) in the [path integral](../../../../../path-integral.md).

The [operator-path-integral equivalence](../../../../../operator-path-integral-equivalence.md) can be seen directly with a regulator. Divide time into small intervals and insert complete sets of field-coordinate states for bosons, and resolutions in [fermionic coherent states](../../../../../fermionic-coherent-state.md) for fermions. The bosonic matrix elements produce the phase-space factor $\exp i\sum[\pi\Delta\phi-H\Delta t]$; integrating out the quadratic [canonical momentum](../../../../../canonical-momentum.md) produces the bosonic [action](../../../../../action.md). The [fermionic coherent state](../../../../../fermionic-coherent-state.md) overlaps produce the first-order term $i\psi^\dagger\dot\psi$ and the [Berezin integral](../../../../../berezin-integral.md) measure. Multiplying the short-time kernels recovers the [path integral](../../../../../path-integral.md). Projecting the remote endpoints onto the [Fock vacuum](../../../../../fock-vacuum.md) with an infinitesimal damping selects the same [Feynman propagators](../../../../../feynman-propagator.md) as the [operator formalism](../../../../../operator-formalism.md). Field insertions become [time-ordered products](../../../../../time-ordered-product.md) under this construction. Conversely, their quadratic [generating functional](../../../../../generating-functional.md) obeys the canonical free-field equations and has precisely the oscillator two-point functions, so its higher free correlators agree by the [Wick theorem](../../../../../wick-s-theorem.md). This establishes the equivalence for the regulated free theory and order by order in the [perturbation series](../../../../../perturbation-series.md).

To couple the matter field electromagnetically, promote its global phase symmetry to the local transformation

$$
\psi\mapsto e^{-ie\lambda(x)}\psi,\qquad
\bar\psi\mapsto\bar\psi e^{ie\lambda(x)},\qquad
A_a\mapsto A_a+\partial_a\lambda.
$$

The [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) $D_a=\partial_a+ieA_a$ obeys $D'_a\psi'=e^{-ie\lambda}D_a\psi$. Replacing $\partial_a$ by $D_a$ in the [Dirac action](../../../../../dirac-action.md) therefore gives the invariant matter density

$$
\bar\psi(i\gamma^aD_a-m)\psi
=\bar\psi(i\gamma^a\partial_a-m)\psi-e\bar\psi\gamma^a\psi A_a.
$$

The [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md) is unchanged by the local transformation. Thus the unfixed [quantum electrodynamics](../../../../../quantum-electrodynamics.md) action is [gauge-invariant](../../../../../gauge-invariance.md). The [Dirac current](../../../../../dirac-current.md) $j^a=\bar\psi\gamma^a\psi$ is conserved by the matter equations, and the [Electron](../../../../../electron.md) and [Positron](../../../../../positron.md) excitations carry opposite charges. The added [gauge fixing](../../../../../gauge-fixing.md) density selects a representative and is not itself invariant under arbitrary local transformations; it does not change gauge-invariant observables. At a free fermion vertex,

$$
q_a\gamma^a=(\not p+\not q-m)-(\not p-m).
$$

For external on-shell [Dirac spinors](../../../../../dirac-spinor.md) the corresponding current contraction vanishes. The quantum extension is the [Ward identity](../../../../../ward-identity.md), which makes physical amplitudes insensitive to adding a multiple of the photon [momentum](../../../../../momentum.md) to its [polarization vector](../../../../../polarization-vector.md). A gauge-compatible regularization preserves this vector-current identity.

With $\mathcal L_{\mathrm{int}}=-e\bar\psi\gamma^a\psi A_a$, expand $\exp(i\int\mathcal L_{\mathrm{int}})$ in powers of $e$. A term of order $n$ contains $n$ spacetime integrations and $1/n!$. Applying the [Wick theorem](../../../../../wick-s-theorem.md) pairs the free fields: an $A$-$A$ [Wick contraction](../../../../../wick-contraction.md) supplies a [photon propagator](../../../../../photon-propagator.md), and a $\psi$-$\bar\psi$ [Wick contraction](../../../../../wick-contraction.md) supplies an oriented [Dirac propagator](../../../../../dirac-propagator.md). Each insertion supplies an [interaction vertex](../../../../../interaction-vertex.md). The permutations of contractions cancel the expansion factorials except for the [Feynman-diagram symmetry factor](../../../../../feynman-diagram-symmetry-factor.md). Interchanging [Grassmann fields](../../../../../grassmann-field.md) produces the [fermionic sign](../../../../../fermionic-sign.md), including a minus sign for every closed fermion loop. This is how [Feynman diagrams](../../../../../feynman-diagram.md) arise from expectation values, rather than an extra dynamical assumption.

The [normalized vacuum generating functional](../../../../../normalized-vacuum-generating-functional.md) removes components with no external insertions. In the [operator formalism](../../../../../operator-formalism.md), for an interacting-vacuum expectation value of an inserted product $\mathcal O$, the same cancellation appears as

$$
\langle\Omega|T\mathcal O|\Omega\rangle
=\frac{\langle0|T\{\mathcal O_I\exp(i\int d^4x\,\mathcal L_{\mathrm{int},I})\}|0\rangle}
{\langle0|T\exp(i\int d^4x\,\mathcal L_{\mathrm{int},I})|0\rangle}.
$$

Vacuum projection and the [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md) are implicit. The [linked-cluster theorem](../../../../../linked-cluster-theorem.md) exponentiates all connected [vacuum bubbles](../../../../../vacuum-feynman-diagram.md) into the same factor in numerator and denominator, so it cancels. **Normalize by $Z[0]$ to remove every vacuum component.** This [cancellation of vacuum bubbles](../../../../../cancellation-of-vacuum-bubbles.md) still leaves products of disconnected diagrams that each contain external insertions. If only connected correlators are wanted, differentiate the [connected generating functional](../../../../../connected-generating-functional.md) $W=-i\log[Z[J,\bar\eta,\eta]/Z[0]]$.

The resulting momentum-space [QED Feynman rules](../../../../../qed-feynman-rules.md) for the bare theory can be stated in [Feynman gauge](../../../../../feynman-gauge.md) as follows:

- An internal oriented fermion line of [four-momentum](../../../../../four-momentum.md) $p$ contributes $i(\not p+m)/(p^2-m^2+i0)$.
- An internal [photon](../../../../../photon.md) line contributes $-i\eta_{ab}/(p^2+i0)$.
- A one-photon two-fermion [interaction vertex](../../../../../interaction-vertex.md) contributes $\boxed{-ie\gamma^a}$, with its spinor and photon indices attached to the incident lines.
- Each [interaction vertex](../../../../../interaction-vertex.md) conserves [four-momentum](../../../../../four-momentum.md). With all incident [momenta](../../../../../momentum.md) treated as incoming, include $(2\pi)^4\delta^4(\sum p)$; after using these constraints, integrate every independent loop [four-momentum](../../../../../four-momentum.md) as $\int d^4\ell/(2\pi)^4$.
- Contract the [gamma matrix](../../../../../gamma-matrices.md) and [Dirac propagator](../../../../../dirac-propagator.md) factors in their order along the fermion line. A closed fermion loop has a [trace](../../../../../matrix-trace.md) and a factor $-1$. A relative odd permutation of external fermions also contributes $-1$.
- Divide each labelled diagram by its [Feynman-diagram symmetry factor](../../../../../feynman-diagram-symmetry-factor.md) and sum the allowed diagrams. Omit vacuum components as explained above.
- For an amputated scattering amplitude, an incoming [Electron](../../../../../electron.md) has $u_s(p)$ and an outgoing [Electron](../../../../../electron.md) has $\bar u_s(p)$; an incoming [Positron](../../../../../positron.md) has $\bar v_s(p)$ and an outgoing [Positron](../../../../../positron.md) has $v_s(p)$. An incoming [photon](../../../../../photon.md) has $\epsilon_a(p)$ and an outgoing [photon](../../../../../photon.md) has $\epsilon_a^*(p)$. The external [polarization vectors](../../../../../polarization-vector.md) are physical and transverse, and external [four-momenta](../../../../../four-momentum.md) are on shell. This last step follows from the [LSZ reduction formula](../../../../../lsz-reduction-formula.md) and [amputation of external propagators](../../../../../amputation-of-external-propagators.md); an unamputated correlator keeps its external [quantum field theory propagators](../../../../../propagator.md).

<a id="1/image-an-oriented-electron-line-meets-a-photon-at-the-qed-interaction-vertex"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-301-qed-vertex.png)

**[Figure 1](#1/image-an-oriented-electron-line-meets-a-photon-at-the-qed-interaction-vertex). An oriented electron line meets a photon at the QED interaction vertex**.

The illustrated [interaction vertex](../../../../../interaction-vertex.md) has incoming fermion [momentum](../../../../../momentum.md) $p$, incoming photon [momentum](../../../../../momentum.md) $k$, and outgoing fermion [momentum](../../../../../momentum.md) $p'=p+k$. Its solid-line arrows indicate fermion flow. The [photon](../../../../../photon.md) wavy line has no fermion-flow arrow. **The propagators, the vertex $-ie\gamma^a$, momentum conservation, and the fermionic signs determine the perturbative amplitudes.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 301](../../paper-301-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
