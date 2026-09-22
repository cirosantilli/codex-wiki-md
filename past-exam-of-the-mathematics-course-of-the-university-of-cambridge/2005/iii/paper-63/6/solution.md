<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use $\iota_{X_f}\omega=df$ and $\{f,g\}=\omega(X_f,X_g)$. For an actual infinitesimal left [Lie group action](../../../../../lie-group-action.md), define $\xi_P(p)=\left.\frac d{dt}\right|_0\exp(t\xi)\cdot p$. Its [fundamental vector fields](../../../../../fundamental-vector-field.md) obey $[\xi_P,\eta_P]=-[\xi,\eta]_P$ with this convention.

**Existence and its global obstruction.** Preservation of the [symplectic form](../../../../../symplectic-form.md) gives $\mathcal L_{\xi_P}\omega=0$. By [Cartan's magic formula](../../../../../cartan-s-magic-formula.md), $\iota_{\xi_P}\omega$ is closed. Locally it equals $d\mu_\xi$; globally this requires its class in $H^1_{\rm dR}(P)$ to vanish. If it does for every $\xi$, choose potentials linearly in $\xi$ and define

$$
\langle\mu(p),\xi\rangle=\mu_\xi(p),\qquad d\mu_\xi=\iota_{\xi_P}\omega.
$$

This gives the component Hamiltonians of a [weakly Hamiltonian action](../../../../../weakly-hamiltonian-action.md). The assumption in the question does not alone guarantee a global [moment map](../../../../../moment-map.md): on $T^2$ with $\omega=dx\wedge dy$, translation in $x$ preserves $\omega$, but its contraction is $dy$, whose integral around the $y$ circle is nonzero. It is not an exact [one-form](../../../../../one-form.md). Thus no global real-valued component Hamiltonian exists for that circle action. The intended construction is valid locally, or globally with this exactness condition, for example if $H^1_{\rm dR}(P)=0$.

**Matching the Lie algebra.** On each connected component, the [moment-map equivariance obstruction](../../../../../moment-map-equivariance-obstruction.md) is the constant

$$
c(\xi,\eta)=\{\mu_\xi,\mu_\eta\}-\mu_{[\xi,\eta]}.
$$

Indeed, the identities $[X_f,X_g]=-X_{\{f,g\}}$ and $[\xi_P,\eta_P]=-[\xi,\eta]_P$ show that its differential vanishes. The [Jacobi identity](../../../../../jacobi-identity.md) for the [Poisson bracket](../../../../../poisson-bracket.md) says

$$
c([\xi,\eta],\zeta)+c([\eta,\zeta],\xi)+c([\zeta,\xi],\eta)=0.
$$

Changing $\mu_\xi$ by a linear constant $b(\xi)$ changes $c$ to $c-b([\xi,\eta])$. Consequently the necessary and sufficient infinitesimal condition is **the cocycle must be a coboundary**, so that the constants can be chosen with

$$
\boxed{\{\mu_\xi,\mu_\eta\}=\mu_{[\xi,\eta]}.}
$$

Equivalently its class in $H^2(\mathfrak g,\mathbb R)$ vanishes. For a connected group this infinitesimal equivariance integrates to equivariance under its [coadjoint action](../../../../../coadjoint-representation.md). A disconnected group can impose additional conditions. Here “coincides” means representing the specified Lie brackets; it does not guarantee injectivity when the group action has ineffective generators.

**Proof using the Killing form.** A nondegenerate [Killing form](../../../../../killing-form.md) $B$ makes $\mathfrak g$ semisimple. First, it is perfect: the $B$-orthogonal complement of $[\mathfrak g,\mathfrak g]$ is the center by invariance, and the center is zero by nondegeneracy. For symplectic fields,

$$
\iota_{[\xi,\eta]_P}\omega=d[\omega(\xi_P,\eta_P)]
$$

by [Cartan's magic formula](../../../../../cartan-s-magic-formula.md) and the antihomomorphism sign. Every commutator therefore has an exact contraction. Perfectness supplies component Hamiltonians for every generator, even when $P$ is not simply connected: this is [Hamiltonian existence for a semisimple symplectic action](../../../../../hamiltonian-existence-for-a-semisimple-symplectic-action.md).

It remains to eliminate the cocycle, not merely to name an existence theorem. Define a linear operator $D$ on $\mathfrak g$ by $B(D\xi,\eta)=c(\xi,\eta)$. Antisymmetry of $c$ makes $D$ skew for $B$. Combining its cocycle identity with invariance of $B$ gives

$$
D[\xi,\eta]=[D\xi,\eta]+[\xi,D\eta].
$$

Choose $Z\in\mathfrak g$ by $B(Z,\xi)=\operatorname{tr}(D\operatorname{ad}_\xi)$, possible because $B$ is nondegenerate. Since $D$ is a derivation, $[D,\operatorname{ad}_\xi]=\operatorname{ad}_{D\xi}$. Cyclicity of the [matrix trace](../../../../../matrix-trace.md) then gives

$$
\begin{aligned}
B([Z,\xi],\eta)&=B(Z,[\xi,\eta])=\operatorname{tr}(D[\operatorname{ad}_\xi,\operatorname{ad}_\eta])\\
&=\operatorname{tr}([D,\operatorname{ad}_\xi]\operatorname{ad}_\eta)=B(D\xi,\eta).
\end{aligned}
$$

Thus $D=\operatorname{ad}_Z$, and $c(\xi,\eta)=B(Z,[\xi,\eta])$. Taking $b(\xi)=B(Z,\xi)$ removes $c$, proving the required condition. This applies to [semisimple Lie groups](../../../../../semisimple-lie-group.md), including $SU(n)$ for $n\ge2$, $SO(3)$ and $SL(n,\mathbb R)$ for $n\ge2$. It is nondegeneracy, not positive definiteness, that matters. Groups with a nonzero central Lie algebra, such as $U(3)$, do not satisfy this Killing-form criterion, although particular actions can still have equivariant [moment maps](../../../../../moment-map.md).

**The isotropic oscillator.** On $T^*\mathbb R^3$, put

$$
z_j=\frac{x_j+ip_j}{\sqrt2},\qquad\omega=i\sum_j dz_j\wedge d\bar z_j,\qquad H=z^\dagger z.
$$

The action $z\mapsto Uz$, $U\in U(3)$, preserves the Hermitian norm and the [symplectic form](../../../../../symplectic-form.md), and therefore preserves $H$. A Hermitian matrix $A$ parametrizes the Lie algebra generator $\xi=-iA$. Its [unitary moment map of an isotropic oscillator](../../../../../unitary-moment-map-of-an-isotropic-oscillator.md) is

$$
\mu_A=z^\dagger Az,\qquad X_{\mu_A}z=-iAz.
$$

Since $\{z_j,\bar z_k\}=-i\delta_{jk}$, direct differentiation yields

$$
\boxed{\{\mu_A,\mu_B\}=-iz^\dagger[A,B]z=\mu_{-i[A,B]}.}
$$

The matrix $-i[A,B]$ is Hermitian and corresponds precisely to $[\xi_A,\xi_B]$; no central defect remains. The full [moment map](../../../../../moment-map.md) can be identified, using the pairing with Hermitian matrices, with the rank-one matrix $zz^\dagger$. The central generator $A=I$ gives **$\mu_I=H$**, whose flow is $z(t)=e^{-it}z(0)$. Globally $U(3)=(SU(3)\times U(1))/\mathbb Z_3$, so the “$U(1)$ factor” refers to this central circle, rather than a literal direct-product decomposition.

The real orthogonal subgroup acts geometrically by $(x,p)\mapsto(Rx,Rp)$, the [cotangent lift of a diffeomorphism](../../../../../cotangent-lift-of-a-diffeomorphism.md) of $\mathbb R^3$. If $K$ is real antisymmetric and $A=iK$, then $\mu_A=-x^TKp$. For $Kv=\Omega\times v$, this is $\Omega\cdot(x\times p)$, so its three components are the usual [angular momentum](../../../../../angular-momentum.md) $L_i=\epsilon_{ijk}x_jp_k$.

The remaining six independent Hermitian directions can be taken as real symmetric matrices. Their moment functions span

$$
Q_{ij}=\frac12(x_ix_j+p_ip_j),\qquad Q_{ij}=Q_{ji}.
$$

The diagonal ones are the individual oscillator energies; their sum is $H$. The off-diagonal ones correlate two oscillator modes. Their flows mix positions and momenta and are not cotangent lifts of the obvious spatial rotation action: for a real symmetric $A$, $\dot x=Ap$ and $\dot p=-Ax$, rather than $\dot x=Kx$, $\dot p=Kp$. All nine quadratic functions commute with $H$, since the entire [unitary group](../../../../../unitary-group.md) action preserves the oscillator [Hamiltonian](../../../../../hamiltonian.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 63](../../paper-63-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
