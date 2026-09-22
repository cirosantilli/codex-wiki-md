<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use $g_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$ throughout. Vary the [Maxwell action](../../../../../maxwell-action.md) with respect to the [electromagnetic four-potential](../../../../../electromagnetic-four-potential.md). Antisymmetry of the [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md) gives $\delta\mathcal L=-F^{\mu\nu}\partial_\mu\delta A_\nu$. After integration by parts, the [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) is

$$
\boxed{\partial_\mu F^{\mu\nu}=0},\qquad
\Box A^\nu-\partial^\nu(\partial_\mu A^\mu)=0.
$$

A [gauge transformation](../../../../../gauge-transformation.md) $A_\mu\mapsto A_\mu+\partial_\mu\chi$ leaves $F_{\mu\nu}$ unchanged because [partial derivatives](../../../../../partial-derivative.md) commute. It therefore leaves the [Maxwell action](../../../../../maxwell-action.md) and observable electromagnetic fields unchanged: different potentials represent the same physical field. This redundancy matters for [canonical quantization](../../../../../canonical-quantization.md): before [gauge fixing](../../../../../gauge-fixing.md), the momentum conjugate to $A_0$ vanishes and the four potential components cannot be treated as four independent physical oscillators.

Choose the [Lorenz gauge](../../../../../lorenz-gauge-condition.md) $D=\partial_\mu A^\mu=0$, attainable by solving $\Box\chi=-D$ with suitable boundary data. The [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) then reduces to

$$
\boxed{\Box A^\mu=0}.
$$

[Residual Lorenz gauge symmetry](../../../../../residual-lorenz-gauge-symmetry.md) consists of transformations with $\Box\chi=0$. The gauge condition and this residual redundancy ultimately leave two [transverse polarizations](../../../../../transverse-polarization.md) of a free [photon](../../../../../photon.md).

For the specified kinetic density $\mathcal L_C=-\frac12\partial_\mu A_\nu\partial^\mu A^\nu$, one has $\partial\mathcal L_C/\partial(\partial_\mu A_\nu)=-\partial^\mu A^\nu$. Its [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) is therefore $-\Box A^\nu=0$. This density is the [Feynman-gauge Maxwell kinetic density after a boundary-term subtraction](../../../../../feynman-gauge-maxwell-kinetic-density-after-a-boundary-term-subtraction.md), since

$$
-\frac14F_{\mu\nu}F^{\mu\nu}-\frac12D^2
=\mathcal L_C+\partial_\mu K^\mu,\qquad
K^\mu=\frac12(A_\nu\partial^\nu A^\mu-A^\mu D).
$$

The divergence follows by expanding both sides and commuting the second derivatives. Thus the wave equation follows from a [Feynman gauge](../../../../../feynman-gauge.md) action; the additional physical-state condition will implement the [Lorenz gauge](../../../../../lorenz-gauge-condition.md). One must not impose $D=0$ inside the original action before varying it.

Take the covariant components $A_\nu$ as canonical coordinates. The [canonical momentum](../../../../../canonical-momentum.md) computed from $\mathcal L_C$ is

$$
\boxed{\Pi^\nu=\frac{\partial\mathcal L_C}{\partial(\partial_0A_\nu)}=-\partial_0A^\nu}.
$$

The equal-time canonical Poisson brackets are $\{A_\mu(t,\mathbf x),\Pi^\nu(t,\mathbf y)\}=\delta_\mu{}^\nu\delta^3(\mathbf x-\mathbf y)$, with coordinate-coordinate and momentum-momentum brackets zero. Applying [canonical quantization](../../../../../canonical-quantization.md) gives

$$
\boxed{[A_\mu(t,\mathbf x),\Pi^\nu(t,\mathbf y)]=i\delta_\mu{}^\nu\delta^3(\mathbf x-\mathbf y)},\qquad
[A_\mu,A_\nu]=[\Pi^\mu,\Pi^\nu]=0.
$$

In particular $[A_\mu,\dot A_\nu]=-ig_{\mu\nu}\delta^3$. The negative temporal sign is the source of the indefinite state-space norm in covariant photon quantization.

The spatial [Fourier transform](../../../../../fourier-transform.md) of the wave equation gives an oscillator of frequency $\omega=|\mathbf k|$ for each component. The [Hermitian adjoint](../../../../../adjoint-operator.md) condition on the [electromagnetic four-potential](../../../../../electromagnetic-four-potential.md) then yields the [mode expansion of a free field](../../../../../mode-expansion-of-a-free-field.md)

$$
\boxed{A_\mu(x)=\int\frac{d^3k}{(2\pi)^3 2\omega}\,[a_\mu(\mathbf k)e^{-ik\cdot x}+a_\mu^\dagger(\mathbf k)e^{ik\cdot x}]},\qquad k^\mu=(\omega,\mathbf k).
$$

These are massless [on shell](../../../../../on-shell.md) modes. Consistently with the preceding equal-time [canonical commutation relation](../../../../../canonical-commutation-relation.md),

$$
[a_\mu(\mathbf k),a_\nu^\dagger(\mathbf l)]=-g_{\mu\nu}(2\pi)^3 2\omega\delta^3(\mathbf k-\mathbf l),\qquad
[a_\mu,a_\nu]=[a_\mu^\dagger,a_\nu^\dagger]=0.
$$

The normalization is the same as for the scalar modes, with $-g_{\mu\nu}$ replacing the species identity matrix.

