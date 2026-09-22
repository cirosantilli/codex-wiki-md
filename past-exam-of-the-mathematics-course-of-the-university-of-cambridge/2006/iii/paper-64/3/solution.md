<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use $\omega=\sum_i dq_i\wedge dp_i$, $\iota_{X_f}\omega=df$ and

$$
\{f,g\}=\sum_i\left(\frac{\partial f}{\partial q_i}\frac{\partial g}{\partial p_i}-\frac{\partial f}{\partial p_i}\frac{\partial g}{\partial q_i}\right).
$$

Then $X_f(g)=\{g,f\}$ and $[X_f,X_g]=-X_{\{f,g\}}$. For a left [group action](../../../../../group-action.md), let $\xi_P(p)=\left.\frac{d}{dt}\right|_0\exp(t\xi)\cdot p$; its fundamental fields obey $[\xi_P,\eta_P]=-[\xi,\eta]_P$.

The components of a [moment map](../../../../../moment-map.md) satisfy

$$
\mu_\xi(p)=\langle\mu(p),\xi\rangle,\qquad
d\mu_\xi=\iota_{\xi_P}\omega.
$$

Thus $\xi_P=X_{\mu_\xi}$. A [Hamiltonian](../../../../../hamiltonian.md) [moment map](../../../../../moment-map.md) additionally has coadjoint equivariance,

$$
\mu(gp)=\operatorname{Ad}_{g^{-1}}^*\mu(p).
$$

Here the right side evaluates on $\xi$ as $\langle\mu(p),\operatorname{Ad}_{g^{-1}}\xi\rangle$. With that convention its infinitesimal form is $\{\mu_\xi,\mu_\eta\}=\mu_{[\xi,\eta]}$. Some definitions reserve “[moment map](../../../../../moment-map.md)” for this equivariant version; choosing Hamiltonians for every generator first gives a [weakly Hamiltonian action](../../../../../weakly-hamiltonian-action.md).

To derive the obstruction, compare the two antihomomorphism identities:

$$
X_{\{\mu_\xi,\mu_\eta\}-\mu_{[\xi,\eta]}}=0.
$$

On connected $P$, nondegeneracy of $\omega$ makes

$$
\kappa(\xi,\eta)=\{\mu_\xi,\mu_\eta\}-\mu_{[\xi,\eta]}
$$

a constant alternating bilinear form. The two Jacobi identities imply

$$
\kappa([\xi,\eta],\zeta)+\kappa([\eta,\zeta],\xi)+\kappa([\zeta,\xi],\eta)=0.
$$

Replacing $\mu_\xi$ by $\mu_\xi+b(\xi)$ changes $\kappa$ to $\kappa-b([\xi,\eta])$. Thus vanishing of this class in [Lie algebra cohomology](../../../../../lie-algebra-cohomology.md) is the precise [moment-map equivariance obstruction](../../../../../moment-map-equivariance-obstruction.md). In particular **a connected group with $H^2(\mathfrak g,\mathbb R)=0$ permits constants to be chosen so that the component [Poisson algebra](../../../../../poisson-algebra.md) is the [Lie algebra](../../../../../lie-algebra-split.md)**. A locally effective action makes this realization faithful; otherwise it realizes the quotient by the infinitesimal kernel. The linear span of the components has the Lie brackets; the entire algebra of polynomial products of them is, of course, larger.

A useful sufficient condition is semisimplicity, which can be proved here without assuming the desired equivariance. Let $B$ be the nondegenerate [Killing form](../../../../../killing-form.md) and define $D$ by $B(D\xi,\eta)=\kappa(\xi,\eta)$. Invariance of $B$ and the cocycle identity give

$$
B(D[\xi,\eta],\zeta)
=B(D\xi,[\eta,\zeta])+B(D\eta,[\zeta,\xi])
=B([D\xi,\eta]+[\xi,D\eta],\zeta),
$$

so $D$ is a derivation. Choose $Z$ uniquely by $B(Z,\xi)=\operatorname{tr}(D\operatorname{ad}\xi)$. Since $[D,\operatorname{ad}\xi]=\operatorname{ad}(D\xi)$, cyclicity of trace gives

$$
\begin{aligned}
B([Z,\xi],\eta)
&=B(Z,[\xi,\eta])
=\operatorname{tr}\bigl(D[\operatorname{ad}\xi,\operatorname{ad}\eta]\bigr)\\
&=\operatorname{tr}\bigl([D,\operatorname{ad}\xi]\operatorname{ad}\eta\bigr)
=B(D\xi,\eta).
\end{aligned}
$$

