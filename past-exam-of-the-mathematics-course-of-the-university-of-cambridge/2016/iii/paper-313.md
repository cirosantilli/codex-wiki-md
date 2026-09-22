# Paper 313

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_313.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_313.pdf)

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

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the orientation selected by the [volume form](../../../differential-form.md#volume-form), and let $\operatorname{vol}_g$ be its normalized [Riemannian volume form](../../../differential-geometry.md#riemannian-volume-form). The [Euclidean metric](../../../differential-geometry.md#euclidean-metric) induces an [inner product](../../../linear-algebra.md#inner-product) on the [exterior algebra](../../../linear-algebra.md#exterior-algebra) of covectors. The [Hodge star operator](../../../differential-form.md#hodge-star-operator) is the unique map from $p$-forms to $(4-p)$-forms satisfying

$$
\alpha\wedge *\beta=\langle\alpha,\beta\rangle_g\operatorname{vol}_g.
$$

For an oriented orthonormal coframe $e^1,\ldots,e^4$, it sends a basis wedge to the complementary wedge with the sign of the permutation that restores $e^1\wedge\cdots\wedge e^4$. Applying the [Hodge star operator](../../../differential-form.md#hodge-star-operator) twice exchanges blocks of $p$ and $4-p$ covectors, so

$$
*^2=(-1)^{p(4-p)},\qquad\boxed{*^2=1\quad\text{on two-forms}.}
$$

Here the supplied volume is interpreted in the usual metric-normalized sense. If instead one defines the operator with an arbitrary unnormalized $\operatorname{vol}=f\operatorname{vol}_g$, that operator is $f*_g$ and its square on two-forms is $f^2$. The usual self-duality statements use the metric-normalized [Hodge star operator](../../../differential-form.md#hodge-star-operator), with the supplied volume specifying orientation.

The projections $P_\pm=(1\pm*)/2$ give the [Hodge splitting of Euclidean two-forms](../../../differential-form.md#hodge-splitting-of-euclidean-two-forms):

$$
\boxed{\Lambda^2=\Lambda^2_+\oplus\Lambda^2_-,\qquad
\alpha_\pm=\frac12(\alpha\pm*\alpha),\qquad *\alpha_\pm=\pm\alpha_\pm.}
$$

Both spaces have dimension three. With $e^4=dt$, bases are

$$
\Sigma_i^\pm=e^i\wedge dt\ \pm\ \frac12\epsilon_{ijk}e^j\wedge e^k,
\qquad i=1,2,3.
$$

The [Hodge star operator](../../../differential-form.md#hodge-star-operator) is an orthogonal involution on two-forms and therefore is self-adjoint. For a [self-dual two-form](../../../differential-form.md#self-dual-differential-form) $H$ and an [anti-self-dual two-form](../../../differential-form.md#anti-self-dual-differential-form) $G$,

$$
\langle H,G\rangle=\langle *H,G\rangle
=\langle H,*G\rangle=-\langle H,G\rangle=0.
$$

Consequently

$$
\boxed{H\wedge G=\langle H,*G\rangle\operatorname{vol}_g=0.}
$$

This is the [wedge orthogonality of opposite-duality two-forms](../../../differential-form.md#wedge-orthogonality-of-opposite-duality-two-forms).

For the [Yang-Mills action](../../../relativistic-quantum-field.md#yang-mills-action), take an anti-Hermitian [special unitary group](../../../topological-group.md#special-unitary-group) connection and the fundamental matrix [trace](../../../linear-algebra.md#matrix-trace), so the positive invariant pairing on its [Lie algebra](../../../lie-algebra.md) is $\langle X,Y\rangle=-\operatorname{tr}(XY)$. Write its [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength) as $F=F_++F_-$ using the [Hodge splitting of Euclidean two-forms](../../../differential-form.md#hodge-splitting-of-euclidean-two-forms), and define

$$
\|F_\pm\|^2=-\int\operatorname{tr}(F_\pm\wedge *F_\pm),\qquad
S_{\mathrm{YM}}=-\frac1{g_{\mathrm{YM}}^2}\int\operatorname{tr}(F\wedge*F).
$$

Cross terms vanish by the [wedge orthogonality of opposite-duality two-forms](../../../differential-form.md#wedge-orthogonality-of-opposite-duality-two-forms). Thus

$$
S_{\mathrm{YM}}=\frac{\|F_+\|^2+\|F_-\|^2}{g_{\mathrm{YM}}^2},\qquad
\int\operatorname{tr}(F\wedge F)=-\|F_+\|^2+\|F_-\|^2.
$$

With this anti-Hermitian convention the [Second Chern number](../../../geometry-and-topology.md#second-chern-number) is

$$
k=c_2(E)[S^4]=\frac1{8\pi^2}\int\operatorname{tr}(F\wedge F).
$$

For example, this normalization follows by expanding $\det(1+iF/(2\pi))$ and using $\operatorname{tr}F=0$. Interpreting the integral as an integer [Second Chern number](../../../geometry-and-topology.md#second-chern-number) on $\mathbb R^4$ assumes the usual decay and gauge behavior that allow extension over the point at infinity. The following norm inequality itself does not require integrality:

$$
\boxed{S_{\mathrm{YM}}\ge\frac{8\pi^2}{g_{\mathrm{YM}}^2}|k|.}
$$

The [Yang-Mills instanton Bogomolny bound](../../../classical-field-theory-soliton.md#yang-mills-instanton-bogomolny-bound) is saturated precisely when one component vanishes: $F=*F$ or $F=-*F$. In the stated convention the self-dual case has $k\le0$ and the anti-self-dual case has $k\ge0$. Reversing orientation, or defining topological charge with the opposite sign, reverses this assignment while leaving the absolute-value bound unchanged.

For the [self-dual Yang-Mills equations in temporal gauge](../../../classical-field-theory-soliton.md#self-dual-yang-mills-equations-in-temporal-gauge), choose $\operatorname{vol}_g=dx^1\wedge dx^2\wedge dx^3\wedge dt$ and $\epsilon_{123}=1$. The relevant [Hodge star operator](../../../differential-form.md#hodge-star-operator) identities are

$$
*(dt\wedge dx^i)=-\frac12\epsilon_{ijk}dx^j\wedge dx^k,
\qquad *(dx^j\wedge dx^k)=-\epsilon_{ijk}dt\wedge dx^i.
$$

Writing $F=F_{ti}\,dt\wedge dx^i+\tfrac12F_{jk}\,dx^j\wedge dx^k$, the [self-dual Yang-Mills equations](../../../classical-field-theory-soliton.md#self-dual-yang-mills-equations) $F=*F$ give

$$
F_{ti}=-\frac12\epsilon_{ijk}F_{jk}.
$$

In [temporal gauge](../../../relativistic-quantum-field.md#temporal-gauge), $A_t=0$, so the [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength) component is $F_{ti}=\partial_tA_i-\partial_iA_t+[A_t,A_i]=\partial_tA_i$. Hence

$$
\boxed{\partial_tA_i=-\frac12\epsilon_{ijk}F_{jk},\qquad
F_{jk}=\partial_jA_k-\partial_kA_j+[A_j,A_k].}
$$

The minus sign follows from placing $dt$ last in the orientation and first in the mixed curvature component.

## 2

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The real [vector space](../../../vector-space.md) of [symmetric matrices](../../../linear-algebra.md#symmetric-matrix) has dimension $n(n+1)/2$. On its invertible part the derivative of the [determinant](../../../linear-algebra.md#determinant) is

$$
D(\det)_B(C)=\det(B)\operatorname{tr}(B^{-1}C).
$$

At a determinant-one symmetric matrix, this derivative is nonzero: the symmetric direction $C=B$ gives value $n$. The [regular level set theorem](../../../differential-geometry.md#regular-level-set-theorem) therefore yields

$$
\boxed{\dim M=\frac{n(n+1)}2-1,\qquad
T_BM=\{C=C^T:\operatorname{tr}(B^{-1}C)=0\}.}
$$

This applies to every signature component, not only positive-definite matrices.

The [special linear congruence action on symmetric matrices](../../../lie-theory.md#special-linear-congruence-action-on-symmetric-matrices) preserves symmetry because $(ABA^T)^T=ABA^T$, and preserves determinant because $\det(ABA^T)=(\det A)^2\det B=1$. The identity acts trivially and

$$
A_1\cdot(A_2\cdot B)=A_1A_2B(A_1A_2)^T=(A_1A_2)\cdot B.
$$

These verify a smooth left [Lie group action](../../../lie-theory.md#lie-group-action) of the [special linear group](../../../group-theory.md#special-linear-group). By [Sylvester's law of inertia](../../../linear-algebra.md#sylvester-s-law-of-inertia), it also preserves the numbers of positive and negative eigenvalues.

For $n=2$, parametrize the [symmetric matrices](../../../linear-algebra.md#symmetric-matrix) by

$$
B=\begin{pmatrix}t+x&y\\y&t-x\end{pmatrix},\qquad
\det B=t^2-x^2-y^2.
$$

Thus $M$ is exactly the [two-sheeted hyperboloid](../../../differential-geometry.md#two-sheeted-hyperboloid)

$$
\boxed{t^2-x^2-y^2=1,\qquad t>0\text{ or }t<0.}
$$

The two sheets consist respectively of positive-definite and negative-definite matrices. Each is preserved by the [special linear congruence action on symmetric matrices](../../../lie-theory.md#special-linear-congruence-action-on-symmetric-matrices). They are individually transitive: on the positive sheet $B=AA^T$ with $A=B^{1/2}$ and $\det A=1$; on the negative sheet use $B=-AA^T$. The stabilizer of either $I$ or $-I$ is $SO(2)$.

Differentiating the left [Lie group action](../../../lie-theory.md#lie-group-action) along $\exp(sX)$ gives the [fundamental vector field](../../../lie-theory.md#fundamental-vector-field)

$$
u_X(B)=XB+BX^T.
$$

For the three matrices in the question, their coordinate components are

$$
\begin{aligned}
u_1&=y\partial_t+y\partial_x+(t-x)\partial_y,\\
u_2&=2x\partial_t+2t\partial_x,\\
u_3&=y\partial_t-y\partial_x+(t+x)\partial_y.
\end{aligned}
$$

A sign convention matters here. With the usual [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) $[U,V]f=U(Vf)-V(Uf)$, the fundamental fields of this left action obey $[u_X,u_Y]=-u_{[X,Y]}$. Indeed, for linear coordinate fields $u_X(z)=R_Xz$, the bracket has coefficient $(R_YR_X-R_XR_Y)z$. To obtain a [Lie algebra representation](../../../lie-algebra.md#lie-algebra-representation) rather than an anti-representation, use the [infinitesimal left-action sign convention](../../../lie-theory.md#infinitesimal-left-action-sign-convention)

$$
v_X(B)=\left.\frac{d}{ds}\right|_{s=0}e^{-sX}Be^{-sX^T}=-u_X(B).
$$

An explicit answer is therefore

$$
\boxed{\begin{aligned}
v_1&=-y\partial_t-y\partial_x+(x-t)\partial_y,\\
v_2&=-2x\partial_t-2t\partial_x,\\
v_3&=-y\partial_t+y\partial_x-(t+x)\partial_y.
\end{aligned}}
$$

These are tangent to the [two-sheeted hyperboloid](../../../differential-geometry.md#two-sheeted-hyperboloid): applying each to $Q=t^2-x^2-y^2$ gives zero. For example,

$$
v_1(Q)=-2ty+2xy-2y(x-t)=0.
$$

They can be written on either sheet using $t=\pm\sqrt{1+x^2+y^2}$:

$$
v_1=-y\partial_x+(x-t)\partial_y,\qquad
v_2=-2t\partial_x,\qquad
v_3=y\partial_x-(t+x)\partial_y.
$$

Here the omitted $\partial_t$ component is determined by tangency, and derivatives of $t(x,y)$ must be included when computing brackets in these coordinates.

Direct matrix multiplication gives

$$
[\tau_2,\tau_1]=2\tau_1,\qquad
[\tau_2,\tau_3]=-2\tau_3,\qquad
[\tau_1,\tau_3]=\tau_2.
$$

Direct differentiation of the displayed [vector fields](../../../calculus.md#vector-field) gives exactly

$$
\boxed{[v_2,v_1]=2v_1,\qquad [v_2,v_3]=-2v_3,\qquad [v_1,v_3]=v_2.}
$$

For instance, in ambient $(t,x,y)$ coordinates, $[v_1,v_3]=(-2x,-2t,0)=v_2$. These are the defining relations of the [sl2 Lie algebra](../../../semisimple-lie-algebra.md#sl2-lie-algebra). The three fields are linearly independent over constant real coefficients: if $a v_1+b v_2+c v_3$ vanishes on a sheet, its $\partial_x$ coefficient $(-a+c)y-2bt$ forces $b=0,c=a$, and its $\partial_y$ coefficient then equals $-2at$, forcing $a=c=0$. Thus the representation is **faithful**. Their pointwise span need only have dimension two, consistent with the dimension of each sheet.

## 3

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [principal bundle](../../../fiber-bundle.md#principal-bundle) separates the geometry of internal symmetry from a chosen local [gauge potential](../../../relativistic-quantum-field.md#gauge-field). Let $\pi:P\to X$ be a principal $G$-bundle with a free right [Lie group action](../../../lie-theory.md#lie-group-action). Each fiber is a copy of $G$, but generally no single identification works globally. A [principal connection](../../../fiber-bundle.md#connection-principal-bundle) tells us how to compare fibers over nearby base points. Its physical interpretation is a prescription for [parallel transport](../../../fiber-bundle.md#parallel-transport) of internal states.

For $\xi\in\mathfrak g$, the vertical [fundamental vector field](../../../lie-theory.md#fundamental-vector-field) is $\xi^\#_p=\left.\frac d{ds}\right|_0p\exp(s\xi)$. A [principal connection](../../../fiber-bundle.md#connection-principal-bundle) is a [Lie algebra](../../../lie-algebra.md)-valued one-form $\mathcal A$ on $P$ satisfying

$$
\boxed{\mathcal A(\xi^\#)=\xi,\qquad R_g^*\mathcal A=\operatorname{Ad}_{g^{-1}}\mathcal A.}
$$

Equivalently, the [horizontal distribution of a principal connection](../../../fiber-bundle.md#horizontal-distribution-of-a-principal-connection) $H_p=\ker\mathcal A_p$ complements the vertical tangent space and is preserved by right translation. Given a curve in $X$ and an initial point in its fiber, there is a unique horizontal lift. For a closed curve its endpoint differs from its start by a group element: the [holonomy of a connection](../../../fiber-bundle.md#holonomy). Thus a [principal connection](../../../fiber-bundle.md#connection-principal-bundle) contains both infinitesimal and global transport information.

Choose local sections $s_\alpha:U_\alpha\to P$. Their [local principal connection forms](../../../fiber-bundle.md#local-principal-connection-form) $A_\alpha=s_\alpha^*\mathcal A$ are the usual [gauge potentials](../../../relativistic-quantum-field.md#gauge-field). If $s_\beta=s_\alpha g_{\alpha\beta}$ on an overlap, equivariance and reproduction of vertical generators give

$$
\boxed{A_\beta=g_{\alpha\beta}^{-1}A_\alpha g_{\alpha\beta}
+g_{\alpha\beta}^{-1}dg_{\alpha\beta}.}
$$

This inhomogeneous law means that a [gauge potential](../../../relativistic-quantum-field.md#gauge-field) is not an ordinary globally defined tensor. Its local formulas glue to a global [principal connection](../../../fiber-bundle.md#connection-principal-bundle). The same law describes changing a local section by a gauge function. For example, to impose [temporal gauge](../../../relativistic-quantum-field.md#temporal-gauge) locally, solve $\partial_tg=-A_tg$ so the transformed time component vanishes.

The [curvature of a principal connection](../../../fiber-bundle.md#curvature-of-a-principal-connection) is

$$
\boxed{\mathcal F=d\mathcal A+\frac12[\mathcal A\wedge\mathcal A],\qquad
F_\alpha=dA_\alpha+A_\alpha\wedge A_\alpha.}
$$

Unlike the [principal connection](../../../fiber-bundle.md#connection-principal-bundle) form, its curvature is horizontal and equivariant. Consequently $F_\beta=g_{\alpha\beta}^{-1}F_\alpha g_{\alpha\beta}$, and the [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength) is globally a two-form on $X$ with values in the [adjoint bundle](../../../fiber-bundle.md#adjoint-bundle) $\operatorname{ad}P=P\times_{\operatorname{Ad}}\mathfrak g$. The curvature measures the failure of horizontal directions to close under brackets: for horizontal lifts $U,V$, $\mathcal F(U,V)=-\mathcal A([U,V])$. A [flat principal connection](../../../fiber-bundle.md#flat-principal-connection) has an integrable horizontal distribution, although nontrivial global [holonomy of a connection](../../../fiber-bundle.md#holonomy) can remain around noncontractible curves.

The [covariant exterior derivative](../../../fiber-bundle.md#exterior-covariant-derivative) on [adjoint bundle](../../../fiber-bundle.md#adjoint-bundle)-valued forms is locally $D_A=d+[A,\,\cdot\,]$. Expanding $F=dA+A\wedge A$ and using $d^2=0$ yields the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity)

$$
\boxed{D_AF=0.}
$$

For a representation $\rho$ of $G$, the same [principal connection](../../../fiber-bundle.md#connection-principal-bundle) induces transport in the corresponding [associated vector bundle](../../../fiber-bundle.md#associated-vector-bundle); locally its [covariant derivative](../../../general-relativity.md#covariant-derivative) is $d+\rho_*(A)$. This explains why charged matter and the [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength) use the same [gauge potential](../../../relativistic-quantum-field.md#gauge-field).

Now put an oriented [Riemannian metric](../../../differential-geometry.md#riemannian-metric) on a four-dimensional base and take $G=SU(n)$. Use anti-Hermitian matrices with positive pairing $-\operatorname{tr}(XY)$, as in the preceding solution. The [Yang-Mills action](../../../relativistic-quantum-field.md#yang-mills-action) is

$$
S[A]=-\frac1{g_{\mathrm{YM}}^2}\int_X\operatorname{tr}(F\wedge*F).
$$

Its gauge invariance follows from curvature conjugation and invariance of the [trace](../../../linear-algebra.md#matrix-trace). Under a compactly supported variation $a=\delta A$, $\delta F=D_Aa$. Integration by parts therefore gives

$$
\delta S=-\frac2{g_{\mathrm{YM}}^2}\int_X\operatorname{tr}(a\wedge D_A*F),\qquad
\boxed{D_A*F=0.}
$$

This is a second-order equation for the [gauge potential](../../../relativistic-quantum-field.md#gauge-field). The [self-dual Yang-Mills equations](../../../classical-field-theory-soliton.md#self-dual-yang-mills-equations) $F=*F$ and the [Anti-self-dual Yang-Mills equations](../../../classical-field-theory-soliton.md#anti-self-dual-yang-mills-equations) $F=-*F$ are first-order equations. Either implies the full [Yang-Mills equations](../../../relativistic-quantum-field.md#yang-mills-equations) immediately, since $D_A*F=\pm D_AF=0$ by the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity). This is [self-duality implies Yang-Mills equations](../../../classical-field-theory-soliton.md#self-duality-implies-yang-mills-equations).

A [Yang-Mills instanton](../../../classical-field-theory-soliton.md#yang-mills-instanton) is a smooth finite-action Euclidean solution with self-dual or anti-self-dual [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength). Its defining first-order condition depends on the [principal connection](../../../fiber-bundle.md#connection-principal-bundle), the metric and the orientation. Since the [Hodge star operator](../../../differential-form.md#hodge-star-operator) on two-forms is unchanged under $g\mapsto e^{2f}g$ in four dimensions, self-duality and the [Yang-Mills action](../../../relativistic-quantum-field.md#yang-mills-action) are conformally invariant. In particular Euclidean solutions can be studied through conformal compactification, with appropriate behavior at infinity.

The global topology is encoded by [Chern-Weil theory](../../../geometry-and-topology.md#chern-weil-homomorphism). Since $\operatorname{tr}F=0$, the [Second Chern form](../../../geometry-and-topology.md#second-chern-form) and [Second Chern number](../../../geometry-and-topology.md#second-chern-number) are

$$
c_2(A)=\frac1{8\pi^2}\operatorname{tr}(F\wedge F),\qquad
k=\int_Xc_2(A)\in\mathbb Z
$$

on a compact oriented four-manifold. The [Bianchi identity](../../../fiber-bundle.md#bianchi-identity) makes $c_2(A)$ closed. More explicitly, under a connection variation,

$$
\delta\operatorname{tr}(F\wedge F)
=2\operatorname{tr}(D_Aa\wedge F)
=2d\operatorname{tr}(a\wedge F).
$$

Thus the integrated [Second Chern number](../../../geometry-and-topology.md#second-chern-number) is independent of the [principal connection](../../../fiber-bundle.md#connection-principal-bundle) on a fixed bundle, with the usual fixed-boundary condition on a noncompact base. The space of connections is affine, so integrating this variation along a straight path also proves that their characteristic forms differ by an exact form.

Locally the same characteristic form has a [Chern-Simons 3-form](../../../geometry-and-topology.md#chern-simons-3-form) primitive:

$$
\operatorname{tr}(F\wedge F)=d\operatorname{tr}\left(A\wedge dA+\frac23A\wedge A\wedge A\right).
$$

On $\mathbb R^4$ the underlying bundle is trivial, but a finite-action instanton with the standard extendible behavior at infinity can define a nontrivial bundle after adding the point at infinity. The transition map on an equatorial $S^3$ takes values in $SU(n)$; for $n\ge2$, its homotopy class lies in $\pi_3(SU(n))\cong\mathbb Z$. The boundary integral of the [Chern-Simons 3-form](../../../geometry-and-topology.md#chern-simons-3-form) computes that integer with the chosen sign convention. This reconciles a local matrix-valued [gauge potential](../../../relativistic-quantum-field.md#gauge-field) on $\mathbb R^4$ with nonzero global [Second Chern number](../../../geometry-and-topology.md#second-chern-number) on $S^4$.

Finally the [Hodge splitting of Euclidean two-forms](../../../differential-form.md#hodge-splitting-of-euclidean-two-forms) produces the [Yang-Mills instanton Bogomolny bound](../../../classical-field-theory-soliton.md#yang-mills-instanton-bogomolny-bound)

$$
\boxed{S[A]\ge\frac{8\pi^2}{g_{\mathrm{YM}}^2}|k|.}
$$

Equality holds exactly when the opposite-duality component of the [gauge curvature](../../../relativistic-quantum-field.md#gauge-field-strength) vanishes. Thus a [Yang-Mills instanton](../../../classical-field-theory-soliton.md#yang-mills-instanton) is an **absolute action minimum in its fixed topological sector**, not merely a stationary solution. In this trace convention self-dual instantons have $k<0$ and anti-self-dual instantons have $k>0$. In the zero sector, a self-dual or anti-self-dual finite-action solution has $S=0$ and hence $F=0$.

Different [principal connections](../../../fiber-bundle.md#connection-principal-bundle) related by bundle gauge transformations describe the same physical configuration. Fixing $k$ and taking the quotient of instanton solutions by this [gauge equivalence of principal connections](../../../fiber-bundle.md#gauge-equivalence-of-principal-connections) gives the [instanton moduli space](../../../classical-field-theory-soliton.md#instanton-moduli-space). Near an anti-self-dual solution, write a variation as $a\in\Omega^1(X,\operatorname{ad}P)$. The linearized instanton equation and infinitesimal gauge transformations are

$$
P_+D_Aa=0,\qquad a\sim a+D_A\varepsilon.
$$

A local gauge condition $D_A^*a=0$ removes this redundancy. The combined operator $D_A^*\oplus P_+D_A$ is elliptic: for nonzero covector $\xi$, its principal symbol $a\mapsto(\iota_{\xi^\sharp}a,P_+(\xi\wedge a))$ has zero kernel. Choose $\xi=dt$; the first component removes $a_t$, and the self-dual projection of $dt\wedge a$ removes the three remaining components. This connects the [instanton moduli space](../../../classical-field-theory-soliton.md#instanton-moduli-space) to geometric analysis, while the characteristic number and transport law explain its topological and physical meaning.

## 4

↑ **Parent:** [Paper 313](paper-313.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [Poisson bivector](../../../symplectic-geometry.md#poisson-bivector) is a smooth antisymmetric contravariant two-tensor

$$
\omega=\frac12\omega^{ij}(x)\partial_i\wedge\partial_j
$$

whose bracket on smooth functions,

$$
\boxed{\{F,G\}=\omega(dF,dG)=\omega^{ij}\partial_iF\partial_jG,}
$$

satisfies the [Jacobi identity](../../../lie-algebra.md#jacobi-identity). Bilinearity and antisymmetry are immediate, and the product rule makes the bracket a derivation in each argument. Together these properties define a [Poisson manifold](../../../symplectic-geometry.md#poisson-manifold). Unlike a [symplectic form](../../../symplectic-geometry.md#symplectic-form), the [Poisson bivector](../../../symplectic-geometry.md#poisson-bivector) need not be nondegenerate.

Apply the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) to the coordinate functions. Since $\{x^i,x^j\}=\omega^{ij}$,

$$
0=\{x^i,\{x^j,x^k\}\}+\{x^j,\{x^k,x^i\}\}+\{x^k,\{x^i,x^j\}\}
=\sum_m\left(\omega^{im}\partial_m\omega^{jk}
+\omega^{jm}\partial_m\omega^{ki}
+\omega^{km}\partial_m\omega^{ij}\right).
$$

Changing $\omega^{im}$ to $-\omega^{mi}$ and rearranging the three summands gives the printed [coordinate Jacobi condition for a Poisson bivector](../../../symplectic-geometry.md#coordinate-jacobi-condition-for-a-poisson-bivector):

$$
\boxed{\sum_m\left(\omega^{mi}\partial_m\omega^{jk}
+\omega^{mk}\partial_m\omega^{ij}
+\omega^{mj}\partial_m\omega^{ki}\right)=0.}
$$

This is also sufficient: expanding the Jacobiator of three arbitrary smooth functions, all terms involving second derivatives cancel in pairs by antisymmetry. The remaining coefficient of $\partial_iF\partial_jG\partial_kH$ is the coordinate-function Jacobiator displayed above.

For a [Lie algebra](../../../lie-algebra.md), the natural global space carrying the proposed linear bracket is its [dual space](../../../linear-algebra.md#dual-space) $\mathfrak g^*$. If $v^i$ is the chosen basis, define its linear coordinate function by $x^i(\ell)=\ell(v^i)$. The [Lie-Poisson bracket](../../../symplectic-geometry.md#lie-poisson-bracket) is

$$
\boxed{\{F,G\}(\ell)=\ell([dF_\ell,dG_\ell])
=c^{ij}_kx^k\partial_iF\partial_jG,}
$$

where $dF_\ell,dG_\ell$ are elements of $\mathfrak g=(\mathfrak g^*)^*$. On a general manifold the same coordinate expression gives a local construction; a global one requires compatible transition rules. The use of $\mathfrak g^*$ supplies that compatibility intrinsically.

Here $\omega^{ij}=c^{ij}_rx^r$ and $\partial_m\omega^{jk}=c^{jk}_m$. The left side of the [coordinate Jacobi condition for a Poisson bivector](../../../symplectic-geometry.md#coordinate-jacobi-condition-for-a-poisson-bivector) is therefore

$$
x^r\sum_m\left(c^{mi}_rc^{jk}_m+c^{mk}_rc^{ij}_m+c^{mj}_rc^{ki}_m\right)
=-x^r\sum_m\left(c^{jk}_mc^{im}_r+c^{ij}_mc^{km}_r+c^{ki}_mc^{jm}_r\right)=0.
$$

The final coefficient is the negative of the coefficient of $v^r$ in the [Lie algebra](../../../lie-algebra.md) identity $[v^i,[v^j,v^k]]+[v^j,[v^k,v^i]]+[v^k,[v^i,v^j]]=0$. Thus the [Lie-Poisson bracket](../../../symplectic-geometry.md#lie-poisson-bracket) satisfies the [Jacobi identity](../../../lie-algebra.md#jacobi-identity).

It remains to find the [Lie algebra structure constants](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) for the printed rotation fields. Distinguish their original spatial coordinates $(x,y,z)$ from the coordinates $(x^1,x^2,x^3)$ on the [dual space](../../../linear-algebra.md#dual-space). Use the conventional [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields). Their component vectors are $(0,-z,y)$, $(z,0,-x)$ and $(-y,x,0)$, respectively. For example,

$$
[v^1,v^2]=(y,-x,0)=-v^3.
$$

Similarly,

$$
\boxed{[v^2,v^3]=-v^1,\qquad [v^3,v^1]=-v^2,\qquad
c^{ij}_k=-\epsilon_{ijk}.}
$$

The negative sign is essential: these are the fundamental fields of a left rotation action with the stated [Lie bracket of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields), and consequently have the [infinitesimal left-action sign convention](../../../lie-theory.md#infinitesimal-left-action-sign-convention) discussed above. The first field here has component $y\partial_z$, as printed in the PDF.

The [Lie-Poisson bracket](../../../symplectic-geometry.md#lie-poisson-bracket) on the [dual space](../../../linear-algebra.md#dual-space) consequently has

$$
\{x^1,x^2\}=-x^3,\qquad
\{x^2,x^3\}=-x^1,\qquad
\{x^3,x^1\}=-x^2.
$$

For the evolution convention $\dot F=\{F,H\}$, the [Hamiltonian function](../../../symplectic-geometry.md#hamiltonian-function) has derivatives $(2Ax^1,2Bx^2,2Cx^3)$. Substitution gives the [quadratic rotational Lie-Poisson dynamics](../../../classical-mechanics.md#quadratic-rotational-lie-poisson-dynamics)

$$
\boxed{\begin{aligned}
\dot x^1&=2(C-B)x^2x^3,\\
\dot x^2&=2(A-C)x^3x^1,\\
\dot x^3&=2(B-A)x^1x^2.
\end{aligned}}
$$

These are Euler-type [Hamilton's equations](../../../classical-mechanics.md#hamilton-s-equations) on a noncanonical [Poisson manifold](../../../symplectic-geometry.md#poisson-manifold). When $A=1/(2I_1)$, $B=1/(2I_2)$ and $C=1/(2I_3)$ with positive principal inertias, they are the [Euler equations for a torque-free rigid body](../../../classical-mechanics.md#euler-equations-for-a-torque-free-rigid-body) in body angular-momentum coordinates. As a check, $H$ is conserved by antisymmetry of the [Poisson bracket](../../../classical-mechanics.md#poisson-bracket), and $C_0=(x^1)^2+(x^2)^2+(x^3)^2$ is a [Casimir function of a Poisson manifold](../../../symplectic-geometry.md#casimir-function-of-a-poisson-manifold). Direct differentiation of $C_0$ in the three equations cancels the terms $4[(C-B)+(A-C)+(B-A)]x^1x^2x^3$. The [Hamiltonian flow](../../../classical-mechanics.md#hamiltonian-flow) therefore lies on both an energy level and a sphere, a [symplectic leaf](../../../symplectic-geometry.md#symplectic-leaf) of this signed rotational bracket.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
