<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Vary the [Maxwell Lagrangian](../../../../../maxwell-lagrangian.md) with respect to $A_\nu$. Since $\delta F_{\mu\nu}=\partial_\mu\delta A_\nu-\partial_\nu\delta A_\mu$ and $F$ is antisymmetric,

$$
\delta\mathcal L=-F^{\mu\nu}\partial_\mu\delta A_\nu.
$$

After [integration by parts](../../../../../integration-by-parts.md), the [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) is

$$
\boxed{\partial_\mu F^{\mu\nu}=0,\qquad
\Box A^\nu-\partial^\nu(\partial_\mu A^\mu)=0.}
$$

The [gauge transformation](../../../../../gauge-transformation.md) $A_\mu\mapsto A_\mu+\partial_\mu\chi$ leaves $F_{\mu\nu}$ unchanged because [partial derivatives](../../../../../partial-derivative.md) commute. This [gauge invariance](../../../../../gauge-invariance.md) means that potentials related in this way represent the same electromagnetic field; all four potential components are not independent physical [photon](../../../../../photon.md) degrees of freedom. In particular, the ungauged kinetic operator is singular and its temporal [canonical momentum](../../../../../canonical-momentum.md) vanishes.

Choose the [Lorenz gauge](../../../../../lorenz-gauge-condition.md) $\partial_\mu A^\mu=0$. The field equation then becomes $\boxed{\Box A_\mu=0}$. Residual [gauge transformations](../../../../../gauge-transformation.md) with $\Box\chi=0$ preserve this condition. The correctly named [Lorenz gauge condition](../../../../../lorenz-gauge-condition.md) concerns the divergence of the potential; [Lorentz covariance](../../../../../lorentz-covariance.md) is the separate transformation property of the equations.

For the alternative quadratic [Lagrangian density](../../../../../lagrangian-density.md), direct differentiation gives