Hence $D=\operatorname{ad}Z$ and $\kappa(\xi,\eta)=B(Z,[\xi,\eta])$. The shift $b(\xi)=B(Z,\xi)$ removes the obstruction. This proves [semisimple moment-map equivariance](../../../../../semisimple-moment-map-equivariance.md); for connected $G$ infinitesimal equivariance integrates along its one-parameter subgroups to group equivariance. It does not claim that arbitrary symplectic actions of arbitrary groups have [moment maps](../../../../../moment-map.md).

For the Kepler calculation, put $k=Mm$ and work on $r=|\mathbf r|>0$, since the [Hamiltonian](../../../../../hamiltonian.md) is singular at the origin. The [Hamilton equations](../../../../../hamilton-s-equations.md) are

$$
\dot{\mathbf r}=\mathbf p,\qquad
\dot{\mathbf p}=-k\frac{\mathbf r}{r^3}.
$$

The [angular momentum](../../../../../angular-momentum.md) therefore obeys

$$
\dot{\mathbf L}=\mathbf p\times\mathbf p+\mathbf r\times\dot{\mathbf p}=0.
$$

For the [Runge-Lenz vector](../../../../../laplace-runge-lenz-vector.md),

$$
\dot{\mathbf K}=\dot{\mathbf p}\times\mathbf L
-k\left(\frac{\mathbf p}{r}-\frac{\mathbf r(\mathbf r\cdot\mathbf p)}{r^3}\right).
$$

The [vector triple product identity](../../../../../vector-triple-product.md) gives $\mathbf r\times\mathbf L=\mathbf r(\mathbf r\cdot\mathbf p)-r^2\mathbf p$. Therefore

$$
\dot{\mathbf p}\times\mathbf L
=k\frac{\mathbf p}{r}-k\frac{\mathbf r(\mathbf r\cdot\mathbf p)}{r^3},
$$

and the terms cancel. Since $\dot f=\{f,H\}$, this proves

$$
\boxed{\{L_i,H\}=\{K_i,H\}=0.}
$$

The conserved quantities consequently generate transformations preserving energy. Their brackets give the [Kepler dynamical symmetry algebra](../../../../../kepler-dynamical-symmetry-algebra.md). On $H<0$, define $\mathbf A=\mathbf K/\sqrt{-2H}$ as a function on that whole open region. Because $H$ Poisson commutes with both vectors, its brackets are

$$
\{L_i,L_j\}=\epsilon_{ijk}L_k,\qquad
\{L_i,A_j\}=\epsilon_{ijk}A_k,\qquad
\{A_i,A_j\}=\epsilon_{ijk}L_k.
$$

With $\mathbf J_\pm=(\mathbf L\pm\mathbf A)/2$ one obtains two commuting $\mathfrak{so}(3)$ algebras:

$$
\{J_{\pm i},J_{\pm j}\}=\epsilon_{ijk}J_{\pm k},\qquad
\{J_{+i},J_{-j}\}=0.
$$

Thus the negative-energy algebra is **$\mathfrak{so}(4)$**. On $H>0$, using $\mathbf A=\mathbf K/\sqrt{2H}$ instead changes the last bracket to $-\epsilon_{ijk}L_k$, yielding **$\mathfrak{so}(3,1)$**, with $\mathbf L$ rotations and $\mathbf A$ boosts. At zero energy the brackets of conserved functions on the characteristic orbit quotient give **$\mathfrak e(3)=\mathfrak{so}(3)\ltimes\mathbb R^3$**, with commuting $\mathbf K$.

There are two global qualifications. First, an energy hypersurface carries a [presymplectic form](../../../../../presymplectic-form.md): its restricted [two-form](../../../../../2-form.md) has characteristic direction $X_H$. At $H=0$, the literal vector fields of $\mathbf K$ need only commute modulo $X_H$, since differentiating $\{K_i,K_j\}=-2H\epsilon_{ijk}L_k$ still produces an $L_kX_H$ term. On nonzero-energy regions the energy-dependent normalization above gives an exact [Hamiltonian](../../../../../hamiltonian.md) [Lie algebra](../../../../../lie-algebra-split.md); one must differentiate that normalization before restricting to a level. Second, completeness is required for a global [group action](../../../../../group-action.md). The collision-excluded Kepler phase space need not have complete hidden-symmetry flows, so the brackets establish local actions (or the appropriate simply connected covers), not an unconditional global action on every unregularized trajectory. Collision regularization supplies the familiar global bound-motion symmetry; this distinction is developed in [https://math.berkeley.edu/~alanw/277papers00/tang.pdf](https://math.berkeley.edu/~alanw/277papers00/tang.pdf) . It does not change the three energy-dependent [Lie algebras](../../../../../lie-algebra-split.md) just derived.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
