<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The first massless level of a [closed string](../../../../../../closed-string.md) contains a spin-two field, an antisymmetric two-form and a scalar: the [graviton](../../../../../../graviton.md), [Kalb–Ramond field](../../../../../../kalb-ramond-field.md) and [dilaton](../../../../../../dilaton.md). The polarization redundancies found in Question 2 become, in position space, the linearized transformations $\delta G_{\mu\nu}=\partial_\mu\xi_\nu+\partial_\nu\xi_\mu$ and $\delta B_{\mu\nu}=\partial_\mu\Lambda_\nu-\partial_\nu\Lambda_\mu$. Thus the massless spin-two field already carries the gauge symmetry of linearized [general relativity](../../../../../../general-relativity-split.md).

To describe slowly varying backgrounds, promote these polarizations to fields of the embedding coordinates. The Euclidean [string nonlinear sigma model](../../../../../../string-nonlinear-sigma-model.md) is

$$
S_\sigma=\frac1{4\pi\alpha'}\int d^2\sigma\left(\sqrt h\,h^{ab}G_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu+i\epsilon^{ab}B_{\mu\nu}(X)\partial_aX^\mu\partial_bX^\nu+\alpha'\sqrt h\,R^{(2)}\Phi(X)\right).
$$

Here $\epsilon^{ab}$ is the antisymmetric coordinate density. Quantum consistency requires [worldsheet Weyl anomaly](../../../../../../worldsheet-weyl-anomaly.md) cancellation, not merely the classical background equations. At first order in $\alpha'$ the [bosonic sigma-model Weyl anomaly coefficients](../../../../../../bosonic-sigma-model-weyl-anomaly-coefficients.md) give

$$
R_{\mu\nu}+2\nabla_\mu\nabla_\nu\Phi-\frac14H_{\mu\rho\sigma}H_\nu{}^{\rho\sigma}=0,\qquad\nabla_\rho(e^{-2\Phi}H^{\rho\mu\nu})=0,
$$

where $H=dB$ is the [Kalb-Ramond field strength](../../../../../../kalb-ramond-field-strength.md). The scalar anomaly condition, combined with the trace of the metric condition in the critical dimension, gives

$$
R+4\nabla^2\Phi-4(\nabla\Phi)^2-\frac1{12}H^2=0.
$$

These are the Euler–Lagrange equations of the leading [string-frame massless effective action](../../../../../../string-frame-massless-effective-action.md)

$$
S_{\rm eff}^{(s)}=\frac1{2\kappa_0^2}\int d^{26}x\sqrt{-G}\,e^{-2\Phi}\left[R(G)+4(\nabla\Phi)^2-\frac1{12}H^2+O(\alpha')\right].
$$

For example, variation of $B$ gives the divergence equation above. Varying $\Phi$ and integrating its kinetic variation by parts gives $R+4\nabla^2\Phi-4(\nabla\Phi)^2-H^2/12=0$. Combining this with the metric variation yields the Ricci equation. Thus the string's quantum conformal consistency reproduces target-space gravity coupled to matter. Equivalently, expanding string scattering amplitudes at small [momenta](../../../../../../momentum.md) gives the same [action](../../../../../../action.md): massless exchange poles are reproduced by these fields, while analytic terms from massive exchange become local higher-derivative interactions.

The apparent [dilaton](../../../../../../dilaton.md)-dependent coefficient of $R$ is a frame choice. Put $\phi=\Phi-\Phi_0$ and, in dimension $D>2$, define the [Einstein-frame metric](../../../../../../einstein-frame-metric.md)

$$
g_{\mu\nu}^{(E)}=e^{-4\phi/(D-2)}G_{\mu\nu},\qquad\kappa^2=\kappa_0^2e^{2\Phi_0}.
$$

To see the cancellation explicitly, write $G=e^{2\omega}g^{(E)}$, $\omega=2\phi/(D-2)$. Then

$$
\sqrt{-G}\,e^{-2\Phi}R(G)=e^{-2\Phi_0}\sqrt{-g^{(E)}}\left[R_E-2(D-1)\nabla_E^2\omega-(D-1)(D-2)(\nabla_E\omega)^2\right].
$$

The Laplacian term is a boundary term. Combining the last term with the original positive [dilaton](../../../../../../dilaton.md) kinetic term produces $-4(\nabla_E\phi)^2/(D-2)$. The three inverse metrics in $H^2$ give its remaining exponential factor. Hence

$$
S_{\rm eff}^{(E)}=\frac1{2\kappa^2}\int d^Dx\sqrt{-g^{(E)}}\left[R_E-\frac4{D-2}(\nabla_E\phi)^2-\frac1{12}e^{-8\phi/(D-2)}H_E^2+O(\alpha')\right].
$$

For the uncompactified bosonic theory $D=26$, these coefficients are $-1/6$ and $e^{-\phi/3}$. The Ricci term is now the [Einstein-Hilbert action](../../../../../../einstein-hilbert-action.md); its metric variation gives the [Einstein field equations](../../../../../../einstein-field-equations.md) with [stress-energy tensor](../../../../../../stress-energy-tensor.md) from the scalar and two-form. **The leading low-energy theory is [general relativity](../../../../../../general-relativity-split.md) coupled to the massless string fields.**

The approximation requires characteristic [momenta](../../../../../../momentum.md) $E\sqrt{\alpha'}\ll1$ and small curvature in string units. Massive string modes have masses of order $1/\sqrt{\alpha'}$ and can be integrated out, generating corrections with extra powers of $\alpha' E^2$ or $\alpha' R$. The [string genus expansion](../../../../../../string-genus-expansion.md) supplies independent loop corrections controlled by $g_s=e^{\Phi_0}$; at weak coupling tree-level gravity dominates. Dimensional analysis gives $\kappa_{26}^2\propto g_s^2(\alpha')^{12}$.

[Compactification](../../../../../../compactification-physics.md) supplies lower-dimensional gravity and additional matter: metric and two-form components give [gauge fields](../../../../../../gauge-field.md), internal geometry gives scalar [moduli](../../../../../../modulus.md), and light modes of [Kaluza-Klein theory](../../../../../../kaluza-klein-theory.md) must be kept if their masses lie below the chosen cutoff. [Open strings](../../../../../../open-string.md) add [gauge fields](../../../../../../gauge-field.md), and supersymmetric string theories add [spacetime](../../../../../../spacetime.md) [fermions](../../../../../../fermion.md). Their particular matter spectrum depends on the [compactification](../../../../../../compactification-physics.md) and projection; universal massless spin-two interactions retain the gravitational form. Finally, the bosonic massless-sector [action](../../../../../../action.md) is a formal truncation around a tachyonically unstable vacuum. It does not remove that instability. Tachyon-free superstring backgrounds provide stable applications of this low-energy gravitational interpretation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
