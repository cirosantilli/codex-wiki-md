# Paper 15

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper15.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper15.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

At a point $[X]\in\mathbf P^n$, the [complex tautological line bundle](../../../fiber-bundle.md#complex-tautological-line-bundle) has fiber $\mathbb CX\subseteq\mathbb C^{n+1}$. The [hyperplane line bundle](../../../fiber-bundle.md#hyperplane-line-bundle) is its dual, $[H]=\mathcal O(1)$, and $\mathcal O(m)=\mathcal O(1)^{\otimes m}$. On $U_i=\{X_i\ne0\}$ let $t_i=X/X_i$ be the tautological frame and $e_i$ its dual. On overlaps $e_j=(X_j/X_i)e_i$. The [sheaf of holomorphic sections of a vector bundle](../../../complex-geometry.md#sheaf-of-holomorphic-sections-of-a-vector-bundle) of this dual bundle is the sheaf $\mathcal O_{\mathbf P^n}(1)$.

If a nonzero linear form $\ell$ cuts out the [projective hyperplane](../../../algebraic-topology.md#projective-hyperplane) $H$, it gives a [holomorphic section](../../../complex-geometry.md#holomorphic-section) $s_H$ of $\mathcal O(1)$ with a simple zero along $H$. Dividing a local section $s$ by $s_H$ gives a [meromorphic function](../../../isolated-singularity.md#meromorphic-function) with no poles away from $H$ and at most a simple pole on $H$. Conversely multiplication by $s_H$ turns such a function into a [holomorphic section](../../../complex-geometry.md#holomorphic-section). These mutually inverse local constructions agree on overlaps and prove the [holomorphic line bundle associated to a divisor](../../../complex-geometry.md#holomorphic-line-bundle-associated-to-a-divisor) identification

$$
\boxed{\mathcal O(1)\cong\mathcal O(H).}
$$

The [nonnegative hyperplane twist cohomology by restriction](../../../projective-space.md#nonnegative-hyperplane-twist-cohomology-by-restriction) calculation gives

$$
\boxed{h^r(\mathbf P^n,\mathcal O(m))=\begin{cases}\binom{n+m}{n},&r=0,\\0,&r>0.\end{cases}}
$$

To derive it from the permitted vanishing, use the [hyperplane exact sequence for twisting sheaves](../../../ringed-space.md#hyperplane-exact-sequence-for-twisting-sheaves)

$$
0\longrightarrow\mathcal O_{\mathbf P^n}(m-1)\xrightarrow{\,s_H\,}\mathcal O_{\mathbf P^n}(m)
\longrightarrow i_*\mathcal O_H(m)\longrightarrow0,
$$

where $i:H\hookrightarrow\mathbf P^n$ and $H\cong\mathbf P^{n-1}$. Local multiplication by a defining equation is injective, and restriction gives exactly its cokernel. Induct on $n$, starting from a point, and then on $m$. For $m=0$, higher [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) vanishes by assumption and global [holomorphic functions](../../../complex-analysis.md#holomorphic-function) are constant by compactness and the maximum principle. For $m>0$, the [long exact sequence in sheaf cohomology](../../../ringed-space.md#long-exact-sequence-in-sheaf-cohomology), the inductive vanishing for $\mathcal O(m-1)$ and the dimension induction on $H$ give vanishing in every positive degree and

$$
h^0(\mathbf P^n,\mathcal O(m))-h^0(\mathbf P^n,\mathcal O(m-1))=\binom{n-1+m}{n-1}.
$$

Summing this recurrence gives $\binom{n+m}{n}$. Homogeneous degree-$m$ monomials give that many independent sections, so they form a basis. The printed extra equality to zero cannot hold in degree zero, already because $h^0(\mathbf P^n,\mathcal O)=1$; the boxed calculation gives the intended dimensions.

For the [differential of the projective quotient map](../../../algebraic-topology.md#differential-of-the-projective-quotient-map), the [differential of a smooth map](../../../differential-geometry.md#differential-of-a-smooth-map) is computed by applying a tangent vector to coordinate functions. Since $x_j=X_j/X_0$,

$$
\frac{\partial x_j}{\partial X_i}=\frac{\delta_{ij}}{a_0}\quad(i>0),\qquad
\frac{\partial x_j}{\partial X_0}=-\frac{a_j}{a_0^2}.
$$

Thus

$$
\boxed{\pi_*\left(\frac\partial{\partial X_i}\right)=\frac1{a_0}\frac\partial{\partial x_i}\ (i>0),\qquad
\pi_*\left(\frac\partial{\partial X_0}\right)=-\sum_{j=1}^n\frac{a_j}{a_0^2}\frac\partial{\partial x_j}.}
$$

Under replacing $X$ by $\lambda X$, $d\pi$ on a constant ambient tangent vector scales by $\lambda^{-1}$, while a homogeneous linear form $L$ scales by $\lambda$. Therefore $d\pi_X(L(X)\partial_{X_j})$ is independent of the representative. Its chart coefficients are holomorphic, so it is a global [holomorphic vector field](../../../complex-geometry.md#holomorphic-vector-field). The radial [Euler vector field](../../../complex-geometry.md#euler-vector-field) lies in the kernel of $d\pi$, either from the same formulas or because it differentiates a scaling orbit. Hence

$$
\boxed{\pi_*\left(\sum_{i=0}^nX_i\partial_{X_i}\right)=0.}
$$

Describe the [Euler sequence on complex projective space](../../../algebraic-topology.md#euler-sequence-on-complex-projective-space) fiberwise as well as in coordinates. At a line $\ell=\mathbb CX$, the middle bundle has fiber $\operatorname{Hom}(\ell,\mathbb C^{n+1})$ and the [holomorphic tangent bundle](../../../complex-geometry.md#holomorphic-tangent-bundle) has fiber $\operatorname{Hom}(\ell,\mathbb C^{n+1}/\ell)$. Send a homomorphism to its composition with the quotient. The map from $\mathcal O$ sends a scalar to that scalar times the inclusion $\ell\hookrightarrow\mathbb C^{n+1}$. In homogeneous notation these maps are

$$
f\longmapsto(fX_0,\ldots,fX_n),\qquad
(s_0,\ldots,s_n)\longmapsto d\pi_X\left(\sum_js_j(X)\partial_{X_j}\right).
$$

A local section of $\mathcal O(1)$ is a local degree-one homogeneous function on the punctured cone, so the second expression is representative-independent. Quotienting is surjective, and its kernel consists exactly of scalar inclusion maps. This proves the short exact sequence of [locally free sheaves](../../../ringed-space.md#locally-free-sheaf)

$$
\boxed{0\to\mathcal O\to\mathcal O(1)^{\oplus(n+1)}\to\mathcal O(T')\to0.}
$$

Since it is locally split, dualizing and tensoring by $\mathcal O(1)$ preserves exactness and gives the [cotangent Euler sequence in homogeneous coordinates](../../../algebraic-geometry.md#cotangent-euler-sequence-in-homogeneous-coordinates)

$$
0\to\Omega^1(1)\to\mathcal O^{\oplus(n+1)}\xrightarrow{(c_i)\mapsto\sum_i c_iX_i}\mathcal O(1)\to0.
$$

On global sections the last map identifies $\mathbb C^{n+1}$ with the basis of linear forms in $H^0(\mathcal O(1))$. Its kernel is zero. This proves the [vanishing of global sections of the once-twisted projective cotangent bundle](../../../algebraic-geometry.md#vanishing-of-global-sections-of-the-once-twisted-projective-cotangent-bundle); left exactness gives **$\boxed{h^0(\mathbf P^n,\Omega^1(1))=0}$**.

## 2

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

An [almost complex structure](../../../complex-geometry.md#almost-complex-manifold) is a smooth endomorphism $J:TM\to TM$ with $J^2=-I$; in particular the real dimension is even. Complexifying the [tangent bundle](../../../fiber-bundle.md#tangent-bundle) splits it into the $i$ and $-i$ eigensubbundles

$$
T_{\mathbb C}M=T^{1,0}M\oplus T^{0,1}M,
$$

interchanged by conjugation. On a [complex manifold](../../../complex-geometry.md#complex-manifold), these are locally spanned by $\partial_{z^j}$ and $\partial_{\bar z^j}$. An [integrable almost complex structure](../../../complex-geometry.md#integrable-almost-complex-structure) is one arising from a holomorphic coordinate atlas. Its $T^{0,1}$ sections are closed under the [Lie bracket](../../../lie-algebra.md#lie-bracket). The obstruction is the [Nijenhuis tensor](../../../complex-geometry.md#nijenhuis-tensor)

$$
N_J(X,Y)=[JX,JY]-J[JX,Y]-J[X,JY]-[X,Y].
$$

Expanding this expression in the two eigentypes shows that $N_J=0$ is equivalent to involutivity of $T^{0,1}$. Holomorphic coordinates make this condition necessary; the [Newlander-Nirenberg theorem](../../../complex-geometry.md#newlander-nirenberg-theorem) gives its sufficiency for smooth $J$. Integrability also gives $d=\partial+\bar\partial$, with $\partial^2=\bar\partial^2=0$ and $\partial\bar\partial+\bar\partial\partial=0$. The [Dolbeault operator](../../../complex-geometry.md#dolbeault-operator) on $T^{1,0}M=T'_M$ defines its [holomorphic vector bundle](../../../complex-geometry.md#holomorphic-vector-bundle) structure.

A real [connection on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle) $\nabla$ on $TM$ preserves $J$ when $\nabla J=0$. Its complexification then preserves both eigensubbundles. Restricting to $T'_M$ gives a complex connection $D$. Conversely any complex connection on $T'_M$ gives such a real connection by adjoining its conjugate on $T^{0,1}$ and restricting to the conjugation-fixed real tangent bundle. Equivalently, transfer $D$ through the real isomorphism $v\mapsto(v-iJv)/2$. These operations are inverse. **Preserving $J$ alone does not impose the holomorphic compatibility condition $D^{0,1}=\bar\partial_{T'}$.**

For integrable $J$, the latter condition has a precise real-connection interpretation: the mixed-type [torsion tensor](../../../fiber-bundle.md#torsion-tensor) vanishes. In holomorphic coordinates it says $D_{\partial_{\bar z^i}}\partial_{z^j}=0$. Reality also gives $\nabla_{\partial_{z^j}}\partial_{\bar z^i}=0$. Since these coordinate fields commute, their torsion is zero. Conversely a $J$-preserving real connection with zero mixed torsion has these two derivatives equal; they belong to opposite eigentypes, so both vanish, proving $D^{0,1}=\bar\partial_{T'}$. This is the [holomorphic tangent connection and mixed torsion criterion](../../../complex-geometry.md#holomorphic-tangent-connection-and-mixed-torsion-criterion).

Full torsion-freeness imposes the additional symmetry $\Gamma^k_{ij}=\Gamma^k_{ji}$ in $D_{\partial_{z^i}}\partial_{z^j}=\Gamma^k_{ij}\partial_{z^k}$, and its conjugate. Such a $J$-preserving torsion-free connection exists on any [complex manifold](../../../complex-geometry.md#complex-manifold): local holomorphic-coordinate flat connections have these properties, and a real [partition of unity](../../../differential-geometry.md#partition-of-unity) combines them globally. Preservation of $J$ and zero torsion persist because both conditions are affine in the connection. Conversely if $J$ is merely almost complex, a torsion-free connection preserving it forces $N_J=0$: replace brackets by $\nabla_XY-\nabla_YX$ in the displayed tensor and use $\nabla J=0$; all terms cancel. Thus this connection condition detects integrability, without imposing any metric condition.

A [Hermitian metric](../../../complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle) is a real [Riemannian metric](../../../differential-geometry.md#riemannian-metric) $g$ with $g(JX,JY)=g(X,Y)$. It induces a Hermitian metric $h$ on $T'_M$ and the fundamental two-form $\omega(X,Y)=g(JX,Y)$. The unique [Chern connection](../../../complex-geometry.md#chern-connection) satisfies both $D^{0,1}=\bar\partial_{T'}$ and metric compatibility. In a holomorphic frame with metric matrix $H$ and coefficient-column convention, its matrix is $H^{-1}\partial H$. It need not be torsion-free when transferred to $TM$.

In holomorphic coordinates its coefficients are $\Gamma^k_{ij}=h^{k\bar l}\partial_i h_{j\bar l}$. Their symmetry in $i,j$ is equivalent to $\partial_i h_{j\bar l}=\partial_j h_{i\bar l}$, which says $\partial\omega=0$. The conjugate gives $\bar\partial\omega=0$. The result that a [torsion-free Chern tangent connection characterizes a Kähler metric](../../../complex-geometry.md#torsion-free-chern-tangent-connection-characterizes-a-kahler-metric) follows: **the transferred Chern connection is torsion-free exactly when $\boxed{d\omega=0}$**, the [Kähler metric](../../../complex-geometry.md#kahler-metric) condition. In that case it equals the [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection), by uniqueness of the metric-compatible torsion-free connection. Equivalently a Hermitian metric is Kähler exactly when its [Levi-Civita connection](../../../general-relativity.md#levi-civita-connection) preserves $J$. In the reverse direction $\nabla J=0$ implies $\nabla\omega=0$, and zero torsion gives $d\omega=0$.

This explains the role of [Kähler metrics](../../../complex-geometry.md#kahler-metric): they make the real Riemannian and holomorphic connection theories coincide. A general [complex manifold](../../../complex-geometry.md#complex-manifold) has torsion-free $J$-preserving connections and has Hermitian metrics, but need not have a connection satisfying both requirements simultaneously. On a [Kähler manifold](../../../complex-geometry.md#kahler-manifold), the [Kähler identities](../../../complex-geometry.md#kahler-identities) then link the [Dolbeault Laplacian](../../../complex-geometry.md#dolbeault-laplacian) and [Hodge Laplacian](../../../differential-form.md#hodge-laplacian), giving $\Delta_d=2\Delta_{\bar\partial}=2\Delta_\partial$ and the resulting harmonic [Hodge decomposition theorem for compact Kähler manifolds](../../../complex-geometry.md#hodge-decomposition-theorem-for-compact-kahler-manifolds).

## 3

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a smooth complex [vector bundle](../../../fiber-bundle.md#vector-bundle) $E$, a connection is a complex-linear map $D:\Gamma(E)\to A^1(M;E)$ satisfying $D(fs)=df\otimes s+fDs$ for smooth complex functions $f$. Local trivializations supply flat local connections. A locally finite smooth [partition of unity](../../../differential-geometry.md#partition-of-unity) $(\rho_i)$ subordinate to them gives $D=\sum_i\rho_iD_i$; local finiteness makes the sum smooth and $\sum_i\rho_i=1$ gives the [Leibniz rule](../../../calculus.md#leibniz-rule). Thus [connections on a vector bundle](../../../fiber-bundle.md#connection-vector-bundle) always exist on the usual paracompact smooth manifold.

Extend $D$ to bundle-valued forms by $D(\alpha\otimes s)=d\alpha\otimes s+(-1)^{\deg\alpha}\alpha\wedge Ds$. Squaring shows that $D^2(fs)=fD^2s$, so the [curvature form](../../../fiber-bundle.md#curvature-form) is the endomorphism-valued two-form $\Theta=D^2$. With a row frame $e=(e_1,\ldots,e_r)$, write $De=eA$; for coefficient columns $s=ev$, $Ds=e(dv+Av)$. Applying $D$ again and using the graded [Leibniz rule](../../../calculus.md#leibniz-rule) gives

$$
D^2(ev)=e(dA+A\wedge A)v.
$$

The cross terms $-A\wedge dv$ and $A\wedge dv$ cancel. Hence the [Cartan curvature matrix equation](../../../fiber-bundle.md#cartan-curvature-matrix-equation) in this convention is

$$
\boxed{\Theta=dA+A\wedge A.}
$$

For a frame change $e'=eg$, the [connection matrix](../../../fiber-bundle.md#connection-one-form) and curvature transform as $A'=g^{-1}Ag+g^{-1}dg$ and $\Theta'=g^{-1}\Theta g$. Trace is invariant under conjugation, so the local forms $\operatorname{Tr}\Theta$ patch into the global [trace of vector-bundle curvature](../../../fiber-bundle.md#trace-of-vector-bundle-curvature).

The induced [determinant connection](../../../fiber-bundle.md#determinant-connection) on $\det E=\Lambda^rE$ is

$$
D_r(s_1\wedge\cdots\wedge s_r)=\sum_{j=1}^r s_1\wedge\cdots\wedge Ds_j\wedge\cdots\wedge s_r,
$$

where the one-form factor of each $Ds_j$ is placed in front of the section factors. In the local determinant frame $e_1\wedge\cdots\wedge e_r$, only the diagonal terms survive, so its connection form is $\operatorname{Tr}A$. Its curvature is $d\operatorname{Tr}A$. Since

$$
\operatorname{Tr}(A\wedge A)=\sum_{i,j}A_{ij}\wedge A_{ji}=0
$$

by pairing off-diagonal terms and using $A_{ii}\wedge A_{ii}=0$, we obtain

$$
\boxed{\Theta_{D_r}=d\operatorname{Tr}A=\operatorname{Tr}\Theta_D.}
$$

It is closed locally by $d^2=0$, and thus closed globally.

For two connections, $B=D_1-D_0$ is a global endomorphism-valued one-form: the derivative terms cancel in their Leibniz rules. In a local frame $A_1=A_0+B$, so

$$
\Theta_1-\Theta_0=dB+A_0\wedge B+B\wedge A_0+B\wedge B.
$$

Taking traces cancels the mixed terms, because both factors are one-forms, and cancels $\operatorname{Tr}(B\wedge B)$. Therefore the [trace curvature transgression](../../../fiber-bundle.md#trace-curvature-transgression) formula is

$$
\boxed{\operatorname{Tr}\Theta_1-\operatorname{Tr}\Theta_0=d\operatorname{Tr}B.}
$$

The right-hand side is globally exact, proving independence of the [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) class without needing a sheaf-cohomology identification.

Finally let $e$ be a holomorphic frame for the [holomorphic line bundle](../../../complex-geometry.md#holomorphic-line-bundle), with $h=\|e\|^2>0$. Define $De=e\,\partial\log h$, extending by the Leibniz rule. If $e'=eg$ for a nowhere-zero holomorphic function $g$, then $h'=|g|^2h$ and

$$
\partial\log h'=\partial\log h+g^{-1}dg.
$$

This is exactly the line-bundle frame-change law for a connection, so the local definitions glue globally. Its $(0,1)$ part is the [Dolbeault operator](../../../complex-geometry.md#dolbeault-operator). Metric compatibility follows from $d\log h=\partial\log h+\bar\partial\log h$, or $dh=h(A+\overline A)$ for $A=\partial\log h$. These conditions uniquely force this $A$, identifying the [Chern connection](../../../complex-geometry.md#chern-connection). Since a scalar one-form wedges with itself to zero,

$$
\boxed{\Theta=d(\partial\log h)=\bar\partial\partial\log h=-\partial\bar\partial\log h.}
$$

This agrees with the [local formula for the Chern connection on a line bundle](../../../complex-geometry.md#local-formula-for-the-chern-connection-on-a-line-bundle); keeping the order of the two Dolbeault differentials fixes the sign.

## 4

↑ **Parent:** [Paper 15](paper-15.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [Hermitian metric](../../../complex-geometry.md#hermitian-metric-on-a-holomorphic-vector-bundle) induces pointwise Hermitian inner products on the exterior powers of the complex [cotangent bundle](../../../symplectic-geometry.md#cotangent-bundle), with different bidegrees orthogonal, and a positive volume form $dV_g$. Thus the global $L^2$ inner product on smooth [differential forms](../../../differential-form.md) of type $(p,q)$ is

$$
\langle\alpha,\beta\rangle_{L^2}=\int_M\langle\alpha(x),\beta(x)\rangle_g\,dV_g.
$$

Let $\bar\partial^*$ be the formal adjoint of the [Dolbeault operator](../../../complex-geometry.md#dolbeault-operator), defined by integration by parts, and let $\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial$. This [Dolbeault Laplacian](../../../complex-geometry.md#dolbeault-laplacian) preserves bidegree, is elliptic and nonnegative, and has

$$
\langle\Delta_{\bar\partial}\alpha,\alpha\rangle=\|\bar\partial\alpha\|^2+\|\bar\partial^*\alpha\|^2.
$$

On a compact Hermitian manifold without boundary, the [Dolbeault Hodge decomposition on a compact Hermitian manifold](../../../complex-geometry.md#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold) says that the smooth harmonic space $\mathcal H_{\bar\partial}^{p,q}=\ker\Delta_{\bar\partial}$ is finite-dimensional and

$$
A^{p,q}=\mathcal H_{\bar\partial}^{p,q}\mathbin{\oplus^\perp}\Delta_{\bar\partial}A^{p,q}.
$$

More precisely, there are the orthogonal harmonic projection $H$ and a [Dolbeault Green operator](../../../complex-geometry.md#dolbeault-green-operator) $G$ taking smooth forms to smooth forms, with $G=0$ on harmonics and $\Delta_{\bar\partial}G=G\Delta_{\bar\partial}=I-H$. Elliptic regularity ensures these are statements about smooth forms, not only $L^2$ completions. The Green operator commutes with $\bar\partial$ and $\bar\partial^*$, since the Laplacian does and its inverse is unique on the orthogonal complement of the kernel.

Expanding $\alpha=H\alpha+\Delta_{\bar\partial}G\alpha$ gives

$$
\boxed{A^{p,q}=\mathcal H_{\bar\partial}^{p,q}\oplus\bar\partial A^{p,q-1}\oplus\bar\partial^*A^{p,q+1}.}
$$

The three summands are orthogonal: harmonic forms are killed by both adjoints, and $\langle\bar\partial u,\bar\partial^*v\rangle=\langle\bar\partial^2u,v\rangle=0$. If $\alpha$ is $\bar\partial$-closed, its coexact component is orthogonal to every closed form; taking its inner product with $\alpha$ shows that component has norm zero. Conversely the first two components are closed. Thus **$\boxed{\ker\bar\partial=\mathcal H_{\bar\partial}^{p,q}\oplus\bar\partial A^{p,q-1}}$**, with out-of-range form spaces taken to be zero.

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

On the [Kähler manifold](../../../complex-geometry.md#kahler-manifold) define $L\alpha=\omega\wedge\alpha$ using the [Kähler form](../../../complex-geometry.md#kahler-form); the operator $\Lambda=L^*$ is the [adjoint Lefschetz operator](../../../complex-geometry.md#adjoint-lefschetz-operator), the pointwise contraction adjoint to wedging with $\omega$. It lowers bidegree by $(1,1)$. Set

$$
\Delta_d=dd^*+d^*d,\qquad \Delta_\partial=\partial\partial^*+\partial^*\partial,
$$

and keep $\Delta_{\bar\partial}$ as above. These are the [Hodge Laplacian](../../../differential-form.md#hodge-laplacian) and the holomorphic and antiholomorphic Laplacians respectively. The permitted identity among the [Kähler identities](../../../complex-geometry.md#kahler-identities) $[\Lambda,\partial]=i\bar\partial^*$ gives $\bar\partial^*=-i[\Lambda,\partial]$. Expanding rather than assuming the desired anticommutation,

$$
\partial\bar\partial^*+\bar\partial^*\partial
=-i\bigl(\partial\Lambda\partial-\partial^2\Lambda+\Lambda\partial^2-\partial\Lambda\partial\bigr)=0,
$$

because $\partial^2=0$. Hence **$\boxed{\partial\bar\partial^*+\bar\partial^*\partial=0}$**.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Complex conjugation preserves the real [Kähler form](../../../complex-geometry.md#kahler-form) and interchanges $\partial,\bar\partial$ and their formal adjoints. Conjugating the permitted identity among the [Kähler identities](../../../complex-geometry.md#kahler-identities) therefore yields $[\Lambda,\bar\partial]=-i\partial^*$. The same nilpotence calculation as in part (a) gives $\bar\partial\partial^*+\partial^*\bar\partial=0$. Now expand $d=\partial+\bar\partial$ and $d^*=\partial^*+\bar\partial^*$:

$$
\Delta_d=\Delta_\partial+\Delta_{\bar\partial}
+\partial\bar\partial^*+\bar\partial^*\partial
+\bar\partial\partial^*+\partial^*\bar\partial.
$$

Both mixed anticommutators vanish, proving **$\boxed{\Delta_d=\Delta_\partial+\Delta_{\bar\partial}}$**.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Use both [Kähler identities](../../../complex-geometry.md#kahler-identities) from the preceding parts, so that $\partial^*=i[\Lambda,\bar\partial]$ and $\bar\partial^*=-i[\Lambda,\partial]$. For odd operators $a,b$, write $\{a,b\}=ab+ba$. Direct expansion gives

$$
\{\partial,[\Lambda,\bar\partial]\}+\{\bar\partial,[\Lambda,\partial]\}
=[\Lambda,\{\partial,\bar\partial\}]=0.
$$

Since $\partial\bar\partial+\bar\partial\partial=0$, we obtain

$$
\Delta_\partial=i\{\partial,[\Lambda,\bar\partial]\}
=-i\{\bar\partial,[\Lambda,\partial]\}=\Delta_{\bar\partial}.
$$

Together with part (b), this proves the full [Kähler Laplacian identity](../../../complex-geometry.md#kahler-laplacian-identity)

$$
\boxed{\Delta_d=2\Delta_\partial=2\Delta_{\bar\partial}.}
$$

Now take the exact form $\eta$. Being $\bar\partial$-exact, it is orthogonal to the harmonic space, so $H\eta=0$, and it is also $\bar\partial$-closed. Choose $\alpha=G\eta$ for the [Dolbeault Green operator](../../../complex-geometry.md#dolbeault-green-operator) of the [Dolbeault Laplacian](../../../complex-geometry.md#dolbeault-laplacian). Commutation gives $\bar\partial\alpha=G\bar\partial\eta=0$. Therefore

$$
\boxed{\eta=\Delta_{\bar\partial}\alpha=\bar\partial\bar\partial^*\alpha.}
$$

Suppose also $\partial\eta=0$, and put $v=\bar\partial^*\alpha$, $u=\partial v$. The mixed identities and $(\bar\partial^*)^2=0$ give

$$
\bar\partial u=-\partial\bar\partial v=-\partial\eta=0,\qquad
\bar\partial^*u=-\partial\bar\partial^*v=0.
$$

Thus $u=\partial\bar\partial^*\alpha$ is harmonic for the [Dolbeault Laplacian](../../../complex-geometry.md#dolbeault-laplacian). By the [Kähler Laplacian identity](../../../complex-geometry.md#kahler-laplacian-identity) it is also $\partial$-harmonic and hence $\partial^*u=0$. But it is $\partial$-exact, so

$$
\|u\|^2=\langle\partial v,u\rangle=\langle v,\partial^*u\rangle=0.
$$

Consequently **$\boxed{\partial\bar\partial^*\alpha=0}$**: the form $v$ is $\partial$-closed.

For every harmonic form $h$ of the same bidegree as $v$, $\langle v,h\rangle=\langle\alpha,\bar\partial h\rangle=0$. Harmonic spaces for the two Dolbeault Laplacians coincide, so $v$ has no $\partial$-harmonic component. Apply the $\partial$ version of the [Dolbeault Hodge decomposition](../../../complex-geometry.md#dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold). Since $v$ is $\partial$-closed, it has no $\partial^*$-coexact component either. Thus $v=\partial\phi$, with $\phi\in A^{p-1,q-1}$. We conclude the requested [ddbar lemma](../../../complex-geometry.md#ddbar-lemma):

$$
\boxed{\eta=\bar\partial\partial\phi.}
$$

For example $\phi=\partial^*Gv$ is a choice, since the same Green operator serves $\Delta_\partial=\Delta_{\bar\partial}$. If $p=0$ or $q=0$, the relevant negative-bidegree space is zero and the argument forces $\eta=0$. Compactness, the absence of boundary and the [Kähler](../../../complex-geometry.md#kahler-manifold) condition are essential to this global harmonic argument.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
