# Paper 50

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_50.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_50.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 50](paper-50.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

There is a small domain issue in the printed notation. If $\mathbb R^3/\mathbb R^2$ means a [quotient vector space](../../../vector-space.md#quotient-vector-space) by the horizontal plane, the displayed formula does not descend to that [quotient vector space](../../../vector-space.md#quotient-vector-space): $(0,0,0)$ and $(1,0,0)$ represent the same class but give different values. The intended construction is [stereographic projection](../../../complex-analysis.md#stereographic-projection), restricted to the unit [sphere](../../../geometry-and-topology.md#sphere) with the north pole removed. Interpreting the slash as removal of the plane $z=1$ also supplies a suitable ambient domain. The [holomorphic stereographic atlas of the sphere](../../../complex-analysis.md#holomorphic-stereographic-atlas-of-the-sphere) is obtained as follows.

Write $N=(0,0,1)$ and $S=(0,0,-1)$. On $U_N=S^2\setminus\{N\}$ use $\zeta=(x+iy)/(1-z)$. Its inverse, with $\zeta=u+iv$, is

$$
x=\frac{2u}{1+u^2+v^2},\qquad
y=\frac{2v}{1+u^2+v^2},\qquad
z=\frac{u^2+v^2-1}{1+u^2+v^2}.
$$

These formulas give a smooth [manifold chart](../../../differential-geometry.md#manifold-chart) from $U_N$ onto $\mathbb C$. On $U_S=S^2\setminus\{S\}$ choose the second [manifold chart](../../../differential-geometry.md#manifold-chart)

$$
\eta=\frac{x-iy}{1+z}.
$$

Its inverse is $x=2\operatorname{Re}\eta/(1+|\eta|^2)$, $y=-2\operatorname{Im}\eta/(1+|\eta|^2)$ and $z=(1-|\eta|^2)/(1+|\eta|^2)$, so this is also a smooth [manifold chart](../../../differential-geometry.md#manifold-chart) onto $\mathbb C$. The conjugation in this second [stereographic projection](../../../complex-analysis.md#stereographic-projection) is essential. On the overlap, $x^2+y^2=1-z^2$, so

$$
\zeta\eta=\frac{x^2+y^2}{1-z^2}=1,\qquad
\boxed{\eta=\zeta^{-1}}.
$$

Both directions of this transition are [holomorphic maps](../../../complex-analysis.md#holomorphic-map) on $\mathbb C^\times$, with nonzero derivative. The two [manifold charts](../../../differential-geometry.md#manifold-chart) cover the [sphere](../../../geometry-and-topology.md#sphere), hence define a [holomorphic atlas](../../../complex-geometry.md#holomorphic-atlas), giving precisely the [Riemann sphere](../../../complex-analysis.md#riemann-sphere). If one instead used $x+iy$ in both [manifold charts](../../../differential-geometry.md#manifold-chart), the transition would be $1/\bar\zeta$ and would not be [holomorphic](../../../complex-analysis.md#complex-differentiability-at-a-point).

Orient the [sphere](../../../geometry-and-topology.md#sphere) by this [holomorphic atlas](../../../complex-geometry.md#holomorphic-atlas). The given [volume form](../../../differential-form.md#volume-form) is smooth at infinity: replacing $\zeta$ by $1/\eta$ in its [exterior product](../../../linear-algebra.md#exterior-product) gives the same expression

$$
\Omega=\frac{i\,d\eta\wedge d\bar\eta}{(1+|\eta|^2)^2}.
$$

Moreover, $i\,d\zeta\wedge d\bar\zeta=2\,du\wedge dv$, so the normalization of this [volume form](../../../differential-form.md#volume-form) is

$$
\int_{S^2}\Omega
=2\int_0^{2\pi}\int_0^\infty\frac{r}{(1+r^2)^2}\,dr\,d\theta
=2\pi.
$$

Thus the printed [volume form](../../../differential-form.md#volume-form) has half the area of the standard round unit [sphere](../../../geometry-and-topology.md#sphere); replacing its integral by $4\pi$ would introduce an erroneous factor of two.

For $k\ge1$, the [holomorphic map](../../../complex-analysis.md#holomorphic-map) $f(\zeta)=\zeta^k$ extends over infinity, since the target reciprocal coordinate is $\eta^k$ when the source reciprocal coordinate is $\eta$. Its [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) is

$$
f^*\Omega=\frac{i\,k^2|\zeta|^{2k-2}\,d\zeta\wedge d\bar\zeta}
{(1+|\zeta|^{2k})^2}.
$$

Using $s=r^{2k}$ gives

$$
\int_{S^2}f^*\Omega
=4\pi k^2\int_0^\infty\frac{r^{2k-1}}{(1+r^{2k})^2}\,dr
=2\pi k\int_0^\infty\frac{ds}{(1+s)^2}
=2\pi k.
$$

The [degree of a map between oriented manifolds](../../../homology.md#degree-of-a-map-between-oriented-manifolds) is therefore

$$
\boxed{\deg f=\frac{\int_{S^2}f^*\Omega}{\int_{S^2}\Omega}=k}.
$$

For $k=0$, the formula on the finite [manifold chart](../../../differential-geometry.md#manifold-chart) is the constant $1$. Its unique continuous extension is also $1$ at infinity, rather than an undefined expression $\infty^0$. Its [pullback of a differential form](../../../differential-form.md#pullback-of-a-differential-form) is zero and its [degree of a map between oriented manifolds](../../../homology.md#degree-of-a-map-between-oriented-manifolds) is **zero**.

For the preimage calculation when $k\ge1$, choose a [regular value](../../../differential-geometry.md#regular-value) $w\in\mathbb C^\times$. There are exactly $k$ distinct roots of $\zeta^k=w$. At each root the real [Jacobian determinant](../../../calculus.md#jacobian-determinant) is $|k\zeta^{k-1}|^2>0$, so every local contribution to the [degree of a map between oriented manifolds](../../../homology.md#degree-of-a-map-between-oriented-manifolds) is $+1$. Their sum is $k$, agreeing with the integral. The exceptional values $0$ and infinity are avoided because they are branch values when $k>1$. For the constant map, any $w\ne1$ is a [regular value](../../../differential-geometry.md#regular-value) with no preimages, giving the same answer zero. This establishes the [degree of a power map of the Riemann sphere](../../../complex-analysis.md#degree-of-a-power-map-of-the-riemann-sphere) for every allowed $k$.

## 2

↑ **Parent:** [Paper 50](paper-50.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The geometric object underlying an $SU(2)$ [gauge field](../../../relativistic-quantum-field.md#gauge-field) is a [principal connection](../../../fiber-bundle.md#connection-principal-bundle) on a [principal bundle](../../../fiber-bundle.md#principal-bundle) $P\to M$ with structure group [SU(2)](../../../topological-group.md#su-2-group). The base $M$ is spacetime, or an oriented [Riemannian manifold](../../../riemannian-geometry.md#riemannian-manifold) in the Euclidean formulation. A choice of local section identifies each fibre with [SU(2)](../../../topological-group.md#su-2-group) and produces a local [gauge potential](../../../relativistic-quantum-field.md#gauge-field). Such a choice is a choice of internal frame; changing it produces a [gauge equivalence of principal connections](../../../fiber-bundle.md#gauge-equivalence-of-principal-connections). The bundle specifies the global gluing of these frames, while the [principal connection](../../../fiber-bundle.md#connection-principal-bundle) specifies how frames at neighbouring points are compared.

The [SU(2)](../../../topological-group.md#su-2-group) group consists of $2\times2$ [unitary matrices](../../../linear-operator-theory.md#unitary-matrix) of [determinant](../../../linear-algebra.md#determinant) one. Its [Lie algebra](../../../lie-algebra.md) consists of traceless [Skew-Hermitian](../../../linear-operator-theory.md#skew-hermitian-matrix) matrices. For definiteness use

$$
t_a=-\frac{i}{2}\sigma_a,\qquad
[t_a,t_b]=\epsilon_{abc}t_c,\qquad
-\operatorname{tr}(t_at_b)=\frac12\delta_{ab},
$$

where the $\sigma_a$ are [Pauli matrices](../../../algebra.md#pauli-matrices). The [commutator](../../../lie-algebra.md#commutator) fixes all signs below. The positive invariant inner product on this [Lie algebra](../../../lie-algebra.md) is $-\operatorname{tr}(XY)$. Absorb the coupling into the [gauge potential](../../../relativistic-quantum-field.md#gauge-field), so the [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) in the defining two-dimensional representation is $D=d+A$ with $A=A^at_a$. A convention using Hermitian [Pauli matrices](../../../algebra.md#pauli-matrices) instead moves factors of $i$ and the coupling into $D$; the underlying [principal connection](../../../fiber-bundle.md#connection-principal-bundle) is the same geometric data.

A [principal connection](../../../fiber-bundle.md#connection-principal-bundle) can be given by a [Lie algebra](../../../lie-algebra.md)-valued [differential one-form](../../../differential-form.md#one-form) $\mathcal A$ on $P$ satisfying

$$
\mathcal A(\xi_P)=\xi,\qquad
R_h^*\mathcal A=\operatorname{Ad}_{h^{-1}}\mathcal A.
$$

Here $\xi_P$ is the vertical vector generated by the right group action. The first identity recovers vertical motion and the second makes the construction independent of a fibre frame. Its kernel is the [horizontal distribution of a principal connection](../../../fiber-bundle.md#horizontal-distribution-of-a-principal-connection), complementary to the vertical tangent spaces. A curve is horizontal when $\mathcal A$ annihilates its velocity, so a [principal connection](../../../fiber-bundle.md#connection-principal-bundle) defines [parallel transport](../../../fiber-bundle.md#parallel-transport) along curves in $M$.

For a local section $s$, the [local principal connection form](../../../fiber-bundle.md#local-principal-connection-form) is $A=s^*\mathcal A$. Change the section to $s'=sh$, with $h:U\to SU(2)$. Differentiating $sh$ has a translated horizontal part and a vertical part from $dh$. The two defining identities for the [principal connection](../../../fiber-bundle.md#connection-principal-bundle) therefore give

$$
\boxed{A'=h^{-1}Ah+h^{-1}dh}.
$$

On overlapping trivializations this is exactly the compatibility law for the [local principal connection forms](../../../fiber-bundle.md#local-principal-connection-form). In particular, the [gauge potentials](../../../relativistic-quantum-field.md#gauge-field) need not glue as ordinary globally defined [differential one-forms](../../../differential-form.md#one-form) on $M$. On a nontrivial [principal bundle](../../../fiber-bundle.md#principal-bundle) there need not be any global section with respect to which one could write a single matrix-valued $A$.

An active [gauge equivalence of principal connections](../../../fiber-bundle.md#gauge-equivalence-of-principal-connections) is generated by a bundle automorphism covering the identity on $M$ and commuting with the right [SU(2)](../../../topological-group.md#su-2-group) action. Its local description has the same transformation formula, but its local group-valued functions must satisfy transition compatibility on overlaps. This distinguishes the structure group [SU(2)](../../../topological-group.md#su-2-group) from the full [gauge group](../../../relativistic-quantum-field.md#gauge-group) of a fixed bundle. Two descriptions related by a passive change of section encode the same [principal connection](../../../fiber-bundle.md#connection-principal-bundle); two connections related by such an automorphism lie in the same physical [gauge orbit](../../../relativistic-quantum-field.md#gauge-orbit). The space of [principal connections](../../../fiber-bundle.md#connection-principal-bundle) on a fixed bundle is affine: the difference of two connection forms is a [differential one-form](../../../differential-form.md#one-form) with values in the [adjoint bundle](../../../fiber-bundle.md#adjoint-bundle), since their inhomogeneous transformation terms cancel.

The [curvature of a principal connection](../../../fiber-bundle.md#curvature-of-a-principal-connection) is

$$
\mathcal F=d\mathcal A+\tfrac12[\mathcal A\wedge\mathcal A].
$$

It is horizontal and equivariant, hence descends to a [differential two-form](../../../differential-form.md#2-form) on $M$ valued in the [adjoint bundle](../../../fiber-bundle.md#adjoint-bundle). In a local section the [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength) becomes

$$
F=dA+A\wedge A
=\frac12F_{\mu\nu}\,dx^\mu\wedge dx^\nu,\qquad
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu].
$$

The product $A\wedge A$ combines the [exterior product](../../../linear-algebra.md#exterior-product) with matrix multiplication. The [commutator](../../../lie-algebra.md#commutator) term is the specifically non-Abelian interaction. Substitution of the transformation of $A$, using $d(h^{-1})=-h^{-1}(dh)h^{-1}$, cancels all derivatives of $h$ and gives

$$
\boxed{F'=h^{-1}Fh}.
$$

Thus the [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength) transforms tensorially even though the [gauge potential](../../../relativistic-quantum-field.md#gauge-field) does not. Geometrically, the [curvature of a principal connection](../../../fiber-bundle.md#curvature-of-a-principal-connection) measures the failure of the [horizontal distribution of a principal connection](../../../fiber-bundle.md#horizontal-distribution-of-a-principal-connection) to be integrable; physically it is the non-Abelian [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength).

Matter fields are sections of [associated vector bundles](../../../fiber-bundle.md#associated-vector-bundle). A field in the defining representation of [SU(2)](../../../topological-group.md#su-2-group) is a section of $E=P\times_{SU(2)}\mathbb C^2$. Its two local components satisfy $\psi'=h^{-1}\psi$ under the section convention above. The induced [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) obeys

$$
D'\psi'=(d+A')(h^{-1}\psi)=h^{-1}(d+A)\psi.
$$

This covariance is why replacing ordinary derivatives by [gauge covariant derivatives](../../../relativistic-quantum-field.md#gauge-covariant-derivative) makes the [kinetic terms](../../../quantum-field-theory.md#kinetic-term) compatible with changes of internal frame. Applying the [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) twice yields $D^2\psi=F\psi$, so the [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength) also measures the noncommutativity of covariant differentiation. Other [group representations](../../../representation-theory.md#group-representation) give other [associated vector bundles](../../../fiber-bundle.md#associated-vector-bundle) and replace $A$ by its image under the differential of the representation.

For an adjoint-valued [differential form](../../../differential-form.md) $\Phi$ of degree $r$, set

$$
D_A\Phi=d\Phi+A\wedge\Phi-(-1)^r\Phi\wedge A.
$$

Expansion of $F=dA+A\wedge A$, using $d^2=0$, proves the [gauge-theory Bianchi identity](../../../relativistic-quantum-field.md#gauge-theory-bianchi-identity)

$$
\boxed{D_AF=dF+A\wedge F-F\wedge A=0}.
$$

This is an identity for every [principal connection](../../../fiber-bundle.md#connection-principal-bundle), independent of any field equation. It should be distinguished from the dynamical [Yang-Mills equations](../../../relativistic-quantum-field.md#yang-mills-equations).

To obtain dynamics, equip $M$ with a [Riemannian metric](../../../differential-geometry.md#riemannian-metric) and an orientation, and let $*$ be its [Hodge star operator](../../../differential-form.md#hodge-star-operator). With the [Skew-Hermitian](../../../linear-operator-theory.md#skew-hermitian-matrix) normalization above, the positive Euclidean [Yang-Mills action](../../../relativistic-quantum-field.md#yang-mills-action) is

$$
S[A]=-\frac1{g_{\mathrm{YM}}^2}\int_M\operatorname{tr}(F\wedge *F).
$$

The [matrix trace](../../../linear-algebra.md#matrix-trace) and the [Hodge star operator](../../../differential-form.md#hodge-star-operator) make this independent of the choice of local section. The minus sign compensates for the negative trace form on [Skew-Hermitian](../../../linear-operator-theory.md#skew-hermitian-matrix) matrices. Varying the [principal connection](../../../fiber-bundle.md#connection-principal-bundle) gives $\delta F=D_A\delta A$, and therefore

$$
\delta S=-\frac{2}{g_{\mathrm{YM}}^2}
\int_M\operatorname{tr}(D_A\delta A\wedge *F).
$$

For compactly supported variations, or on a closed base, integration by parts gives the [Yang-Mills equations](../../../relativistic-quantum-field.md#yang-mills-equations)

$$
\boxed{D_A*F=0}.
$$

In components these are $D_\mu F^{\mu\nu}=0$. The [gauge-theory Bianchi identity](../../../relativistic-quantum-field.md#gauge-theory-bianchi-identity) provides the complementary geometric identity $D_AF=0$. Coupling matter adds the associated gauge current to the dynamical equation; the transformation law of the [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) ensures covariance of that current as well.

The [principal connection](../../../fiber-bundle.md#connection-principal-bundle) also supplies nonlocal observables. Along a path $\gamma$, [parallel transport](../../../fiber-bundle.md#parallel-transport) is determined by

$$
\frac{d\psi}{dt}+A(\dot\gamma)\psi=0,\qquad
U_\gamma=\mathcal P\exp\left(-\int_\gamma A\right).
$$

The ordering is necessary because the [Lie algebra](../../../lie-algebra.md) matrices at different points need not commute. The resulting [Wilson line](../../../relativistic-quantum-field.md#wilson-line) transforms as $U_\gamma'=h(\gamma(1))^{-1}U_\gamma h(\gamma(0))$. For a closed path, its [matrix trace](../../../linear-algebra.md#matrix-trace) is a [Wilson loop](../../../relativistic-quantum-field.md#wilson-loop), independent of the frame at the basepoint. These observables record the [holonomy of a connection](../../../fiber-bundle.md#holonomy). A [flat principal connection](../../../fiber-bundle.md#flat-principal-connection) has trivial [holonomy of a connection](../../../fiber-bundle.md#holonomy) around sufficiently small contractible loops but may have nontrivial [holonomy of a connection](../../../fiber-bundle.md#holonomy) around noncontractible loops. Thus vanishing local [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength) need not eliminate global gauge information.

The global topology becomes particularly visible in four dimensions. For a closed oriented four-dimensional base, [Chern-Weil theory](../../../geometry-and-topology.md#chern-weil-homomorphism) gives the [Second Chern number](../../../geometry-and-topology.md#second-chern-number) of the defining [associated vector bundle](../../../fiber-bundle.md#associated-vector-bundle):

$$
k=c_2(E)[M]=\frac1{8\pi^2}\int_M\operatorname{tr}(F\wedge F)\in\mathbb Z.
$$

The plus sign here uses [Skew-Hermitian](../../../linear-operator-theory.md#skew-hermitian-matrix) curvature and the mathematical second-Chern convention: expanding $\det(I+iF/(2\pi))$ with $\operatorname{tr}F=0$ gives precisely the displayed [Second Chern form](../../../geometry-and-topology.md#second-chern-form). A convention defining a physics topological charge with a leading minus sign instead calls that charge $-k$. Neither choice changes the absolute-value action bound.

The [Second Chern number](../../../geometry-and-topology.md#second-chern-number) is independent of the [principal connection](../../../fiber-bundle.md#connection-principal-bundle) on a fixed bundle. Indeed, the [gauge-theory Bianchi identity](../../../relativistic-quantum-field.md#gauge-theory-bianchi-identity) implies

$$
\delta\operatorname{tr}(F\wedge F)
=2d\,\operatorname{tr}(\delta A\wedge F),
$$

whose integral vanishes on a closed base by [Stokes theorem](../../../calculus.md#stokes-theorem). A nonzero [Second Chern number](../../../geometry-and-topology.md#second-chern-number) obstructs a global trivialization: for a globally defined $A$, $\operatorname{tr}(F\wedge F)=d\,\operatorname{tr}(A\wedge dA+\tfrac23A\wedge A\wedge A)$, so its integral on a closed base would be zero. On $S^4$, gluing two trivial bundles over four-balls uses a transition map $S^3\to SU(2)$. Since [SU(2) as the three-sphere](../../../topological-group.md#su-2-as-the-three-sphere) identifies the target with $S^3$, such gluing maps have integer [degree of a map between oriented manifolds](../../../homology.md#degree-of-a-map-between-oriented-manifolds), illustrating how distinct topological sectors arise.

In four Euclidean dimensions, the [Hodge star operator](../../../differential-form.md#hodge-star-operator) squares to one on [differential two-forms](../../../differential-form.md#2-form). Decompose $F=F_++F_-$ with $*F_\pm=\pm F_\pm$. Define the nonnegative squared norms $a_\pm=-\int\operatorname{tr}(F_\pm\wedge *F_\pm)$. Orthogonality gives

$$
S=\frac{a_++a_-}{g_{\mathrm{YM}}^2},\qquad
8\pi^2k=-a_++a_-,
\qquad
\boxed{S\ge\frac{8\pi^2}{g_{\mathrm{YM}}^2}|k|}.
$$

Equality means that one component vanishes, giving the [self-dual Yang-Mills equations](../../../classical-field-theory-soliton.md#self-dual-yang-mills-equations) or the [Anti-self-dual Yang-Mills equations](../../../classical-field-theory-soliton.md#anti-self-dual-yang-mills-equations). Such finite-action solutions are [Yang-Mills instantons](../../../classical-field-theory-soliton.md#yang-mills-instanton). They solve the full [Yang-Mills equations](../../../relativistic-quantum-field.md#yang-mills-equations) because $D_A*F=\pm D_AF=0$. With the second-Chern convention just specified, anti-self-dual curvature has $k\ge0$ and self-dual curvature has $k\le0$. On noncompact spacetime one must impose suitable decay or boundary conditions before treating the topological integral as an integer and using the same bound without boundary terms.

**Local [gauge potentials](../../../relativistic-quantum-field.md#gauge-field), matter [gauge covariant derivatives](../../../relativistic-quantum-field.md#gauge-covariant-derivative), [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength), [parallel transport](../../../fiber-bundle.md#parallel-transport) and [Second Chern number](../../../geometry-and-topology.md#second-chern-number) are different manifestations of one [principal connection](../../../fiber-bundle.md#connection-principal-bundle).** The [principal bundle](../../../fiber-bundle.md#principal-bundle) preserves the global information that a single local [gauge potential](../../../relativistic-quantum-field.md#gauge-field) cannot capture; the [Yang-Mills action](../../../relativistic-quantum-field.md#yang-mills-action) then selects its physical dynamics.

## 3

↑ **Parent:** [Paper 50](paper-50.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Acting on the column $(x,1)^T$ gives the faithful [Matrix Lie group](../../../lie-theory.md#matrix-lie-group) representation

$$
\begin{pmatrix}e^\alpha&\beta\\0&1\end{pmatrix}
\begin{pmatrix}x\\1\end{pmatrix}
=\begin{pmatrix}e^\alpha x+\beta\\1\end{pmatrix}.
$$

Multiplication and inversion are

$$
(\alpha,\beta)(a,b)=(\alpha+a,\beta+e^\alpha b),\qquad
(\alpha,\beta)^{-1}=(-\alpha,-e^{-\alpha}\beta).
$$

Thus $G$ is the [real affine group](../../../lie-theory.md#orientation-preserving-affine-group-of-the-real-line). Differentiating the matrices at the identity gives its [Lie algebra](../../../lie-algebra.md)

$$
\mathfrak g=\left\{\begin{pmatrix}a&b\\0&0\end{pmatrix}:a,b\in\mathbb R\right\}.
$$

With

$$
D=\begin{pmatrix}1&0\\0&0\end{pmatrix},\qquad
T=\begin{pmatrix}0&1\\0&0\end{pmatrix},
$$

the matrix [commutator](../../../lie-algebra.md#commutator) is **$[D,T]=T$**, and $[D,D]=[T,T]=0$.

The left [Maurer-Cartan form](../../../lie-theory.md#maurer-cartan-form) and its right analogue are

$$
\theta_L=g^{-1}dg
=\begin{pmatrix}d\alpha&e^{-\alpha}d\beta\\0&0\end{pmatrix}
=D\,d\alpha+T\,e^{-\alpha}d\beta,
$$



$$
\theta_R=dg\,g^{-1}
=\begin{pmatrix}d\alpha&d\beta-\beta\,d\alpha\\0&0\end{pmatrix}
=D\,d\alpha+T(d\beta-\beta\,d\alpha).
$$

For a constant $h$, left translation leaves $\theta_L$ unchanged, and right translation leaves $\theta_R$ unchanged. Taking their dual [vector fields](../../../calculus.md#vector-field) gives

$$
\boxed{D_L=\partial_\alpha,\qquad T_L=e^\alpha\partial_\beta},
\qquad
\boxed{D_R=\partial_\alpha+\beta\partial_\beta,\qquad T_R=\partial_\beta}.
$$

The first pair consists of [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field); the second consists of [right-invariant vector fields](../../../lie-theory.md#right-invariant-vector-field). These are the [invariant frames of the real affine group](../../../lie-theory.md#invariant-frames-of-the-real-affine-group). Computing their [Lie brackets of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) yields

$$
[D_L,T_L]=T_L,\qquad [D_R,T_R]=-T_R.
$$

All brackets of a field with itself vanish. The sign difference is necessary: evaluation at the identity identifies [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field) with the matrix [Lie algebra](../../../lie-algebra.md) as a homomorphism, whereas [right-invariant vector fields realize the opposite Lie algebra](../../../lie-theory.md#right-invariant-vector-fields-realize-the-opposite-lie-algebra). Equivalently, $\xi\mapsto-\xi_R$ is a homomorphism for the same matrix [commutator](../../../lie-algebra.md#commutator). There is no convention in which these particular coordinate fields both have the positive structure constant while retaining the usual [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields).

The [Maurer-Cartan equation](../../../lie-theory.md#maurer-cartan-equation) gives the same check. If $\theta_L=D\ell^D+T\ell^T$, then

$$
d\ell^D=0,\qquad d\ell^T=-\ell^D\wedge\ell^T.
$$

For $\theta_R=Dr^D+Tr^T$, instead

$$
dr^D=0,\qquad dr^T=r^D\wedge r^T.
$$

Thus the left equation is $d\theta_L+\theta_L\wedge\theta_L=0$ and the right equation is $d\theta_R-\theta_R\wedge\theta_R=0$, explaining the opposite bracket signs directly.

Finally, the two given matrix curves are $\exp(\epsilon T)$ and $\exp(\epsilon D)$. Their left action on a general group element is

$$
g_1(\epsilon)g(\alpha,\beta)=g(\alpha,\beta+\epsilon),\qquad
g_2(\epsilon)g(\alpha,\beta)=g(\alpha+\epsilon,e^\epsilon\beta).
$$

Differentiating at $\epsilon=0$ gives $T_R$ and $D_R$ respectively. Hence **[Left translations on a Lie group](../../../lie-theory.md#left-and-right-translation-on-a-lie-group) are generated by [right-invariant vector fields](../../../lie-theory.md#right-invariant-vector-field)**. More generally, the velocity of $\exp(t\xi)g$ is $(dR_g)_e\xi$, which is right-invariant because left and right multiplication commute. In the other direction, the flows $g\exp(t\xi)$ generate [left-invariant vector fields](../../../lie-theory.md#left-invariant-vector-field) and are [right translations on a Lie group](../../../lie-theory.md#left-and-right-translation-on-a-lie-group).

## 4

↑ **Parent:** [Paper 50](paper-50.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $\pi:T^*M\to M$ be the [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle) projection. Its [canonical one-form on a cotangent bundle](../../../symplectic-geometry.md#canonical-one-form-on-a-cotangent-bundle) is defined intrinsically by $\lambda_{(x,p)}(V)=p(d\pi(V))$, so locally $\lambda=p_i\,dx^i$. Choose the position-first [symplectic form](../../../symplectic-geometry.md#symplectic-form)

$$
\omega=-d\lambda=dx^i\wedge dp_i.
$$

It is closed by $d^2=0$ and nondegenerate, since contraction with $a^i\partial_{x^i}+b_i\partial_{p_i}$ is $a^i dp_i-b_i dx^i$, which vanishes only when both coefficient sets vanish. The intrinsic definition of $\lambda$ makes this [symplectic form](../../../symplectic-geometry.md#symplectic-form) independent of coordinates.

Use the convention $\iota_{X_H}\omega=dH$. Then the [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) and the [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) are

$$
X_H=\frac{\partial H}{\partial p_i}\partial_{x^i}
-\frac{\partial H}{\partial x^i}\partial_{p_i},
\qquad
\{F,G\}=\frac{\partial F}{\partial x^i}\frac{\partial G}{\partial p_i}
-\frac{\partial F}{\partial p_i}\frac{\partial G}{\partial x^i},
$$

so $X_H(F)=\{F,H\}$. Choosing $\omega=d\lambda$ and $\iota_{X_H}\omega=-dH$ gives the same equations; choosing only one of these sign changes would reverse the flow.

For the [geodesic Hamiltonian](../../../riemannian-geometry.md#geodesic-hamiltonian), [Hamilton's equations](../../../classical-mechanics.md#hamilton-s-equations) give

$$
\dot x^i=g^{ij}p_j,\qquad
\dot p_i=-\frac12(\partial_i g^{jk})p_jp_k.
$$

Put $v^i=\dot x^i$, so $p_i=g_{ij}v^j$. Differentiating $g^{jk}g_{ka}=\delta^j_a$ gives

$$
(\partial_i g^{jk})p_jp_k=-(\partial_i g_{ab})v^av^b.
$$

Consequently,

$$
g_{ij}\ddot x^j+(\partial_k g_{ij})v^kv^j
=\frac12(\partial_i g_{ab})v^av^b.
$$

Symmetrizing the velocity factors and raising the first index converts this to

$$
\boxed{\ddot x^\ell+\Gamma^\ell{}_{jk}\dot x^j\dot x^k=0},
\qquad
\Gamma^\ell{}_{jk}=\frac12g^{\ell i}
(\partial_jg_{ik}+\partial_kg_{ij}-\partial_ig_{jk}).
$$

These [Christoffel symbols](../../../riemannian-geometry.md#christoffel-symbol) are those of the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection). Thus a Hamiltonian [integral curve of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) projects to an affinely parametrized [geodesic](../../../riemannian-geometry.md#geodesic). Conversely, an affinely parametrized [geodesic](../../../riemannian-geometry.md#geodesic) lifts by $p_i=g_{ij}\dot x^j$ to an [integral curve of a vector field](../../../calculus.md#integral-curve-of-a-vector-field) of $X_H$, since reversing the calculation proves both [Hamilton's equations](../../../classical-mechanics.md#hamilton-s-equations). This is the [geodesic flow](../../../riemannian-geometry.md#geodesic-flow) on the [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle). The conserved [Hamiltonian](../../../classical-mechanics.md#hamiltonian) is half the squared speed, and the zero-energy case gives the constant [geodesics](../../../riemannian-geometry.md#geodesic).

A quadratic [homogeneous polynomial](../../../algebra.md#homogeneous-polynomial) depends only on the symmetric part of its coefficient matrix. Accordingly take its unique [symmetric coefficients of a quadratic polynomial](../../../linear-algebra.md#symmetric-coefficients-of-a-quadratic-polynomial), $K^{ij}=K^{ji}$. This is the standard implicit convention in identifying such polynomials with [symmetric tensors](../../../linear-algebra.md#symmetric-tensor). If an arbitrary nonsymmetric representative were allowed, the literal equivalence would fail: in Euclidean $\mathbb R^2$, $K^{12}=x^1$, $K^{21}=-x^1$ and all other components zero give the zero polynomial, which has zero [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) with every function, whereas the lowered coefficient array is not a [Killing tensor](../../../riemannian-geometry.md#killing-tensor) because it is not symmetric.

Lower the indices of the symmetric coefficient tensor using the [Riemannian metric](../../../differential-geometry.md#riemannian-metric). Since $p_i=g_{ij}v^j$,

$$
K^{ij}p_ip_j=K_{ij}v^iv^j.
$$

Along an affinely parametrized [geodesic](../../../riemannian-geometry.md#geodesic), [metric compatibility](../../../fiber-bundle.md#metric-compatibility) and $\nabla_vv=0$ imply

$$
\frac{d}{dt}(K_{ij}v^iv^j)
=(\nabla_aK_{bc})v^av^bv^c
=\nabla_{(a}K_{bc)}\,v^av^bv^c.
$$

Here parentheses mean normalized symmetrization over all indicated indices. The left side is $\{K,H\}$ by the [Hamiltonian vector field](../../../symplectic-geometry.md#hamiltonian-vector-field) convention. Therefore a [rank-two Killing tensor](../../../riemannian-geometry.md#rank-two-killing-tensor), defined by symmetry and $\nabla_{(a}K_{bc)}=0$, gives a [quadratic geodesic first integral](../../../riemannian-geometry.md#quadratic-geodesic-first-integral).

Conversely, if $\{K,H\}=0$ everywhere on $T^*M$, the last cubic expression vanishes for every $v$ at every point, because the [Riemannian metric](../../../differential-geometry.md#riemannian-metric) identifies tangent and cotangent spaces invertibly. A symmetric trilinear form is determined by its diagonal cubic polynomial: equivalently, compare its coefficients, or polarize the cubic. Hence $\nabla_{(a}K_{bc)}=0$. This proves both directions:

$$
\boxed{\{K,H\}=0\quad\Longleftrightarrow\quad
K_{ij}=K_{ji}\ \text{and}\ \nabla_{(a}K_{bc)}=0}
$$

with symmetry understood on the coefficient representative from the outset. The equivalence is local and does not require [geodesic completeness](../../../riemannian-geometry.md#geodesic-completeness).

For the final construction, the antisymmetric [differential two-form](../../../differential-form.md#2-form) $Y$ is a [Killing-Yano two-form](../../../riemannian-geometry.md#killing-yano-two-form). Its defining equation says $\nabla_aY_{bc}=-\nabla_bY_{ac}$. Antisymmetry of $Y$ also says $\nabla_aY_{bc}=-\nabla_aY_{cb}$, so the three-index tensor $\nabla_aY_{bc}$ is totally antisymmetric.

The proposed tensor is symmetric, since it is the inner product of the covectors $Y_{i\cdot}$ and $Y_{j\cdot}$:

$$
K_{ij}=g^{k\ell}Y_{ik}Y_{j\ell}=K_{ji}.
$$

There is a useful geometric proof of its [Killing tensor](../../../riemannian-geometry.md#killing-tensor) equation. Along any affinely parametrized [geodesic](../../../riemannian-geometry.md#geodesic), define $w_k=Y_{ik}v^i$. Then

$$
\nabla_vw_k=v^av^i\nabla_aY_{ik}+Y_{ik}\nabla_vv^i=0.
$$

The first term vanishes by antisymmetry in $a,i$, and the second by the [geodesic](../../../riemannian-geometry.md#geodesic) equation. Thus $w$ is carried by [parallel transport](../../../fiber-bundle.md#parallel-transport). By [metric compatibility](../../../fiber-bundle.md#metric-compatibility), its squared norm is constant, and

$$
|w|^2=g^{k\ell}Y_{ik}Y_{j\ell}v^iv^j=K_{ij}v^iv^j.
$$

Every tangent vector is the initial velocity of a local [geodesic](../../../riemannian-geometry.md#geodesic), so differentiation at the initial point gives $\nabla_{(a}K_{bc)}v^av^bv^c=0$ for every $v$. The same cubic-coefficient argument proves

$$
\boxed{\nabla_{(a}K_{bc)}=0}.
$$

This proves that the [square of a Killing-Yano two-form](../../../riemannian-geometry.md#square-of-a-killing-yano-two-form) is a [rank-two Killing tensor](../../../riemannian-geometry.md#rank-two-killing-tensor) and supplies a nonnegative [quadratic geodesic first integral](../../../riemannian-geometry.md#quadratic-geodesic-first-integral). The argument also explains the conserved quantity: it is the squared norm of a covector that the [Killing-Yano two-form](../../../riemannian-geometry.md#killing-yano-two-form) makes parallel along every [geodesic](../../../riemannian-geometry.md#geodesic).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