$$
\frac{\partial\mathcal L'}{\partial(\partial_\rho A_\nu)}=-\partial^\rho A^\nu,
$$

so its [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) is also $\Box A^\nu=0$. This density is the [Feynman-gauge Maxwell kinetic density after a boundary-term subtraction](../../../../../feynman-gauge-maxwell-kinetic-density-after-a-boundary-term-subtraction.md). Indeed, with $D=\partial_\mu A^\mu$,

$$
-\frac14F_{\mu\nu}F^{\mu\nu}-\frac12D^2
=-\frac12\partial_\mu A_\nu\partial^\mu A^\nu+\partial_\mu K^\mu,\qquad
K^\mu=\frac12(A_\nu\partial^\nu A^\mu-A^\mu D).
$$

The divergence identity follows by expanding $\partial_\mu K^\mu$ and commuting its second derivatives. The quadratic density alone describes four wave equations; the gauge constraint must still be incorporated in the physical states. It is not an unconstrained four-positive-polarization replacement for [Maxwell equations](../../../../../maxwell-equations.md).

Using this specified boundary-term convention, the [canonical momentum](../../../../../canonical-momentum.md) conjugate to $A_\nu$ is

$$
\boxed{\Pi^\nu=-\partial_0A^\nu.}
$$

The [canonical commutation relations](../../../../../canonical-commutation-relation.md) are therefore

$$
\boxed{[A_\mu(t,\mathbf x),\Pi^\nu(t,\mathbf y)]
=i\delta_\mu{}^\nu\delta^3(\mathbf x-\mathbf y),}
$$

with field-field and momentum-momentum brackets zero. Equivalently $[A_\mu,\dot A_\nu]=-ig_{\mu\nu}\delta^3$. The temporal component has the opposite sign to the spatial components; replacing the metric by a positive Euclidean one would destroy these brackets.

The [wave equation](../../../../../wave-equation-split.md) gives massless [frequencies](../../../../../frequency.md) $\omega_{\mathbf k}=|\mathbf k|$. Hermiticity pairs its positive- and negative-frequency solutions, so the [Heisenberg picture](../../../../../heisenberg-picture.md) field has the expansion

$$
\boxed{A_\mu(x)=\int\frac{d^3k}{(2\pi)^3 2\omega_{\mathbf k}}
\left[a_\mu(k)e^{-ik\cdot x}+a_\mu^\dagger(k)e^{ik\cdot x}\right],\qquad
k^0=\omega_{\mathbf k},\quad k^2=0.}
$$

This is a real field expansion for each component, but its oscillator metric is indefinite. The assumed brackets, with the dagger's vector index restored, are

$$
[a_\mu(k),a_\nu^\dagger(k')]=-g_{\mu\nu}(2\pi)^3 2\omega_{\mathbf k}\delta^3(\mathbf k-\mathbf k').
$$

They verify the [photon oscillator completeness and canonical brackets](../../../../../photon-oscillator-completeness-and-canonical-brackets.md). Inserting $\Pi^\nu=-\dot A^\nu$ gives at equal times

$$
[A_\mu(t,\mathbf x),\Pi^\nu(t,\mathbf y)]
=\frac{i\delta_\mu{}^\nu}{2}\int\frac{d^3k}{(2\pi)^3}
\left[e^{i\mathbf k\cdot(\mathbf x-\mathbf y)}+e^{-i\mathbf k\cdot(\mathbf x-\mathbf y)}\right]
=i\delta_\mu{}^\nu\delta^3(\mathbf x-\mathbf y).
$$

The other brackets cancel between the two [frequency](../../../../../frequency.md) contributions. Thus both the $2\omega$ normalization and the sign $-g_{\mu\nu}$ are needed.

The [Gupta-Bleuler formalism](../../../../../gupta-bleuler-formalism.md) imposes the [Lorenz gauge condition](../../../../../lorenz-gauge-condition.md) weakly on states:

$$
(\partial_\mu A^\mu)^{(+)}|\mathrm{phys}\rangle=0,
\qquad k^\mu a_\mu(k)|\mathrm{phys}\rangle=0\quad\text{for every }k.
$$

Here $(+)$ is the annihilation, positive-frequency part. Setting the full divergence to zero as an operator would conflict with the four-component [canonical commutation relations](../../../../../canonical-commutation-relation.md). The subsidiary condition instead selects a physical pre-space inside the [covariant photon Fock space](../../../../../covariant-photon-fock-space.md), followed by a quotient of its null states.

Apply it to $|k,\epsilon\rangle=\epsilon^\nu a_\nu^\dagger(k)|0\rangle$. Commuting $k^\mu a_\mu$ through the creator gives a multiple of $-k_\nu\epsilon^\nu|0\rangle$. Hence the allowed [photon polarization vectors](../../../../../photon-polarization-vector.md) obey

$$
\boxed{k\cdot\epsilon=0.}
$$

Take $k=(\omega,0,0,\omega)$. The complete solution is

$$
\epsilon=(c,\alpha,\beta,c)
=c(1,0,0,1)+\alpha(0,1,0,0)+\beta(0,0,1,0),
$$

with complex [coefficients](../../../../../coefficient.md). The last two vectors are transverse linear [photon polarizations](../../../../../photon-polarization.md), and $(0,1,\pm i,0)/\sqrt2$ gives the two circular [photon polarizations](../../../../../photon-polarization.md). The first vector is $k/\omega$, the allowed temporal-longitudinal combination. A purely spatial longitudinal vector $(0,0,0,1)$ by itself does not satisfy the subsidiary condition.

The oscillator brackets give, apart from the positive continuum normalization factor,

$$
\langle k,\epsilon|k,\epsilon\rangle=-\epsilon^{*\mu}g_{\mu\nu}\epsilon^\nu
=\boxed{|\alpha|^2+|\beta|^2}.
$$

[Momentum](../../../../../momentum.md) eigenstates are distributionally normalized; a box or a [wave packet](../../../../../wave-packet.md) makes the norm statement literal. The allowed longitudinal combination has zero norm because $k^2=0$, and it is orthogonal to every constrained state since $k\cdot\epsilon=0$. It also gives a pure-gauge field wave: the field strength of $A_\mu\propto k_\mu e^{-ik\cdot x}$ vanishes. Thus $\epsilon$ and $\epsilon+ck$ represent the same physical [photon polarization](../../../../../photon-polarization.md). The [Gupta-Bleuler null-state quotient](../../../../../gupta-bleuler-null-state-quotient.md) removes this null direction and leaves **two positive-norm transverse [photon](../../../../../photon.md) [photon polarizations](../../../../../photon-polarization.md)**. The negative-norm temporal oscillator of the unrestricted space is not an extra physical state. This is the [transverse one-photon physical quotient](../../../../../transverse-one-photon-physical-quotient.md).

Finally verify the [two-photon fermion Ward identity](../../../../../two-photon-fermion-ward-identity.md) directly for [electron-positron annihilation into two photons](../../../../../electron-positron-annihilation-into-two-photons.md). Define $D(r)=\not r-m$ and the reduced [Dirac propagator](../../../../../dirac-propagator.md)

$$
G(r)=D(r)^{-1}=\frac{\not r+m}{r^2-m^2}.
$$

The equality follows from the [Clifford algebra](../../../../../clifford-algebra.md), since $(\not r-m)(\not r+m)=(r^2-m^2)I$. The incoming [Dirac spinors](../../../../../dirac-spinor.md) obey $D(p)u(p)=0$ and $\overline v(q)(\not q+m)=0$. On replacing one inserted [photon polarization vector](../../../../../photon-polarization-vector.md) by $k$, the [spinor](../../../../../spinor.md) factor in the two diagrams is

$$
\overline v(q)\left[\not\epsilon'G(p-k)\not k+\not kG(p-k')\not\epsilon'\right]u(p).
$$

At the electron end, $\not k=D(p)-D(p-k)$, so

$$
G(p-k)\not k\,u(p)=-u(p).
$$

For the other diagram, [four-momentum conservation](../../../../../four-momentum-conservation.md) gives $p-k'=k-q$. Hence

$$
\not k=D(p-k')+(\not q+m),\qquad
\overline v(q)\not kG(p-k')=\overline v(q).
$$

The two contributions therefore cancel exactly:

$$
T\big|_{\epsilon\to k}
=-e^2\left[-\overline v(q)\not\epsilon' u(p)+\overline v(q)\not\epsilon' u(p)\right]
=\boxed{0}.
$$

Individual diagrams need not vanish; their sum implements the [Ward identity](../../../../../ward-identity.md). Linearity then gives invariance under $\epsilon\mapsto\epsilon+ck$, as required by [gauge invariance](../../../../../gauge-invariance.md). In particular, the null longitudinal [photon polarization](../../../../../photon-polarization.md) proportional to $k$ has zero physical production amplitude. **Physical scattering produces the transverse [photon](../../../../../photon.md) classes**, not an independent longitudinal massless [photon](../../../../../photon.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
