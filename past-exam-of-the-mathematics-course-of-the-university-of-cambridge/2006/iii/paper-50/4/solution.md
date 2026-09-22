<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the metric $\eta=\operatorname{diag}(1,-1,-1,-1)$ and first consider the connected [Poincaré group](../../../../../poincare-group.md), $\mathbb R^{1,3}\rtimes SO^+(1,3)$. Physical half-integer spins require [unitary representations](../../../../../unitary-representation.md) of its double cover $\mathbb R^{1,3}\rtimes SL(2,\mathbb C)$; genuine representations of the group without this cover permit only integer spin. Write $P^\mu=d(P^\mu)$ and $M^{\mu\nu}=d(M^{\mu\nu})$. Strong continuity gives self-adjoint generators, with [commutators](../../../../../commutator.md) understood on a common invariant dense domain.

The commuting translation generators have a joint spectral resolution. [Lorentz transformations](../../../../../lorentz-transformation.md) carry the spectral four-momentum $p$ to $\Lambda p$, so an [irreducible representation](../../../../../irreducible-representation.md) has its momentum spectral measure concentrated on a single Lorentz orbit. For positive-energy particles the orbits of interest are the future [mass shells](../../../../../mass-shell.md) $p^2=m^2>0$, or $p^2=0$ with $p\neq0$ and $p^0>0$. The zero-momentum orbit and spacelike or negative-energy orbits are outside these two particle cases.

Choose $\epsilon^{0123}=1$ and define the [Pauli-Lubanski pseudovector](../../../../../pauli-lubanski-pseudovector.md) with the overall sign convention

$$
W^\mu=-\frac12\epsilon^{\mu\nu\rho\sigma}P_\nu M_{\rho\sigma}.
$$

This sign makes the spatial rest-frame vector equal to $m\mathbf J$. The generators' Hermiticity and the antisymmetric epsilon contraction make $W^\mu$ Hermitian: the ordering correction from commuting $P$ through $M$ contracts metric tensors into epsilon and vanishes. The same antisymmetry proves [Pauli-Lubanski orthogonality](../../../../../pauli-lubanski-orthogonality.md), $W^\mu P_\mu=0$.

The assumed [commutators](../../../../../commutator.md) say that $P^\mu$ and $W^\mu$ transform as four-vectors and that $W$ commutes with all translations. Consequently

$$
C_1=P_\mu P^\mu,\qquad C_2=W_\mu W^\mu
$$

commute with the entire [Poincare algebra](../../../../../poincare-algebra.md). For instance the two terms in the Lorentz [commutator](../../../../../commutator.md) with a contracted vector square cancel. The [Casimir operators](../../../../../casimir-element.md) therefore have fixed spectral values in a [unitary irreducible representation](../../../../../unitary-irreducible-representation.md), by the [Schur lemma](../../../../../schur-s-lemma.md) applied to their spectral projections. A second ingredient, the [little group](../../../../../little-group.md), distinguishes the internal states.

Fix a standard momentum $k$ on the orbit. Its [little group](../../../../../little-group.md) is the subgroup of [Lorentz transformations](../../../../../lorentz-transformation.md) leaving $k$ fixed. Choose $L(p)$ with $L(p)k=p$. A [Lorentz transformation](../../../../../lorentz-transformation.md) acts on the internal fibre by the [Wigner rotation](../../../../../wigner-rotation.md)

$$
R(\Lambda,p)=L(\Lambda p)^{-1}\Lambda L(p),
\qquad R(\Lambda,p)k=k.
$$

If $d_K$ is a [unitary irreducible representation](../../../../../unitary-irreducible-representation.md) of this stabilizer, the [induced representation](../../../../../induced-representation.md) acts on wavefunctions as

$$
(U(a,\Lambda)\psi)(p)
=e^{-ia\cdot p}\,
d_K\!\left(R(\Lambda,\Lambda^{-1}p)\right)\psi(\Lambda^{-1}p).
$$

The measure $d^3p/(2p^0)$ on either future [mass shell](../../../../../mass-shell.md) is Lorentz invariant, so this action is unitary. The identity

$$
R(\Lambda_1\Lambda_2,p)
=R(\Lambda_1,\Lambda_2p)R(\Lambda_2,p)
$$

proves the group multiplication law. Conversely, covariance of the translation spectral resolution supplies precisely these fibres and their stabilizer action. A commuting operator acts fibrewise; transitivity relates its fibre values, and irreducibility of $d_K$ makes it scalar. This explains why the construction gives, and classifies, the [unitary irreducible representations](../../../../../unitary-irreducible-representation.md) on each orbit.

For a timelike momentum choose $k=(m,0,0,0)$. A [Lorentz transformation](../../../../../lorentz-transformation.md) fixing it acts only as a rotation of its spatial [orthogonal complement](../../../../../orthogonal-complement.md), so the [massive particle little group](../../../../../massive-particle-little-group.md) is $SO(3)$, or $SU(2)$ in the double cover. Put

$$
J_i=\frac12\epsilon_{ijk}M^{jk},\qquad K_i=M^{0i}.
$$

