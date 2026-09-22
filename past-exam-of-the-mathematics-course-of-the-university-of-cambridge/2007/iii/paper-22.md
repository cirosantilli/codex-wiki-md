# Paper 22

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper22.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper22.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

An [almost complex structure](../../../complex-geometry.md#almost-complex-manifold) is a smooth real [vector bundle endomorphism](../../../fiber-bundle.md#vector-bundle-endomorphism) $J:TM\to TM$ satisfying $J^2=-I$. In particular, $M$ has even real dimension $2n$. Extend $J$ complex-linearly to $T_{\mathbb C}M=TM\otimes_{\mathbb R}\mathbb C$. Its minimal polynomial divides $(u-i)(u+i)$, whose roots are distinct, so the [type decomposition of the complexified tangent bundle](../../../complex-geometry.md#type-decomposition-of-the-complexified-tangent-bundle) is

$$
T_{\mathbb C}M=T^{1,0}M\oplus T^{0,1}M,\qquad
T^{1,0}M=\ker(J-iI),\quad T^{0,1}M=\ker(J+iI).
$$

The smooth projections are $(I-iJ)/2$ and $(I+iJ)/2$. [Complex conjugation](../../../complex-analysis.md#complex-conjugation) exchanges the two rank-$n$ [eigenbundles](../../../fiber-bundle.md#eigenbundle). A $(1,0)$-covector annihilates $T^{0,1}M$ and a $(0,1)$-covector annihilates $T^{1,0}M$. Thus the [differential forms of type (p, q)](../../../complex-geometry.md#differential-form-of-type-p-q) are the smooth sections of

$$
\Lambda^{p,q}T^*M=\Lambda^p(T^{1,0}M)^*\otimes\Lambda^q(T^{0,1}M)^*,
\qquad
\Lambda^rT^*_{\mathbb C}M=\bigoplus_{p+q=r}\Lambda^{p,q}T^*M.
$$

Here the tensor product is identified with its image under the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms). For a real tangent vector $v$, the vectors $v-iJv$ and $v+iJv$ exhibit the two types directly.

We now construct the [almost complex structure from a decomposable volume form](../../../complex-geometry.md#almost-complex-structure-from-a-decomposable-volume-form). Locally write $\Omega=\theta_1\wedge\cdots\wedge\theta_n$. The nonvanishing of $\Omega\wedge\overline\Omega$ says that the $2n$ covectors $\theta_1,\ldots,\theta_n,\overline\theta_1,\ldots,\overline\theta_n$ form a complex coframe. In particular, the span of the $\theta_j$ has the intrinsic description

$$
W_x=\{\alpha\in T_x^*M\otimes\mathbb C:\alpha\wedge\Omega_x=0\}.
$$

Indeed, expansion in that coframe shows that every coefficient of a conjugate factor must vanish if $\alpha\wedge\Omega_x=0$. Therefore this span is independent of the chosen local factorization. The local coframes show that $W$ is a smooth rank-$n$ [vector subbundle](../../../fiber-bundle.md#vector-subbundle), and

$$
T^*M\otimes\mathbb C=W\oplus\overline W.
$$

Define $J_\Omega^*$ to be multiplication by $i$ on $W$ and by $-i$ on $\overline W$. It commutes with [complex conjugation](../../../complex-analysis.md#complex-conjugation), so is the complexification of a real smooth [bundle endomorphism](../../../fiber-bundle.md#vector-bundle-endomorphism), whose dual defines $J_\Omega$ on $TM$. It has square $-I$, and its $(1,0)$-covectors are exactly $W$. Conversely, any such [almost complex structure](../../../complex-geometry.md#almost-complex-manifold) must have this same action on the entire coframe. Thus **$J_\Omega$ exists globally and is unique**, and every factor in every allowed decomposition is a $(1,0)$-form.

Finally suppose $d\Omega=0$. Since $\theta_j\wedge\Omega=0$, the [exterior derivative](../../../differential-form.md#exterior-derivative) product rule gives

$$
0=d(\theta_j\wedge\Omega)=d\theta_j\wedge\Omega-\theta_j\wedge d\Omega
=d\theta_j\wedge\Omega.
$$

Decompose $d\theta_j$ into types $(2,0)$, $(1,1)$ and $(0,2)$ using $J_\Omega$. The first two wedge products with the $(n,0)$-form $\Omega$ vanish by dimension. On $(0,2)$-forms, wedging with $\Omega$ is injective: the monomials $\Omega\wedge\overline\theta_a\wedge\overline\theta_b$ are linearly independent. For $n=1$ the $(0,2)$ space is zero, so the statement still holds. Hence every $d\theta_j$ has no $(0,2)$ component. For an arbitrary $(1,0)$-form $\alpha=\sum_j a_j\theta_j$, the extra terms $da_j\wedge\theta_j$ likewise have only types $(2,0)$ and $(1,1)$. The [bracket and differential-form criteria for integrability](../../../complex-geometry.md#bracket-and-differential-form-criteria-for-integrability) proved below now give

$$
\boxed{d\Omega=0\ \Longrightarrow\ J_\Omega\text{ is integrable}.}
$$

Local decomposability has been used essentially; the nonvanishing top-degree product alone does not provide the required coframe.

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

These are local criteria: multiplying by a smooth bump function extends any local test field or form to a global one without changing it near a chosen point. Assume the [Lie bracket](../../../lie-algebra.md#lie-bracket) of any two sections of $T^{1,0}M$ again lies in $T^{1,0}M$. Because the [almost complex structure](../../../complex-geometry.md#almost-complex-manifold) is real, conjugating this condition shows that the [Lie bracket](../../../lie-algebra.md#lie-bracket) of any two sections $U,V$ of $T^{0,1}M$ lies in $T^{0,1}M$.

For a $(1,0)$-form $\alpha$, the [exterior derivative](../../../differential-form.md#exterior-derivative) formula is

$$
d\alpha(U,V)=U(\alpha(V))-V(\alpha(U))-\alpha([U,V]).
$$

The first two terms vanish because $\alpha$ annihilates $T^{0,1}M$, and the last vanishes by bracket closure. The $(0,2)$ component is exactly the restriction of $d\alpha$ to two arguments in $T^{0,1}M$. Thus it is zero. Since the only types of a two-form are $(2,0)$, $(1,1)$ and $(0,2)$, **the bracket condition implies the stated differential-form condition**. This argument uses neither holomorphic coordinates nor an integrability theorem as an unproved intermediate step.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Conversely, suppose the [exterior derivative](../../../differential-form.md#exterior-derivative) of every $(1,0)$-form has no $(0,2)$ part. For sections $U,V$ of $T^{0,1}M$, the same [exterior derivative](../../../differential-form.md#exterior-derivative) formula gives

$$
0=d\alpha(U,V)=-\alpha([U,V])\qquad\text{for every }(1,0)\text{-form }\alpha.
$$

The common annihilator of all $(1,0)$-covectors is $T^{0,1}M$. Local $(1,0)$-coframes therefore show that $[U,V]$ belongs to $T^{0,1}M$. Conjugating gives bracket closure of $T^{1,0}M$. Thus **the two criteria are equivalent**. These are the [bracket and differential-form criteria for integrability](../../../complex-geometry.md#bracket-and-differential-form-criteria-for-integrability), and establish integrability in the sense used here.

## 2

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

On a [complex manifold](../../../complex-geometry.md#complex-manifold), [holomorphic coordinates](../../../complex-geometry.md#holomorphic-coordinate) give the decomposition $d=\partial+\bar\partial$, with

$$
\partial:\mathcal A^{p,q}\to\mathcal A^{p+1,q},\qquad
\bar\partial:\mathcal A^{p,q}\to\mathcal A^{p,q+1}.
$$

For $\alpha=\sum_{I,J}a_{I\bar J}\,dz^I\wedge d\bar z^J$, the [conjugate Dolbeault operator](../../../complex-geometry.md#conjugate-dolbeault-operator) $\partial$ and the [Dolbeault operator](../../../complex-geometry.md#dolbeault-operator) $\bar\partial$ are explicitly

$$
\partial\alpha=\sum_{I,J,k}\frac{\partial a_{I\bar J}}{\partial z^k}\,dz^k\wedge dz^I\wedge d\bar z^J,
\qquad
\bar\partial\alpha=\sum_{I,J,k}\frac{\partial a_{I\bar J}}{\partial\bar z^k}\,d\bar z^k\wedge dz^I\wedge d\bar z^J.
$$

These are the type components of the intrinsic [exterior derivative](../../../differential-form.md#exterior-derivative), so are independent of coordinates. The identity $d^2=0$, separated by type, gives $\partial^2=\bar\partial^2=0$ and $\partial\bar\partial+\bar\partial\partial=0$. A [holomorphic p-form on a complex manifold](../../../complex-geometry.md#holomorphic-p-form-on-a-complex-manifold) is a $(p,0)$-form whose coefficients are [holomorphic functions](../../../complex-analysis.md#holomorphic-function); equivalently it is a $(p,0)$-form killed by the [Dolbeault operator](../../../complex-geometry.md#dolbeault-operator).

A rank-$r$ [holomorphic vector bundle](../../../complex-geometry.md#holomorphic-vector-bundle) has local trivializations $E|_{U_i}\cong U_i\times\mathbb C^r$ whose changes are $(x,v)\mapsto(x,g_{ij}(x)v)$, with $g_{ij}:U_i\cap U_j\to\operatorname{GL}_r(\mathbb C)$ holomorphic. These [transition functions of a vector bundle](../../../fiber-bundle.md#transition-function-of-a-vector-bundle) satisfy $g_{ii}=I$ and $g_{ij}g_{jk}=g_{ik}$. Equivalently, for local frames we use the convention $e_j=e_i g_{ij}$. A [holomorphic section](../../../complex-geometry.md#holomorphic-section) is a section having holomorphic coordinate functions in every such [holomorphic local frame](../../../complex-geometry.md#holomorphic-local-trivialization); the condition is unchanged by the holomorphic invertible transitions.

The [holomorphic cotangent bundle](../../../complex-geometry.md#holomorphic-cotangent-bundle) has local frames $dz^1,\ldots,dz^n$. Under another [holomorphic coordinate](../../../complex-geometry.md#holomorphic-coordinate) system $w$, the [chain rule](../../../calculus.md#chain-rule) gives

$$
dw^a=\sum_b\frac{\partial w^a}{\partial z^b}\,dz^b.
$$

The Jacobian matrix is holomorphic and invertible, with holomorphic inverse supplied by the inverse coordinate change. These are precisely holomorphic bundle transitions. A section written as $\sum_b f_b(z)\,dz^b$ is holomorphic exactly when every $f_b$ is holomorphic, so

$$
\boxed{H^0(X,\Omega_X^1)=\{\alpha\in\mathcal A^{1,0}(X):\bar\partial\alpha=0\},}
$$

the space of [holomorphic one-forms](../../../complex-geometry.md#holomorphic-one-form). In particular, being a holomorphic section is not the same as being a $d$-closed one-form on an arbitrary [complex manifold](../../../complex-geometry.md#complex-manifold).

The [complex tautological line bundle](../../../fiber-bundle.md#complex-tautological-line-bundle) is

$$
\mathcal O(-1)=\{([Z],v)\in\mathbb{CP}^n\times\mathbb C^{n+1}:v\in\mathbb C Z\}.
$$

On $U_i=\{Z_i\ne0\}$ use the nowhere-zero frame $s_i([Z])=Z/Z_i$. Its components are holomorphic affine coordinates and the constant one in position $i$. On overlaps

$$
s_j=\frac{Z_i}{Z_j}s_i,
$$

so the frame changes are nowhere-zero [holomorphic functions](../../../complex-analysis.md#holomorphic-function). This proves that $\mathcal O(-1)$ is a [holomorphic line bundle](../../../complex-geometry.md#holomorphic-line-bundle), and its inclusion into the trivial bundle is a [holomorphic bundle map](../../../fiber-bundle.md#holomorphic-bundle-map).

A global [holomorphic section](../../../complex-geometry.md#holomorphic-section) composed with that inclusion has $n+1$ component [holomorphic functions](../../../complex-analysis.md#holomorphic-function) on compact connected [Complex projective space](../../../algebraic-topology.md#complex-projective-space). Each is constant: its absolute value attains a maximum; in a coordinate ball the one-variable maximum modulus principle along complex lines makes it locally constant, and connectedness propagates that constant globally. Thus the section is a fixed vector $v\in\mathbb C^{n+1}$ lying in every fibre, namely every line $\mathbb C Z$. For $n\geq1$ the intersection of all these lines is zero. Hence

$$
\boxed{H^0(\mathbb{CP}^n,\mathcal O(-1))=0\quad(n\geq1).}
$$

The positive-dimension convention is necessary: $\mathbb{CP}^0$ is one point and this section space is $\mathbb C$.

## 3

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

An [irreducible analytic subvariety of a complex manifold](../../../complex-geometry.md#irreducible-analytic-subvariety-of-a-complex-manifold) is a closed subset locally defined by finitely many [holomorphic functions](../../../complex-analysis.md#holomorphic-function) which cannot be expressed as the union of two proper closed analytic subsets. In a complex $n$-manifold, codimension $k$ means pure complex dimension $n-k$. A [divisor on a complex manifold](../../../complex-geometry.md#divisor-on-a-complex-manifold) is a locally finite formal integer combination

$$
D=\sum_\nu m_\nu Y_\nu
$$

of irreducible analytic hypersurfaces. Compactness makes the set of components in this sum finite. Negative coefficients are permitted; a local equation for such a [divisor on a complex manifold](../../../complex-geometry.md#divisor-on-a-complex-manifold) is generally meromorphic rather than holomorphic.

We use these precise local facts. In [holomorphic coordinates](../../../complex-geometry.md#holomorphic-coordinate) at $x$, the local ring is $\mathcal O_{X,x}\cong\mathbb C\{z_1,\ldots,z_n\}$, a Noetherian [regular local ring](../../../commutative-algebra.md#regular-local-ring) and a [unique factorization domain](../../../algebra.md#unique-factorization-domain). Each analytic hypersurface germ has finitely many irreducible local branches; their prime ideals have height one and are generated by irreducible holomorphic germs. A holomorphic germ is a unit exactly when its value at $x$ is nonzero. Consequently a nonzero meromorphic germ with order zero on every local hypersurface branch is a holomorphic unit, by cancelling its irreducible factors in numerator and denominator. These are the auxiliary local-ring properties required below.

After shrinking a neighbourhood $U_i$ around each point, choose local branch equations $h_{i\nu a}$, and put

$$
f_i=\prod_{\nu,a}h_{i\nu a}^{m_\nu}.
$$

Its zero and pole orders give exactly the local [divisor on a complex manifold](../../../complex-geometry.md#divisor-on-a-complex-manifold) $D|_{U_i}$. A globally irreducible hypersurface may have several branches locally; all of them must be included with the indicated multiplicity. On an overlap, $f_i/f_j$ has zero order along every branch, so the local-ring facts show that it extends to a nowhere-zero [holomorphic function](../../../complex-analysis.md#holomorphic-function). These germwise extensions patch uniquely to a holomorphic unit on the overlap. This describes a local defining function of $D$ and proves why multiplicities, not just zero sets, matter.

Set $g_{ij}=f_i/f_j$ and glue line-bundle frames by $e_j=g_{ij}e_i$. The identities $g_{ij}g_{jk}=g_{ik}$ give a [holomorphic line bundle associated to a divisor](../../../complex-geometry.md#holomorphic-line-bundle-associated-to-a-divisor), denoted $[D]$. Equivalently, the frame $e_i$ can be represented by $1/f_i$ in the sheaf of meromorphic functions, so $[D]=\mathcal O_X(D)$. If alternative equations are $f'_i=u_i f_i$, where $u_i$ are holomorphic units, the corresponding frames are identified by $e'_i\mapsto u_i^{-1}e_i$. This respects the changed transitions. Refining the cover gives the same identifications, proving that **$[D]$ is well-defined up to holomorphic bundle isomorphism**. The expressions $f_i e_i$ glue to its canonical meromorphic section, whose divisor is $D$.

For two [divisors on a complex manifold](../../../complex-geometry.md#divisor-on-a-complex-manifold) use a common cover with equations $f_i$ and $h_i$. Their sum has equation $f_i h_i$, and the [tensor product of vector bundles](../../../fiber-bundle.md#tensor-product-of-vector-bundles) has frame transitions

$$
\frac{f_i}{f_j}\frac{h_i}{h_j}=\frac{f_i h_i}{f_j h_j}.
$$

Sending the sum-divisor frame to the tensor product of the two frames gives

$$
\boxed{[D_1+D_2]\cong[D_1]\otimes[D_2].}
$$

This also yields $[-D]\cong[D]^*$.

For a nonsingular [complex analytic hypersurface](../../../complex-geometry.md#complex-analytic-hypersurface) $Y$, choose reduced local equations $f_i$ with $df_i$ nonzero along $Y$. The [holomorphic conormal bundle](../../../complex-geometry.md#holomorphic-conormal-bundle) is

$$
N^*_{Y/X}=\ker(\Omega_X^1|_Y\longrightarrow\Omega_Y^1),
$$

whose fibre is the annihilator of $T^{1,0}Y$. It has local frame $df_i|_Y$. Here this restriction is as a covector in the ambient cotangent bundle along $Y$, not its pullback to $\Omega_Y^1$, where it would vanish. The line bundle $[-Y]$ has local frame $a_i=f_i$, and if $f_j=u_{ji}f_i$, then

$$
a_j=u_{ji}a_i,\qquad
df_j|_Y=u_{ji}|_Y\,df_i|_Y,
$$

since $f_i\,du_{ji}$ vanishes along $Y$. The frame identifications $a_i|_Y\mapsto df_i|_Y$ therefore patch and are fibrewise nonzero. This proves the [conormal line of a smooth analytic hypersurface](../../../complex-geometry.md#conormal-line-of-a-smooth-analytic-hypersurface) formula

$$
\boxed{[-Y]|_Y\cong N^*_{Y/X}.}
$$

Equivalently it identifies $\mathcal O_X(-Y)|_Y=\mathcal I_Y/\mathcal I_Y^2$ with the analytic conormal sheaf.

## 4

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Choose [holomorphic coordinates](../../../complex-geometry.md#holomorphic-coordinate) centered at the point $p$ and a [polydisc](../../../complex-geometry.md#polydisc) $U\subset\mathbb C^n$ about the origin. The local [blowup of a complex manifold at a point](../../../complex-geometry.md#blowup-of-a-complex-manifold-at-a-point) is the incidence manifold

$$
\widetilde U=\{(z,[\ell])\in U\times\mathbb{CP}^{n-1}:z_i\ell_j=z_j\ell_i\text{ for all }i,j\},
\qquad\sigma(z,[\ell])=z.
$$

Away from $z=0$ the direction is forced to be $[\ell]=[z]$, giving a [biholomorphism](../../../complex-analysis.md#biholomorphism) with $U\setminus\{0\}$. Glue this punctured part to $X\setminus\{p\}$. The charts below make the result a [complex manifold](../../../complex-geometry.md#complex-manifold). The projection is proper near $p$, since it is the restriction of projection from a closed subset of $U\times\mathbb{CP}^{n-1}$; globally the modification is proper and is an isomorphism off $p$. Its [exceptional divisor](../../../complex-geometry.md#exceptional-divisor) is

$$
E=\sigma^{-1}(p)\cong\mathbb P(T_pX)\cong\mathbb{CP}^{n-1}.
$$

On $\ell_i\ne0$, let $t=z_i$ and $u_j=\ell_j/\ell_i$ for $j\ne i$. Then

$$
z_i=t,\qquad z_j=t u_j\ (j\ne i).
$$

These are coordinates on the open domain where $t$ and all $t u_j$ lie in the original polydisc; at $t=0$ all finite $u_j$ are allowed. Their inverse reads the direction ratios and $z_i$ from the incidence point. In this chart $E$ is the nonsingular hypersurface $t=0$. On overlap with chart $k\ne i$, the [holomorphic coordinate](../../../complex-geometry.md#holomorphic-coordinate) changes are

$$
t'=t u_k,\qquad u'_i=1/u_k,\qquad u'_j=u_j/u_k\quad(j\ne i,k).
$$

They are holomorphic with holomorphic inverses where $u_k\ne0$, and the $n$ charts cover every point of $E$. Intrinsically, changing the original coordinates by $F$ lifts via $[\ell]\mapsto[A(z)\ell]$, where $F(z)=A(z)z$, $A(0)=dF_0$, and $A$ is holomorphic and invertible near zero. One can take $A(z)=\int_0^1dF_{sz}\,ds$ on a sufficiently small polydisc. Away from the origin the lift is uniquely forced; this proves coordinate-independence of the gluing near $E$.

The [canonical bundle](../../../complex-geometry.md#canonical-bundle) is $K_X=\Lambda^n\Omega_X^1$. In the $i$th blowup chart the top-form Jacobian is

$$
\sigma^*(dz_1\wedge\cdots\wedge dz_n)
=(-1)^{i-1}t^{n-1}\,dt\wedge\bigwedge_{j\ne i}du_j,
$$

where the $u_j$ occur in increasing order. Every term with a second $dt$ vanishes in the [wedge product of differential forms](../../../differential-form.md#wedge-product-of-differential-forms). Thus the differential gives a map $\sigma^*K_X\to K_{\widetilde X}$ vanishing to order $n-1$ along $E$ and nowhere else. To express this through the supplied meromorphic-section hypothesis, take a nonzero meromorphic section $s$ of $K_X$ and put $D=\operatorname{div}(s)$. Locally $s=f(z)\,dz_1\wedge\cdots\wedge dz_n$, so

$$
\operatorname{div}(\sigma^*s)=\sigma^*D+(n-1)E.
$$

Here $\sigma^*D$ is the total divisor pullback, including any additional exceptional multiplicity from $f$; it is not merely the strict transform. A line bundle with a nonzero meromorphic section is isomorphic to the line bundle of that section's divisor, as its local coefficient ratios are its frame transitions. Pullback of divisor line bundles and [additivity of analytic divisor line bundles](../../../complex-geometry.md#additivity-of-analytic-divisor-line-bundles) therefore give the [canonical bundle formula for a point blowup](../../../complex-geometry.md#canonical-bundle-formula-for-a-point-blowup):

$$
\boxed{K_{\widetilde X}\cong\sigma^*K_X\otimes\mathcal O_{\widetilde X}((n-1)E).}
$$

For $n=1$ the blowup is already an isomorphism, consistently with the zero exponent.

For the projective-plane construction, an invertible linear change of homogeneous coordinates puts $x=[1:0:0]$. Lines through $x$ are parametrized by $[a:b]\in\mathbb{CP}^1$, with equation $bZ_1-aZ_2=0$. Thus the required map on the punctured plane is

$$
f([Z_0:Z_1:Z_2])=[Z_1:Z_2].
$$

It is well-defined under rescaling and holomorphic on the covering sets $Z_1\ne0$ and $Z_2\ne0$, where its target coordinates are $Z_2/Z_1$ and $Z_1/Z_2$. These sets cover the complement of $x$.

The graph closure is

$$
S=\{([Z_0:Z_1:Z_2],[a:b])\in\mathbb{CP}^2\times\mathbb{CP}^1:Z_1b=Z_2a\}.
$$

Over the complement of $x$ it is the graph of $f$. In the affine chart $Z_0\ne0$, its equation is exactly the two-dimensional local incidence model for the [blowup of a complex manifold at a point](../../../complex-geometry.md#blowup-of-a-complex-manifold-at-a-point), so its first projection identifies it with the required blowup globally. The second projection is a [holomorphic map](../../../complex-analysis.md#holomorphic-map) $\widetilde f:S\to\mathbb{CP}^1$ extending $f\circ\sigma$. Explicitly, the two blowup charts give

$$
(z_1,z_2)=(t,tu):\ \widetilde f=[1:u],\qquad
(z_1,z_2)=(tv,t):\ \widetilde f=[v:1].
$$

These formulas agree when $v=1/u$ and remain holomorphic at $t=0$. Hence **the pencil extends over the exceptional divisor, where it records the projective tangent direction**. This is the [projective pencil resolved by a point blowup](../../../complex-geometry.md#projective-pencil-resolved-by-a-point-blowup).

## 5

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Let $n=\dim_{\mathbb C}X$, and use the complex orientation. Write $g$ for the real [Riemannian metric](../../../differential-geometry.md#riemannian-metric) underlying the [Hermitian metric](../../../complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle). Its [fundamental form of a Hermitian manifold](../../../complex-geometry.md#fundamental-form-of-a-hermitian-manifold) is

$$
\omega(u,v)=g(Ju,v),\qquad
\omega=\frac{i}{2}\sum_{a,b}h_{a\bar b}\,dz^a\wedge d\bar z^b,
$$

where $g=\operatorname{Re}(\sum h_{a\bar b}\,dz^a\otimes d\bar z^b)$ in this convention. It is real and of type $(1,1)$, since $g(Ju,Jv)=g(u,v)$. Choose an adapted real orthonormal frame $E_j,F_j=JE_j$ and its dual coframe $e^j,f^j$. Then $\omega=\sum_j e^j\wedge f^j$, giving the [Riemannian volume form](../../../differential-geometry.md#riemannian-volume-form)

$$
\boxed{\operatorname{vol}_g=e^1\wedge f^1\wedge\cdots\wedge e^n\wedge f^n=\frac{\omega^n}{n!}.}
$$

We use the complex-linear [Hodge star operator](../../../differential-form.md#hodge-star-operator), the extension of the real metric star characterized on equal-degree forms by

$$
\alpha\wedge *\overline\beta=\langle\alpha,\beta\rangle_g\operatorname{vol}_g.
$$

It maps $(p,q)$-forms to $(n-q,n-p)$-forms and satisfies $**\alpha=(-1)^{p+q}\alpha$. It is distinct from the conjugate-linear map $\alpha\mapsto*\overline\alpha$. In the adapted coframe the star of $e^j\wedge f^j$ is the wedge product of all the other two-dimensional factors, with positive sign. Summing proves the [Hodge star of the fundamental Hermitian form](../../../complex-geometry.md#hodge-star-of-the-fundamental-hermitian-form) formula

$$
\boxed{*\omega=\frac{\omega^{n-1}}{(n-1)!}.}
$$

This computation uses no closedness assumption on $\omega$.

Use the integrated Hermitian inner product $(\alpha,\beta)=\int_X\alpha\wedge*\overline\beta$. The [formal adjoints](../../../hilbert-space.md#formal-adjoint) $d^*$ and $\bar\partial^*$ are defined by $(d\alpha,\beta)=(\alpha,d^*\beta)$ and $(\bar\partial\alpha,\beta)=(\alpha,\bar\partial^*\beta)$; compact manifolds here have no boundary. The [Hodge Laplacian](../../../differential-form.md#hodge-laplacian) and [Dolbeault Laplacian](../../../complex-geometry.md#dolbeault-laplacian) are

$$
\Delta_d=dd^*+d^*d,\qquad
\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial.
$$

The [Dolbeault Hodge decomposition on a compact Hermitian manifold](../../../complex-geometry.md#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold) states that

$$
\mathcal A^{p,q}(X)=\mathcal H_{\bar\partial}^{p,q}\oplus
\bar\partial\mathcal A^{p,q-1}(X)\oplus
\bar\partial^*\mathcal A^{p,q+1}(X)
$$

is an orthogonal direct sum, with finite-dimensional $\mathcal H_{\bar\partial}^{p,q}=\ker\Delta_{\bar\partial}$. Each [Dolbeault cohomology](../../../complex-geometry.md#dolbeault-cohomology) class

$$
H_{\bar\partial}^{p,q}(X)=\ker(\bar\partial:\mathcal A^{p,q}\to\mathcal A^{p,q+1})/\bar\partial\mathcal A^{p,q-1}
$$

has a unique representative in $\mathcal H_{\bar\partial}^{p,q}$. A form is harmonic exactly when both $\bar\partial\alpha$ and $\bar\partial^*\alpha$ vanish, since its Laplacian inner product is the sum of their squared norms.

Now let $L\alpha=\omega\wedge\alpha$ be the [Hermitian Lefschetz operator](../../../complex-geometry.md#lefschetz-operator-on-a-hermitian-manifold) and let $\Lambda$ be its pointwise adjoint. For $\beta$ of total degree $r=p+q$ and $\alpha$ of degree $r-2$, the defining inner products give

$$
(L\alpha)\wedge*\overline\beta
=\alpha\wedge\omega\wedge*\overline\beta
=\alpha\wedge*\overline{\Lambda\beta}.
$$

The wedge pairing is nondegenerate, so $*\overline{\Lambda\beta}=L*\overline\beta$. Apply another star to the degree-$(r-2)$ form and use that the star and $L$ commute with conjugation. This yields

$$
\boxed{\Lambda\beta=(-1)^{r-2}*L*\beta=(-1)^{p+q}*L*\beta.}
$$

For degrees below two both sides vanish. The argument also identifies its bidegree as $(-1,-1)$ and does not require the [Kähler](../../../complex-geometry.md#kahler-manifold) condition.

Assume now that $d\omega=0$, so the metric is a [Kähler metric](../../../complex-geometry.md#kahler-metric). Start with the supplied [Kähler identities](../../../complex-geometry.md#kahler-identities) relation $[\Lambda,\partial]=i\bar\partial^*$. Since $\Lambda$ is real, conjugation gives $[\Lambda,\bar\partial]=-i\partial^*$, hence

$$
\bar\partial^*=-i[\Lambda,\partial],\qquad
\partial^*=i[\Lambda,\bar\partial].
$$

The commutators are ordinary commutators because $\Lambda$ has even degree. Using $\partial^2=0$ we obtain, by direct expansion,

$$
\partial\bar\partial^*+\bar\partial^*\partial
=-i\left(\partial\Lambda\partial-\partial^2\Lambda+\Lambda\partial^2-\partial\Lambda\partial\right)=0.
$$

Conjugation gives $\bar\partial\partial^*+\partial^*\bar\partial=0$ as well. Expanding the two unmixed Laplacians and using $\partial\bar\partial=-\bar\partial\partial$ gives the same operator:

$$
\begin{aligned}
\Delta_\partial
&=i\left(\partial\Lambda\bar\partial-\bar\partial\Lambda\partial-\partial\bar\partial\Lambda-\Lambda\partial\bar\partial\right)\\
&=\Delta_{\bar\partial}.
\end{aligned}
$$

Finally expand $d=\partial+\bar\partial$ and $d^*=\partial^*+\bar\partial^*$; the mixed terms just proved zero disappear. This derives the [Kähler Laplacian identity](../../../complex-geometry.md#kahler-laplacian-identity)

$$
\boxed{\Delta_d=\Delta_\partial+\Delta_{\bar\partial}=2\Delta_{\bar\partial}.}
$$

The [Dolbeault Laplacian](../../../complex-geometry.md#dolbeault-laplacian) preserves bidegree. Thus the complex $d$-harmonic forms of total degree $r$ split into their harmonic $(p,q)$ parts. The allowed real [Hodge theorem](../../../differential-form.md#hodge-decomposition-theorem), followed by complexification, gives

$$
b^r(X)=\sum_{p+q=r}h^{p,q},\qquad h^{p,q}=\dim_{\mathbb C}\mathcal H_{\bar\partial}^{p,q}.
$$

The real operator $\Delta_d$ commutes with conjugation, which exchanges $(p,q)$ and $(q,p)$. Therefore $h^{p,q}=h^{q,p}$. For odd $r$, no summand has $p=q$, so they pair off in equal dimensions. This proves that **all odd Betti numbers are even**.

For $1\leq k\leq n$, the [Kähler form](../../../complex-geometry.md#kahler-form) power $\omega^k$ is closed. If it were exact, say $\omega^k=d\eta$, then

$$
\int_X\omega^n=\int_Xd(\eta\wedge\omega^{n-k})=0
$$

by [Stokes theorem](../../../calculus.md#stokes-theorem). But $\omega^n=n!\operatorname{vol}_g$ has strictly positive integral on the nonempty compact manifold. Hence the [powers of a compact Kähler form have nonzero cohomology classes](../../../complex-geometry.md#powers-of-a-compact-kahler-form-have-nonzero-cohomology-classes), and

$$
\boxed{b^{2k-1}(X)\in2\mathbb Z_{\geq0},\qquad b^{2k}(X)\geq1\quad(1\leq k\leq n).}
$$

For an example take the [Hopf surface](../../../complex-geometry.md#hopf-surface)

$$
H=(\mathbb C^2\setminus\{0\})/\langle z\mapsto2z\rangle.
$$

The dilation action is free and properly discontinuous: on a compact subset the radii are bounded above and away from zero, so only finitely many dilations can meet it. It is holomorphic, giving a [complex manifold](../../../complex-geometry.md#complex-manifold) quotient; the annulus $1\leq\|z\|\leq2$ covers the quotient, proving compactness. The map

$$
[z]\longmapsto\left(z/\|z\|,\ \log\|z\|\bmod\log2\right)
$$

is a [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) $H\cong S^3\times S^1$. The [Künneth theorem](../../../cohomology.md#kunneth-theorem) gives $b^1(H)=1$. This violates the necessary odd-degree parity, so **this compact complex surface admits no Kähler metric**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
