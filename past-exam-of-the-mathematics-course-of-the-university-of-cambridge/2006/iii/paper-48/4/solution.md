<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In [quantum electrodynamics](../../../../../quantum-electrodynamics.md), [gauge invariance](../../../../../gauge-invariance.md) connects local phase freedom, electric-charge conservation and the restrictions on [photon](../../../../../photon.md) interactions. For definiteness take

$$
\mathcal L=-\frac14F_{\mu\nu}F^{\mu\nu}+\bar\psi(i\gamma^\mu D_\mu-m)\psi,\qquad
D_\mu=\partial_\mu+ieA_\mu,\qquad
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu.
$$

The [gauge transformation](../../../../../gauge-transformation.md)

$$
\psi\mapsto e^{-ie\alpha(x)}\psi,\qquad
\bar\psi\mapsto\bar\psi e^{ie\alpha(x)},\qquad
A_\mu\mapsto A_\mu+\partial_\mu\alpha
$$

has $D_\mu\psi\mapsto e^{-ie\alpha}D_\mu\psi$: the derivative of the local phase cancels the added [gauge potential](../../../../../gauge-field.md). Also $F_{\mu\nu}$ is unchanged because mixed partial derivatives commute. Consequently every term in the [Lagrangian density](../../../../../lagrangian-density.md) is invariant. This derives the [minimal electromagnetic coupling of a Dirac field](../../../../../minimal-electromagnetic-coupling-of-a-dirac-field.md), including the interaction $-e\bar\psi\gamma^\mu\psi A_\mu$. A [fermion](../../../../../fermion.md) mass is compatible with the symmetry, whereas a local Proca [photon](../../../../../photon.md) mass $m_\gamma^2A_\mu A^\mu/2$ is not.

The classical [Maxwell equations](../../../../../maxwell-equations.md) are $\partial_\mu F^{\mu\nu}=j^\nu$, with $j^\nu=e\bar\psi\gamma^\nu\psi$. Taking a divergence gives $\partial_\nu j^\nu=0$ because $F^{\mu\nu}$ is antisymmetric. The same conservation law follows directly from the charged [Dirac equation](../../../../../dirac-equation.md) and its adjoint. For vanishing flux at spatial infinity, $Q=\int d^3x\,j^0$ is conserved. [Gauss law](../../../../../gauss-s-law.md) identifies this charge with the electric flux through a surrounding surface. Particle-antiparticle creation is allowed, but its net [electric charge](../../../../../electric-charge.md) is zero.

Local [gauge invariance](../../../../../gauge-invariance.md) is also a redundancy in the potentials, rather than an extra propagating degree of freedom. The [canonical momentum](../../../../../canonical-momentum.md) of $A_0$ vanishes, and its field equation enforces the [Gauss law constraint in gauge theory](../../../../../gauss-law-constraint-in-gauge-theory.md), $\boldsymbol\nabla\cdot\mathbf E=j^0$. After imposing the constraint and quotienting gauge freedom, a massless [photon](../../../../../photon.md) has **two transverse physical polarizations**. [Gauge transformations](../../../../../gauge-transformation.md) vanishing at the boundary identify equivalent descriptions; constant phase transformations at infinity can act on charged states and generate their conserved charge. This distinction explains why gauge redundancy and [electric charge](../../../../../electric-charge.md) are compatible.

In perturbative [QED](../../../../../quantum-electrodynamics.md), the quadratic [photon](../../../../../photon.md) operator cannot be inverted before [gauge fixing](../../../../../gauge-fixing.md). Adding $-(\partial_\mu A^\mu)^2/(2\xi)$ gives the [covariant gauge](../../../../../covariant-gauge.md) propagator

$$
D_{\mu\nu}(k)=\frac{-i}{k^2+i0}\left[g_{\mu\nu}-(1-\xi)\frac{k_\mu k_\nu}{k^2+i0}\right].
$$

This propagator contains longitudinal and timelike components, but these are not external physical [photon](../../../../../photon.md) states. A [Gupta-Bleuler null-state quotient](../../../../../gupta-bleuler-null-state-quotient.md), or the equivalent [BRST](../../../../../brst-symmetry.md) construction, removes them. In linear [Lorenz gauge](../../../../../lorenz-gauge-condition.md), $\delta(\partial_\mu A^\mu)=\Box\alpha$, so the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) is independent of $A_\mu$ and the [Faddeev-Popov ghost fields](../../../../../faddeev-popov-ghost.md) decouple. This last statement concerns the linear gauge; Abelian [gauge groups](../../../../../gauge-group.md) alone do not guarantee decoupling in a nonlinear gauge condition.

