<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Consider positive-energy [unitary irreducible representations](../../../../../unitary-irreducible-representation.md) of the proper orthochronous [Poincaré group](../../../../../poincare-group.md), allowing its double cover for physical half-integer spin. Use metric $(+---)$ and define the [Pauli-Lubanski pseudovector](../../../../../pauli-lubanski-pseudovector.md) by

$$
W^\mu=-\tfrac12\epsilon^{\mu\nu\rho\sigma}d(P_\nu)d(M_{\rho\sigma}),\qquad\epsilon^{0123}=1.
$$

This overall sign gives $\mathbf W=m\mathbf J$ at rest. The antisymmetric tensor and commuting translation generators give $P_\mu W^\mu=0$. The given commutators say $W$ commutes with translations and transforms as a Lorentz vector. Hence both $P^2$ and $W^2$ commute with the [Poincare algebra](../../../../../poincare-algebra.md); they are [Casimir operators](../../../../../casimir-element.md).

The commuting Hermitian translation generators admit generalized joint momentum eigenstates. A [Lorentz transformation](../../../../../lorentz-transformation.md) maps a state at $p$ to a state at $\Lambda p$, so an irreducible representation has momentum support on a single Lorentz orbit. Choose a standard momentum $k$. Its [little group](../../../../../little-group.md) consists of the transformations fixing $k$ and acts on the internal states there. Transport those internal states over the orbit by chosen transformations $L(p)k=p$. This gives the construction underlying [Wigner's classification](../../../../../wigner-s-classification.md).

For timelike future-directed momenta, $P^2=m^2$ with $m>0$ and $k=(m,0,0,0)$. The [massive particle little group](../../../../../massive-particle-little-group.md) is [SO(3)](../../../../../so-3-group.md), or [SU(2)](../../../../../su-2-group.md) on the double cover. Write $J_i=\epsilon_{ijk}d(M^{jk})/2$. The rotation commutators give $[J_i,J_j]=i\epsilon_{ijk}J_k$, so the irreducible little-group representation has

$$
\mathbf J^2=s(s+1)I,\qquad J_3\text{ eigenvalues }-s,-s+1,\ldots,s.
$$

At rest, $W^0=0$ and $\mathbf W=m\mathbf J$. Thus the [massive Pauli-Lubanski Casimir](../../../../../massive-pauli-lubanski-casimir.md) is

$$
\boxed{P^2=m^2I,\qquad W^2=-m^2s(s+1)I.}
$$

The rest spin space has dimension $2s+1$. All $s=0,\tfrac12,1,\ldots$ occur for the double cover; only integer spin descends to an ordinary single-valued representation of the proper orthochronous Poincare group.

For the detailed representation, choose a [Lorentz boost](../../../../../lorentz-boost.md) $L(p)$ from $k$ to every point of the positive-energy [mass shell](../../../../../mass-shell.md). With invariant normalization, states $|p,\sigma\rangle=U(L(p))|k,\sigma\rangle$ transform as

$$
U(\Lambda)|p,\sigma\rangle
=\sum_\tau D^{(s)}_{\tau\sigma}(R(\Lambda,p))|\Lambda p,\tau\rangle,\qquad
R(\Lambda,p)=L(\Lambda p)^{-1}\Lambda L(p).
$$

The matrix $R$ fixes $k$, so it is the [Wigner rotation](../../../../../wigner-rotation.md) in the little group. Its cocycle identity

$$
R(\Lambda_2\Lambda_1,p)=R(\Lambda_2,\Lambda_1p)R(\Lambda_1,p)
$$

proves the representation law. Translations give phases; with the convention $U(a)|p,\sigma\rangle=e^{ip\cdot a}|p,\sigma\rangle$, this extends to the [massive induced representation of the Poincare double cover](../../../../../massive-induced-representation-of-the-poincare-double-cover.md) on

$$
L^2\left(\mathcal H_m^+,\frac{d^3p}{2p^0}\right)\otimes\mathbb C^{2s+1}.
$$

The invariant measure and unitary spin matrices give unitarity. A closed invariant subspace restricts at fixed momentum to a little-group invariant spin subspace; irreducibility of that spin representation and transitivity over the mass shell force the full representation to be irreducible. Conversely the momentum-orbit construction recovers every massive positive-energy irreducible representation. The labels are therefore $(m,s)$.

For a nonzero future null momentum choose $k=(E,0,0,E)$. The [massless particle little group](../../../../../massless-particle-little-group.md) is $ISO(2)$. With $K_i=d(M^{0i})$, its [massless little-group generators](../../../../../massless-little-group-generators.md) are

$$
J_3,\qquad N_1=K_1-J_2,\qquad N_2=K_2+J_1,
$$

with $[J_3,N_1]=iN_2$, $[J_3,N_2]=-iN_1$ and $[N_1,N_2]=0$. Evaluating the Pauli-Lubanski vector gives $W^2=-E^2(N_1^2+N_2^2)$.

In a finite-dimensional unitary little-group representation, the joint spectrum of the commuting Hermitian $N_1,N_2$ is finite and invariant under continuous planar rotations. Its only possible values are zero. Thus [finite-dimensional unitary representations of the massless little group have trivial translations](../../../../../finite-dimensional-unitary-representations-of-the-massless-little-group-have-trivial-translations.md). Irreducibility then leaves a one-dimensional rotation character of [helicity](../../../../../helicity.md) $h$, giving

$$
\boxed{W^\mu=hP^\mu,\qquad P^2=W^2=0.}
$$

Helicity supplies an additional label that the two zero Casimirs cannot distinguish. It is integer for the ordinary group and may be half-integer on its physical double cover. Nontrivial little-group translations instead lead to an infinite-dimensional [continuous-spin representation](../../../../../continuous-spin-representation.md) with $W^2<0$; the Poincare algebra by itself allows these too. This completes the timelike and nonzero null cases of physical interest.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
