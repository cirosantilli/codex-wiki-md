<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use $\iota_{X_f}\omega=-df$ and $\{f,g\}=X_gf$, so in the stated real coordinates $\{q^i,p_j\}=\delta^i_j$ and $\dot f=\{f,H\}$. For $\xi\in\mathfrak g$, let $\xi_P$ be the actual [fundamental vector field](../../../../../fundamental-vector-field.md) of the left action, obtained by differentiating $\exp(t\xi)\cdot x$ at zero. Since the action preserves $\omega$, [Cartan's magic formula](../../../../../cartan-s-magic-formula.md) gives $d(\iota_{\xi_P}\omega)=0$.

A global component Hamiltonian $\mu_\xi$ requires this closed one-form to be exact, with

$$
\boxed{d\mu_\xi=-\iota_{\xi_P}\omega,\qquad
\langle\mu(x),\xi\rangle=\mu_\xi(x).}
$$

Choose these functions linearly in $\xi$. This defines the [moment map](../../../../../moment-map.md), with equivariance when the constants have the required normalization. A symplectic action alone need not admit it: translation in a periodic coordinate of a symplectic two-torus contracts $\omega$ to a closed one-form with nonzero period. A sufficient existence condition is $H^1_{\rm dR}(P)=0$; more generally one assumes the action is weakly Hamiltonian and resolves its [moment-map equivariance obstruction](../../../../../moment-map-equivariance-obstruction.md).

Because the group also preserves $H$,

$$
\{H,\mu_\xi\}=X_{\mu_\xi}H=\xi_PH=0,
\qquad\boxed{\dot\mu_\xi=\{\mu_\xi,H\}=0.}
$$

The component vector fields commute with the Hamiltonian flow: in this convention $[X_f,X_g]=-X_{\{f,g\}}$, hence $[X_{\mu_\xi},X_H]=0$. These are both conserved observables and infinitesimal symmetries of the dynamics.

For a left action, fundamental vector fields obey $[\xi_P,\eta_P]=-[\xi,\eta]_P$. Together with the Hamiltonian-field identity, this makes

$$
c(\xi,\eta)=\{\mu_\xi,\mu_\eta\}-\mu_{[\xi,\eta]}
$$

have zero Hamiltonian vector field. It is therefore constant on each connected component of $P$. One sufficient condition for $c=0$ is an equivariant moment map, $\mu(gx)=\operatorname{Ad}_g^*\mu(x)$, where $\langle\operatorname{Ad}_g^*\ell,\xi\rangle=\langle\ell,\operatorname{Ad}_{g^{-1}}\xi\rangle$. Differentiating this condition along $\eta_P$ gives directly

$$
\boxed{\{\mu_\xi,\mu_\eta\}=\mu_{[\xi,\eta]}.}
$$

A useful concrete sufficient condition is a common fixed point $x_0$ and the normalization $\mu_\xi(x_0)=0$. The constant $c$ is zero there because all fundamental fields vanish, and hence zero everywhere on connected $P$. This is [fixed-point normalization removes the moment-map cocycle](../../../../../fixed-point-normalization-removes-the-moment-map-cocycle.md). If the action has an ineffective Lie-algebra kernel, the map to observables can have that kernel; equality of brackets alone is not a claim of a faithful representation.

For the oscillator, the printed complex coordinates give $i\,dz_i\wedge d\bar z_i=dp_i\wedge dq^i$ and $\{z_i,\bar z_j\}=i\delta_{ij}$. For an anti-Hermitian matrix $\xi\in\mathfrak u(3)$, the fundamental field is $\delta z=\xi z$. Direct contraction yields

$$
\iota_{\xi_P}\omega=i\,d(z^\dagger\xi z).
$$

Consequently the [unitary moment map of an isotropic oscillator](../../../../../unitary-moment-map-of-an-isotropic-oscillator.md) in our declared convention is

$$
\boxed{\mu_\xi(z)=-i z^\dagger\xi z.}
$$

It is real because $\xi$ is anti-Hermitian. Identifying $\mathfrak u(3)^*$ with Hermitian matrices by $\langle M,\xi\rangle=-i\operatorname{Tr}(M\xi)$, this is simply **$\mu(z)=zz^\dagger$**. Unitary invariance of $H=z^\dagger z$ proves conservation of all nine real matrix components. Under $z\mapsto Uz$, the matrix transforms as $zz^\dagger\mapsto Uzz^\dagger U^{-1}$, exactly the coadjoint transformation in this pairing. The origin is the required fixed point.

The bracket can also be checked without an equivariance theorem. For $f=-i\bar z\xi z$ and $g=-i\bar z\eta z$, use

$$
\{f,g\}=i\sum_j\left(\frac{\partial f}{\partial z_j}\frac{\partial g}{\partial\bar z_j}
-\frac{\partial f}{\partial\bar z_j}\frac{\partial g}{\partial z_j}\right).
$$

Differentiation gives $\{\mu_\xi,\mu_\eta\}=-i z^\dagger[\xi,\eta]z=\mu_{[\xi,\eta]}$. The central generator $\xi=iI$ has $\mu_\xi=H$, while a real antisymmetric generator $\xi v=a\times v$ has

$$
\mu_\xi=-i\bar z\cdot(a\times z)=a\cdot(q\times p).
$$

Thus the [special orthogonal group](../../../../../special-orthogonal-group.md) subgroup has the usual [angular momentum](../../../../../angular-momentum.md) components $L=q\times p$, with $\{L_i,L_j\}=\varepsilon_{ijk}L_k$. The remaining unitary generators supply the other conserved quadratic observables, with their signs fixed by the stated choice of complex coordinates and Hamiltonian convention.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