At the quantum level, the vector symmetry gives a [Ward identity](../../../../../ward-identity.md). One way to obtain it is to change variables by a localized phase in a time-ordered correlation function containing $\psi(y)$ and $\bar\psi(z)$. The action variation becomes a current divergence; the two field insertions contribute opposite contact terms, since their charges are opposite. [Fourier transformation](../../../../../fourier-transform.md) turns the divergence into the [photon](../../../../../photon.md) momentum, and amputating the external [fermion](../../../../../fermion.md) propagators turns the two contact terms into the difference of their inverse propagators. With the charge removed from the proper vertex and the overall propagator factor $i$ removed from its inverse, the result is the [proper-vertex Ward-Takahashi identity in QED](../../../../../proper-vertex-ward-takahashi-identity-in-qed.md)

$$
\boxed{k_\mu\Gamma^\mu(p+k,p)=S^{-1}(p+k)-S^{-1}(p).}
$$

At tree level this is simply $k_\mu\gamma^\mu=(\not p+\not k-m)-(\not p-m)$. Between on-shell external spinors, the inverse propagators vanish, so the full physical [scattering amplitude](../../../../../scattering-amplitude.md) satisfies $k_\mu\mathcal M^\mu=0$. Therefore replacing a [photon polarization vector](../../../../../photon-polarization-vector.md) by $\varepsilon_\mu+c k_\mu$ leaves the amplitude unchanged. The identity applies to the complete required sum of diagrams, not necessarily each diagram separately. It also ensures cancellation of the gauge parameter from physical observables when all terms at the chosen perturbative order are included.

For the [photon](../../../../../photon.md) two-point function, the [Ward identity](../../../../../ward-identity.md) implies transverse [photon vacuum polarization](../../../../../photon-vacuum-polarization.md):

$$
k_\mu\Pi^{\mu\nu}(k)=0,\qquad
\Pi^{\mu\nu}(k)=(k^2g^{\mu\nu}-k^\mu k^\nu)\Pi(k^2).
$$

Thus ultraviolet subtraction renormalizes the gauge-invariant kinetic term, rather than requiring a local photon-mass [counterterm](../../../../../counterterm.md). Perturbative unbroken [QED](../../../../../quantum-electrodynamics.md) retains a massless [photon](../../../../../photon.md). Transversality by itself would not exclude a nonlocal massless pole in a different theory; the assertion here includes the perturbative [QED](../../../../../quantum-electrodynamics.md) setting.

Taking $k\to0$ in the proper-vertex identity gives $\Gamma^\mu(p,p)=\partial S^{-1}(p)/\partial p_\mu$. Matching the divergent coefficients of the derivative and vertex terms yields the [Ward identity for QED renormalization constants](../../../../../ward-identity-for-qed-renormalization-constants.md), $Z_1=Z_2$, in a gauge-preserving prescription. If $\psi_0=\sqrt{Z_2}\psi$ and $A_0=\sqrt{Z_3}A$, comparison of the interaction coefficients gives

$$
e_0=\mu_R^\epsilon\frac{Z_1}{Z_2\sqrt{Z_3}}e
=\mu_R^\epsilon Z_3^{-1/2}e\qquad(d=4-2\epsilon).
$$

Hence **[charge renormalization](../../../../../charge-renormalization.md) is fixed by [photon](../../../../../photon.md) [wave-function renormalization](../../../../../wave-function-renormalization.md)**. [Gauge invariance](../../../../../gauge-invariance.md) constrains [counterterms](../../../../../counterterm.md) and relates renormalizations; it does not make the [electric charge](../../../../../electric-charge.md) independent of scale.

The [Soft photon theorem](../../../../../soft-photon-theorem.md) gives another physical manifestation. Attaching a [photon](../../../../../photon.md) of small momentum $k$ to the external charged legs gives the leading factor

$$
\mathcal M_{\mathrm{soft}}=e\mathcal M_{\mathrm{hard}}\sum_i\eta_iQ_i\frac{p_i\cdot\varepsilon}{p_i\cdot k}+O(k^0),
$$

where $Q_i$ is charge in units of $e$ and $\eta_i=+1$ for outgoing and $-1$ for incoming legs. Replacing $\varepsilon$ by $k$ makes this factor proportional to $\sum_i\eta_iQ_i$, which vanishes by [electric charge conservation](../../../../../charge-conservation.md). Massless [photons](../../../../../photon.md) also cause [infrared divergences](../../../../../infrared-divergence.md); physical inclusive measurements combine unresolved real emission with virtual corrections, rather than treating either contribution alone as an observable.

Finally, the vector gauge symmetry of a Dirac [fermion](../../../../../fermion.md) in [QED](../../../../../quantum-electrodynamics.md) is anomaly-free, so it can be maintained by regularization and [renormalization](../../../../../renormalization.md). This must be distinguished from the [axial current](../../../../../axial-current.md): its divergence has explicit mass terms, as in Question 3, and can additionally have a quantum [chiral anomaly](../../../../../chiral-anomaly.md). Conservation of the gauge current does not imply axial-current conservation. The resulting picture is that [gauge invariance](../../../../../gauge-invariance.md) simultaneously organizes the physical [photon](../../../../../photon.md) states, enforces electric-charge conservation and ties together amplitudes and ultraviolet subtractions.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