[Gupta-Bleuler quantization](../../../../../gupta-bleuler-formalism.md) starts with the [Fock vacuum](../../../../../fock-vacuum.md) annihilated by every $a_\mu$ and imposes only the annihilation, or [positive-frequency part of a quantum field](../../../../../positive-frequency-part-of-a-quantum-field.md), of the [Lorenz gauge](../../../../../lorenz-gauge-condition.md) condition:

$$
\boxed{(\partial_\mu A^\mu)^{(+)}|\mathrm{phys}\rangle=0}
\quad\Longleftrightarrow\quad
k^\mu a_\mu(\mathbf k)|\mathrm{phys}\rangle=0\quad\text{for every }\mathbf k.
$$

Imposing the entire Hermitian field divergence as a strong operator identity would be incompatible with the four-component [canonical commutation relation](../../../../../canonical-commutation-relation.md). The weaker condition suffices: between two physical states its positive-frequency part vanishes on the ket, and its negative-frequency part vanishes on the bra. Hence $\langle\mathrm{phys}'|\partial_\mu A^\mu|\mathrm{phys}\rangle=0$.

For a one-photon state $|\mathbf k,\epsilon\rangle=\epsilon^\nu a_\nu^\dagger(\mathbf k)|0\rangle$, commuting the constraint through the creator gives

$$
l^\mu a_\mu(\mathbf l)|\mathbf k,\epsilon\rangle
=-(k\cdot\epsilon)(2\pi)^3 2\omega\delta^3(\mathbf l-\mathbf k)|0\rangle.
$$

Thus the allowed [photon polarization vectors](../../../../../photon-polarization-vector.md) satisfy $\boxed{k\cdot\epsilon=0}$. Their state inner product, with the common momentum-normalization factor suppressed, is $\langle\epsilon'|\epsilon\rangle=-\epsilon'^*\cdot\epsilon$. Momentum eigenstates are delta-normalized; the same statements hold with finite norms for normalizable wave packets.

Rotate the spatial axes so that $k=\omega(1,0,0,1)$. The constraint is $\epsilon^0=\epsilon^3$, so the complete allowed family is

$$
\boxed{\epsilon=\alpha(1,0,0,1)+\beta(0,1,0,0)+\gamma(0,0,1,0)},\qquad \alpha,\beta,\gamma\in\mathbb C.
$$

The first vector is the allowed longitudinal gauge polarization, proportional to the null [four-momentum](../../../../../four-momentum.md) $k$. Its state has zero norm because $k^2=0$; it is also orthogonal to every constrained state because $k\cdot\epsilon=0$. A purely spatial vector $(0,0,0,1)$ alone is not an allowed physical polarization: its time component must accompany it to satisfy the constraint. The other two vectors are [transverse polarizations](../../../../../transverse-polarization.md), perpendicular to $\mathbf k$, with positive unit norms. For the displayed family,

$$
-\epsilon^*\cdot\epsilon=|\beta|^2+|\gamma|^2.
$$

The timelike negative-norm excitation has been excluded by the constraint, and the remaining form is positive semidefinite. The [Gupta-Bleuler null-state quotient](../../../../../gupta-bleuler-null-state-quotient.md) identifies $\epsilon$ and $\epsilon+\lambda k$, removing the null direction. It leaves exactly **two transverse physical photon polarizations** with a positive [inner product](../../../../../inner-product.md); their [bosonic Fock space](../../../../../bosonic-fock-space.md) is the physical photon state space.

Finally use [Feynman slash notation](../../../../../feynman-slash-notation.md), $\not a=\gamma^\mu a_\mu$, and impose [four-momentum conservation](../../../../../four-momentum-conservation.md) $p+q=k+k'$. The external [Dirac spinors](../../../../../dirac-spinor.md) obey

$$
(\not p-m)u(p)=0,\qquad \bar v(q)(\not q+m)=0.
$$

Set $r=p-k$ and $r'=p-k'$. Replacing $\epsilon$ by $k$ in the first term of the [electron-positron annihilation into two photons](../../../../../electron-positron-annihilation-into-two-photons.md) amplitude, the rightmost contracted vertex obeys

$$
\not k\,u=(\not p-m)u-(\not r-m)u=-(\not r-m)u.
$$

Since the [Clifford algebra](../../../../../clifford-algebra.md) implies $(\not r+m)(\not r-m)=(r^2-m^2)I_4$, that term becomes

$$
\bar v\not\epsilon'\frac{\not r+m}{r^2-m^2}\not k\,u
=-\bar v\not\epsilon'u.
$$

For the second term, [four-momentum conservation](../../../../../four-momentum-conservation.md) gives $k=q+r'$. The contracted vertex is now adjacent to the outgoing positron spinor on the left, so

$$
\bar v\not k=\bar v(\not q+\not r')=\bar v(\not r'-m).
$$

Consequently

$$
\bar v\not k\frac{\not r'+m}{r'^2-m^2}\not\epsilon'u
=+\bar v\not\epsilon'u.
$$

The two terms cancel, proving the [two-photon fermion Ward identity](../../../../../two-photon-fermion-ward-identity.md)

$$
\boxed{\bar v(q)M\big|_{\epsilon=k}u(p)=0,\qquad T\big|_{\epsilon=k}=0}.
$$

Exchanging the two photon labels proves the same result for $\epsilon'=k'$. By linearity the amplitude is invariant under $\epsilon\mapsto\epsilon+\lambda k$ on either external photon leg. Therefore the null longitudinal gauge polarization has zero production amplitude: **physical scattering produces only the two transverse photon polarizations**. This cancellation also shows why both photon orderings in the [tree-level Feynman diagrams](../../../../../tree-level-feynman-diagram.md) are essential; either term alone fails the [Ward identity](../../../../../ward-identity.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