The [Poincare algebra](../../../../../poincare-algebra.md) gives $[J_i,J_j]=i\epsilon_{ijk}J_k$. The [unitary irreducible representations](../../../../../unitary-irreducible-representation.md) of $SU(2)$ are labelled by $j=0,\frac12,1,\ldots$, with $\mathbf J^2=j(j+1)$ and $J_3$ [eigenvalues](../../../../../eigenvalue.md) $-j,-j+1,\ldots,j$. Evaluation of the [Pauli-Lubanski pseudovector](../../../../../pauli-lubanski-pseudovector.md) at $k$ gives $W^0=0$, $\mathbf W=m\mathbf J$. Thus the [massive Pauli-Lubanski Casimir](../../../../../massive-pauli-lubanski-casimir.md) and particle labels are

$$
\boxed{P^2=m^2,\qquad W^2=-m^2j(j+1),\qquad
(m,j),\quad 2j+1\text{ spin states}.}
$$

The full [massive induced representation of the Poincare double cover](../../../../../massive-induced-representation-of-the-poincare-double-cover.md) is infinite-dimensional because momentum ranges continuously over the orbit; its finite internal multiplicity is $2j+1$.

For a null momentum choose $k=(E,0,0,E)$ with $E>0$. The infinitesimal stabilizer generators are

$$
R=J_3,\qquad N_1=K_1-J_2,\qquad N_2=K_2+J_1.
$$

Their [commutators](../../../../../commutator.md) with momentum, evaluated at $k$, vanish. From the rotation and boost [commutators](../../../../../commutator.md) of the [Poincare algebra](../../../../../poincare-algebra.md) one obtains

$$
[R,N_1]=iN_2,\qquad [R,N_2]=-iN_1,\qquad[N_1,N_2]=0.
$$

These are the [massless little-group generators](../../../../../massless-little-group-generators.md) of $ISO(2)$: a planar rotation and two commuting null rotations, which act like translations in the little-group algebra. Hence the [massless particle little group](../../../../../massless-particle-little-group.md) is the Euclidean plane group, with the appropriate double cover for half-integer spin.

The definition of $W$ gives $W^0=\mathbf P\cdot\mathbf J$ and $\mathbf W=P^0\mathbf J-\mathbf P\times\mathbf K$. At the standard null momentum,

$$
W^\mu=(ER,EN_2,-EN_1,ER),\qquad
W^2=-E^2(N_1^2+N_2^2).
$$

Suppose the little-group representation has finite [dimension](../../../../../dimension-vector-space.md), as for particles with finitely many polarizations. The commuting Hermitian $N_1,N_2$ have a finite joint spectrum. Conjugation by $e^{-i\phi R}$ rotates this spectrum through every planar angle. The only finite set invariant under all these rotations is the origin. Thus both $N_i$ vanish, proving that [finite-dimensional unitary representations of the massless little group have trivial translations](../../../../../finite-dimensional-unitary-representations-of-the-massless-little-group-have-trivial-translations.md). Irreducibility then leaves a one-dimensional rotation character, $R=hI$. The [massless longitudinal Pauli-Lubanski eigenvalues](../../../../../massless-longitudinal-pauli-lubanski-eigenvalues.md) are

$$
\boxed{P^2=0,\qquad W^\mu=hP^\mu,\qquad W^2=0,\qquad
h\in\tfrac12\mathbb Z}
$$

for the double cover, with $h\in\mathbb Z$ for a genuine $SO(2)$ character. The number $h$ is [helicity](../../../../../helicity.md). Different helicities have the same two [Casimir eigenvalues](../../../../../casimir-eigenvalue.md), so the [little group](../../../../../little-group.md) is indispensable for the classification. A connected-group [irreducible representation](../../../../../irreducible-representation.md) has one [helicity](../../../../../helicity.md); if parity is also implemented, it exchanges $h$ and $-h$ and normally requires their pair.

Unitarity alone also permits nontrivial null-rotation generators. The rotation-invariant operator $N_1^2+N_2^2$ is scalar in an irreducible little-group representation; if it has value $(\rho/E)^2>0$, one obtains a [continuous-spin representation](../../../../../continuous-spin-representation.md). A concrete realization on angular wavefunctions is

$$
N_1=\frac{\rho}{E}\cos\phi,\qquad
N_2=\frac{\rho}{E}\sin\phi,\qquad
R=-i\frac{d}{d\phi}.
$$

These operators satisfy the same [commutators](../../../../../commutator.md). Periodic or antiperiodic angular wavefunctions give integer or half-integer rotation modes, and the translation generators connect infinitely many such modes. The invariant labels are

$$
\boxed{P^2=0,\qquad W^2=-\rho^2,\qquad\rho>0.}
$$

These are the additional infinite-polarization massless [unitary irreducible representations](../../../../../unitary-irreducible-representation.md). Restricting to finitely many particle polarizations excludes them; they must not be ruled out merely by assuming unitarity. This completes the timelike and null cases of the [Wigner classification](../../../../../wigner-s-classification.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
