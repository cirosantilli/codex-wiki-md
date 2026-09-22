# Paper 51

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_51.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_51.pdf)

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

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $P=(\omega^{ab})$ be a smooth [antisymmetric matrix](../../../linear-algebra.md#skew-symmetric-matrix) field. It defines a [Poisson bivector](../../../symplectic-geometry.md#poisson-bivector) through

$$
\{f,g\}=\omega^{ab}(x)\,\partial_af\,\partial_bg,\qquad f,g\in C^\infty(U).
$$

This [Poisson bracket](../../../classical-mechanics.md#poisson-bracket) is bilinear, antisymmetric and a [derivation](../../../associative-algebra.md#derivation-of-an-algebra) in each argument. It defines a [Poisson manifold](../../../symplectic-geometry.md#poisson-manifold) when it also satisfies the [Jacobi identity](../../../lie-algebra.md#jacobi-identity). Apply that identity in the form $\{\{f,g\},h\}+\{\{g,h\},f\}+\{\{h,f\},g\}=0$ to the coordinate functions. Since $\{x^a,x^b\}=\omega^{ab}$, it gives

$$
\boxed{J^{abc}:=\omega^{dc}\partial_d\omega^{ab}
+\omega^{db}\partial_d\omega^{ca}
+\omega^{da}\partial_d\omega^{bc}=0.}
$$

This is the [coordinate Jacobi condition for a Poisson bivector](../../../symplectic-geometry.md#coordinate-jacobi-condition-for-a-poisson-bivector). It is also sufficient: in the [Jacobi identity](../../../lie-algebra.md#jacobi-identity) for arbitrary functions the terms containing second derivatives cancel by antisymmetry, leaving $J^{abc}(\partial_af)(\partial_bg)(\partial_ch)$. Thus the coordinate condition captures the whole obstruction.

Now suppose the [Poisson bivector](../../../symplectic-geometry.md#poisson-bivector) is nondegenerate. Write $S=P^{-1}$, so $S_{ab}\omega^{bc}=\delta_a^c$, and define the [2-form](../../../differential-form.md#2-form)

$$
\Omega=\frac12 S_{ab}\,dx^a\wedge dx^b.
$$

An overall minus sign in identifying the [symplectic form](../../../symplectic-geometry.md#symplectic-form) depends on the convention for [Hamiltonian vector fields](../../../symplectic-geometry.md#hamiltonian-vector-field); it does not affect the closure argument. Differentiating the inverse matrix gives

$$
\partial_dS_{ij}=-S_{ia}(\partial_d\omega^{ab})S_{bj}
=S_{ia}S_{jb}\partial_d\omega^{ab}.
$$

Contract the coordinate [Jacobi identity](../../../lie-algebra.md#jacobi-identity) with $S_{ia}S_{jb}S_{kc}$. Antisymmetry gives $\omega^{dc}S_{kc}=-\delta_k^d$, and similarly for the other terms, hence

$$
S_{ia}S_{jb}S_{kc}J^{abc}
=-\{\partial_kS_{ij}+\partial_jS_{ki}+\partial_iS_{jk}\}=0.
$$

The cyclic expression is precisely the coefficient of the [exterior derivative](../../../differential-form.md#exterior-derivative) $d\Omega$. Therefore

$$
\boxed{d\Omega=0.}
$$

Since $S$ is antisymmetric and nondegenerate, $\Omega$ is a [symplectic form](../../../symplectic-geometry.md#symplectic-form). This proves the [closure of the inverse of a nondegenerate Poisson bivector](../../../symplectic-geometry.md#closure-of-the-inverse-of-a-nondegenerate-poisson-bivector). The matrix entries $\omega^{ab}$ are scalar functions; the codomain in the source's matrix description should be read as the space of antisymmetric matrices, rather than a vector-valued individual entry.

## 2

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Multiplying the matrices gives the [Heisenberg group](../../../lie-algebra.md#heisenberg-group) law

$$
(x,y,z)(a,b,c)=(x+a,y+b,z+c+xb),\qquad
(x,y,z)^{-1}=(-x,-y,-z+xy).
$$

Differentiating at the identity gives all strictly upper-triangular matrices. With $X=E_{12}$, $Y=E_{23}$ and $Z=E_{13}$, the [commutator](../../../lie-algebra.md#commutator) gives

$$
\boxed{\mathfrak g=\operatorname{span}\{X,Y,Z\},\qquad [X,Y]=Z,\quad [X,Z]=[Y,Z]=0.}
$$

This is the [Heisenberg Lie algebra](../../../lie-algebra.md#heisenberg-lie-algebra).

The right [Maurer-Cartan form](../../../lie-theory.md#maurer-cartan-form) is

$$
dg\,g^{-1}=X\,dx+Y\,dy+Z\,(dz-y\,dx).
$$

Thus the [right-invariant coframe of the real Heisenberg group](../../../lie-algebra.md#right-invariant-coframe-of-the-real-heisenberg-group) is $\sigma^1=dx$, $\sigma^2=dy$, $\sigma^3=dz-y\,dx$. Under a right translation,

$$
R_{(a,b,c)}(x,y,z)=(x+a,y+b,z+c+xb),
$$

we have $dx'=dx$, $dy'=dy$, and $dz'-y'dx'=dz-y\,dx$. All three [right-invariant differential forms](../../../lie-theory.md#right-invariant-differential-form) are preserved.

Every [right-invariant Riemannian metric](../../../lie-theory.md#right-invariant-riemannian-metric) is determined by an arbitrary [inner product](../../../linear-algebra.md#inner-product) at the identity. In this coframe its most general expression is

$$
\boxed{h=H_{ij}\,\sigma^i\sigma^j,\qquad H=H^{\mathsf T}>0,\quad H_{ij}\text{ constant}.}
$$

Equivalently,

$$
\begin{aligned}
h={}&H_{11}dx^2+H_{22}dy^2+H_{33}(dz-y\,dx)^2\\
&+2H_{12}dx\,dy+2H_{13}dx(dz-y\,dx)+2H_{23}dy(dz-y\,dx).
\end{aligned}
$$

Products here are symmetric products. If a pseudo-Riemannian [metric tensor](../../../general-relativity.md#metric-tensor) is intended, replace positive definiteness by nondegeneracy. Since every right translation preserves the coframe, it is an [isometry](../../../riemannian-geometry.md#isometry). The action is faithful, and $a\mapsto R_{a^{-1}}$ is a group homomorphism, embedding a copy of $G$ into the [isometry group](../../../riemannian-geometry.md#isometry-group).

The one-parameter right translations produce the [Killing frame for a right-invariant Heisenberg metric](../../../lie-algebra.md#killing-frame-for-a-right-invariant-heisenberg-metric):

$$
\boxed{K_X=\partial_x,\qquad K_Y=\partial_y+x\partial_z,\qquad K_Z=\partial_z.}
$$

Their flows are respectively $(x+t,y,z)$, $(x,y+t,z+xt)$ and $(x,y,z+t)$. Each preserves $h$, and their [Lie brackets of vector fields](../../../differential-geometry.md#lie-bracket-of-vector-fields) are $[K_X,K_Y]=K_Z$, with the other two zero. This explicitly realizes the [Heisenberg Lie algebra](../../../lie-algebra.md#heisenberg-lie-algebra). These [Killing vector fields](../../../general-relativity.md#killing-vector-field) are left-invariant vector fields; the vector fields dual to the right-invariant coframe are instead $\partial_x+y\partial_z,\partial_y,\partial_z$, and should not be substituted for these generators.

For the diagonal case, put

$$
h=\alpha\,dx^2+\beta\,dy^2+\chi(dz-y\,dx)^2,\qquad \alpha,\beta,\chi>0.
$$

The [Kaluza-Klein decomposition along a Killing field](../../../general-relativity.md#kaluza-klein-decomposition-along-a-killing-field) uses $V=h(K_X,K_X)=\alpha+\chi y^2$. Completing the square in $dx$ gives the [Heisenberg metric Kaluza-Klein reduction](../../../general-relativity.md#heisenberg-metric-kaluza-klein-reduction):

$$
\boxed{V=\alpha+\chi y^2,\qquad A=-\frac{\chi y}{\alpha+\chi y^2}\,dz,
\qquad \gamma=\beta\,dy^2+\frac{\alpha\chi}{\alpha+\chi y^2}\,dz^2.}
$$

These depend only on the quotient coordinates $(y,z)$ and satisfy $h=V(dx+A)^2+\gamma$. For a diagonal indefinite [metric tensor](../../../general-relativity.md#metric-tensor), the same expressions hold wherever $V\ne0$; a null [Killing vector field](../../../general-relativity.md#killing-vector-field) cannot be treated with this completed-square decomposition.

## 3

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [Chern number](../../../algebraic-geometry.md#chern-number) turns local curvature data into a global integer. Let $E\to M$ be a complex [vector bundle](../../../fiber-bundle.md#vector-bundle) over a compact oriented manifold without boundary, with a [unitary connection](../../../fiber-bundle.md#unitary-connection) represented locally by an anti-Hermitian matrix-valued one-form $A$. Its [curvature form of a connection](../../../fiber-bundle.md#curvature-form) is $F=dA+A\wedge A$. The [Chern-Weil theory](../../../geometry-and-topology.md#chern-weil-homomorphism) representative of the total [Chern class](../../../algebraic-geometry.md#chern-class) is

$$
c(E,A)=\det\left(I+\frac{iF}{2\pi}\right)=1+c_1(E,A)+c_2(E,A)+\cdots.
$$

The coefficients are [closed differential forms](../../../differential-form.md#closed-differential-form). They represent the images of integral [Chern classes](../../../algebraic-geometry.md#chern-class) in [de Rham cohomology](../../../differential-form.md#de-rham-cohomology). On an oriented $2r$-manifold, a product $c_{i_1}\cdots c_{i_s}$ with $i_1+\cdots+i_s=r$ pairs with the [fundamental class](../../../cohomology.md#fundamental-class) to give a [Chern number](../../../algebraic-geometry.md#chern-number), an integer independent of the [unitary connection](../../../fiber-bundle.md#unitary-connection).

For example,

$$
c_1=\frac{i}{2\pi}\operatorname{Tr}F,\qquad
c_2=\frac1{8\pi^2}\left\{\operatorname{Tr}(F\wedge F)-\operatorname{Tr}F\wedge\operatorname{Tr}F\right\}.
$$

For an $SU(N)$ bundle with $N\geq2$, $\operatorname{Tr}F=0$. On an oriented four-manifold the [Second Chern number](../../../geometry-and-topology.md#second-chern-number) is then

$$
\boxed{q=\int_M c_2=\frac1{8\pi^2}\int_M\operatorname{Tr}(F\wedge F)\in\mathbb Z,}
$$

using the fundamental [matrix trace](../../../linear-algebra.md#matrix-trace) and the stated anti-Hermitian convention. The trace-product correction is required for a general $U(N)$ bundle; it cannot simply be omitted. The sign of a physical [instanton number](../../../classical-field-theory-soliton.md#instanton-number) also depends on the trace and [orientation](../../../algebraic-topology.md#orientation-of-a-simplex) convention, so these conventions must accompany the formula.

The local origin of closure is the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity) $D_AF=0$ and the cyclic [matrix trace](../../../linear-algebra.md#matrix-trace): $d\operatorname{Tr}(F\wedge F)=0$. Independence of the [connection one-form](../../../fiber-bundle.md#connection-one-form) follows more concretely by varying a family $A_t$. Since $\dot F_t=D_{A_t}\dot A_t$, the [Chern-Weil connection transgression](../../../geometry-and-topology.md#chern-weil-connection-transgression) is

$$
\frac{d}{dt}\operatorname{Tr}(F_t\wedge F_t)=2\,d\operatorname{Tr}(\dot A_t\wedge F_t).
$$

Its integral on a closed four-manifold is zero by the [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem). This proves connection independence of $q$; the integrality is the global [Chern class](../../../algebraic-geometry.md#chern-class) statement, not merely a consequence of the local formula.

The local primitive of the [Second Chern form](../../../geometry-and-topology.md#second-chern-form) is the [Chern-Simons three-form](../../../geometry-and-topology.md#chern-simons-3-form)

$$
\boxed{Y(A)=\frac1{8\pi^2}\operatorname{Tr}\left(A\wedge dA+\frac23A\wedge A\wedge A\right),\qquad dY=c_2.}
$$

Here we continue to use $SU(N)$, so $c_2=\operatorname{Tr}(F\wedge F)/(8\pi^2)$. The cubic coefficient is forced by the [exterior derivative](../../../differential-form.md#exterior-derivative). In the graded cyclic [matrix trace](../../../linear-algebra.md#matrix-trace), $d\operatorname{Tr}(A^3)=3\operatorname{Tr}(dA\wedge A^2)$ and $\operatorname{Tr}(A^4)=0$, the latter because cycling one degree-one factor past the other three changes its sign. Therefore

$$
d\operatorname{Tr}(A\wedge dA+\tfrac23A^3)
=\operatorname{Tr}(dA\wedge dA+2dA\wedge A^2)
=\operatorname{Tr}(F\wedge F).
$$

Matrix-valued [differential forms](../../../differential-form.md) require both matrix order and the graded signs; treating all factors as commuting scalars would lose this derivation.

The [Chern-Simons three-form](../../../geometry-and-topology.md#chern-simons-3-form) depends on a local trivialization and is not itself gauge-invariant. For the [Yang-Mills gauge transformation](../../../relativistic-quantum-field.md#yang-mills-gauge-transformation) convention $A^g=g^{-1}Ag+g^{-1}dg$, set $u=g^{-1}dg$. The [gauge change of the Chern-Simons three-form](../../../geometry-and-topology.md#gauge-change-of-the-chern-simons-three-form) is

$$
Y(A^g)=Y(A)-\frac1{8\pi^2}d\operatorname{Tr}(dg\,g^{-1}\wedge A)
-\frac1{24\pi^2}\operatorname{Tr}(u\wedge u\wedge u).
$$

The last term is closed by the [Maurer-Cartan equation](../../../lie-theory.md#maurer-cartan-equation). On a closed three-manifold its integral is an integer with the fundamental $SU(N)$ normalization. Consequently **the Chern-Simons integral is naturally defined modulo integers**, while its exponential $\exp(2\pi i\ell\int Y)$ is invariant under large [Yang-Mills gauge transformations](../../../relativistic-quantum-field.md#yang-mills-gauge-transformation) for integer level $\ell$.

This also explains why a nonzero [Chern number](../../../algebraic-geometry.md#chern-number) is compatible with $dY=c_2$: $Y$ need not be a globally defined three-form. On $S^4$, trivialize over two hemispheres and let $A_N=A_S^g$ on their common equator $\Sigma=S^3$, oriented as the boundary of the northern hemisphere. The [Generalized Stokes theorem](../../../differential-form.md#generalized-stokes-theorem) and the gauge-change formula give

$$
q=\int_\Sigma(Y(A_N)-Y(A_S))
=-\frac1{24\pi^2}\int_\Sigma\operatorname{Tr}(g^{-1}dg)^3.
$$

For $SU(2)\cong S^3$, this is the degree of the transition map, with compatible group [orientation](../../../algebraic-topology.md#orientation-of-a-simplex); for $SU(N)$ it is the corresponding integer in $\pi_3(SU(N))$. Thus the [Second Chern number](../../../geometry-and-topology.md#second-chern-number) measures the obstruction to choosing one trivialization over the whole four-sphere.

A simpler [First Chern class](../../../complex-geometry.md#first-chern-class) example is a line bundle over $S^2$. Write $A=-ia$ and choose local real potentials

$$
a_N=\frac{k}{2}(1-\cos\theta)d\phi,\qquad
a_S=-\frac{k}{2}(1+\cos\theta)d\phi.
$$

They have common curvature $da=(k/2)\sin\theta\,d\theta\wedge d\phi$, so $\int_{S^2}c_1=(2\pi)^{-1}\int da=k$. Their difference $a_N-a_S=k\,d\phi$ corresponds to the transition function $e^{-ik\phi}$, which is single-valued exactly when $k\in\mathbb Z$. This illustrates how the global integer arises from patching, rather than from an arbitrary flux normalization.

In physics, these constructions distinguish topological sectors of [Yang-Mills instantons](../../../classical-field-theory-soliton.md#yang-mills-instanton) and relate four-dimensional characteristic densities to three-dimensional boundary actions. The [Chern-Simons three-form](../../../geometry-and-topology.md#chern-simons-3-form) itself gives a metric-independent gauge action in three dimensions. On a closed manifold its first variation is

$$
\delta\int Y=\frac1{4\pi^2}\int\operatorname{Tr}(\delta A\wedge F),
$$

so its classical equation is **$F=0$**. The common thread is that a local expression in the [connection one-form](../../../fiber-bundle.md#connection-one-form) records global topology: curvature produces the invariant [Chern number](../../../algebraic-geometry.md#chern-number), while its local [Chern-Simons three-form](../../../geometry-and-topology.md#chern-simons-3-form) primitive retains gauge and boundary information.

## 4

↑ **Parent:** [Paper 51](paper-51.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write $w=x^1+ix^2$, $z=x^3+ix^4$. The [Euclidean metric](../../../differential-geometry.md#euclidean-metric) is $\sum_a(dx^a)^2$, and the printed four-form is $4\,dx^1\wedge dx^2\wedge dx^3\wedge dx^4$, so it specifies the usual positive [orientation](../../../algebraic-topology.md#orientation-of-a-simplex). The normalized metric [volume form](../../../differential-form.md#volume-form) is one quarter of that expression. The [self-dual frame in complex Euclidean coordinates](../../../differential-form.md#self-dual-frame-in-complex-euclidean-coordinates) is

$$
\begin{aligned}
\omega_1&=dx^1\wedge dx^3-dx^2\wedge dx^4,\\
\omega_2&=dx^1\wedge dx^4+dx^2\wedge dx^3,\\
\omega_3&=2(dx^1\wedge dx^2+dx^3\wedge dx^4).
\end{aligned}
$$

These are real and have the required complex combinations. For the [Hodge star operator](../../../differential-form.md#hodge-star-operator) with this [orientation](../../../algebraic-topology.md#orientation-of-a-simplex),

$$
*(dx^1\wedge dx^2)=dx^3\wedge dx^4,\qquad
*(dx^1\wedge dx^3)=-dx^2\wedge dx^4,\qquad
*(dx^1\wedge dx^4)=dx^2\wedge dx^3,
$$

and applying $*$ again gives the reverse relations. Thus $*\omega_i=\omega_i$. They are linearly independent, while the $+1$ eigenspace of $*$ on [2-forms](../../../differential-form.md#2-form) has dimension three, proving **they span $\Lambda^2_+$**. The TeX aid incorrectly reads the subscript as $1$.

The [ASDYM equations](../../../classical-field-theory-soliton.md#anti-self-dual-yang-mills-equations) require the self-dual projection of the [gauge field strength](../../../relativistic-quantum-field.md#gauge-field-strength) to vanish. Orthogonality to $\omega_1,\omega_2$ sets its $(2,0)$ and $(0,2)$ parts to zero; orthogonality to $\omega_3$ removes the trace of its $(1,1)$ part. Explicitly, if $F=\sum_{a<b}f_{ab}\,dx^a\wedge dx^b$, these conditions are $f_{13}-f_{24}=0$, $f_{14}+f_{23}=0$ and $f_{12}+f_{34}=0$. Since

$$
F_{wz}=\tfrac14\{f_{13}-f_{24}-i(f_{14}+f_{23})\},\qquad
F_{w\bar w}+F_{z\bar z}=\tfrac i2(f_{12}+f_{34}),
$$

and the conjugate equation supplies the other complex component for a real [curvature form of a connection](../../../fiber-bundle.md#curvature-form), the equivalent system is

$$
\boxed{F_{wz}=0,\qquad F_{w\bar w}+F_{z\bar z}=0,\qquad F_{\bar w\bar z}=0.}
$$

To obtain the [complex potential reduction of anti-self-dual Yang-Mills](../../../classical-field-theory-soliton.md#complex-potential-reduction-of-anti-self-dual-yang-mills), set $D_w=\partial_w+A_w$, $D_z=\partial_z+A_z$. The first equation is the integrability condition $[D_w,D_z]=0$. Locally it allows an invertible complex matrix $s$ satisfying $\partial_ws=-A_ws$ and $\partial_zs=-A_zs$. The [Yang-Mills gauge transformation](../../../relativistic-quantum-field.md#yang-mills-gauge-transformation) $A\mapsto s^{-1}As+s^{-1}ds$ consequently gives $A_w=A_z=0$. This is a complex gauge; a real compact [gauge group](../../../relativistic-quantum-field.md#gauge-group) alone generally cannot implement it.

In this gauge the second equation becomes

$$
\partial_wA_{\bar w}+\partial_zA_{\bar z}=0.
$$

Thus the one-form $A_{\bar w}\,dz-A_{\bar z}\,dw$ is closed with respect to the exterior derivative in the $(w,z)$ directions. The local complex version of the [Poincaré lemma](../../../differential-form.md#poincare-lemma) gives a potential $K$ such that

$$
\boxed{A_w=A_z=0,\qquad A_{\bar w}=\partial_zK,\qquad A_{\bar z}=-\partial_wK.}
$$

Because the gauge transformation is complex, $K$ is generally valued in the [complexification of a Lie algebra](../../../lie-algebra.md#complexification-of-a-lie-algebra) $\mathfrak g_{\mathbb C}$; the printed $\mathfrak g$ must be understood in that sense. The elementary reduction is local, and the transformed fields retain a reality condition inherited from the original real connection. For the usual compact matrix gauge groups and smooth fields on all of $\mathbb R^4=\mathbb C^2$, the gauge and potential can also be chosen globally if no condition at infinity is imposed. The flat partial connection defines a holomorphic [principal bundle](../../../fiber-bundle.md#principal-bundle) on the conjugate complex space. That base is a contractible [Stein manifold](../../../complex-geometry.md#stein-manifold), so the [Oka-Grauert principle](../../../complex-geometry.md#oka-grauert-principle) gives a global trivialization and hence a global complex gauge. After that trivialization, the conjugate of [Stein vanishing for the Dolbeault cohomology of functions](../../../complex-geometry.md#stein-vanishing-for-the-dolbeault-cohomology-of-functions) gives a global primitive $K$, component by component in $\mathfrak g_{\mathbb C}$. Prescribed framing or decay at infinity requires a separate compatibility check and is not automatically preserved by this gauge.

Substitute the potential into the remaining [ASDYM equations](../../../classical-field-theory-soliton.md#anti-self-dual-yang-mills-equations) component:

$$
\begin{aligned}
F_{\bar w\bar z}
&=\partial_{\bar w}(-K_w)-\partial_{\bar z}K_z+[K_z,-K_w]\\
&=-K_{w\bar w}-K_{z\bar z}+[K_w,K_z].
\end{aligned}
$$

Therefore all three [ASDYM equations](../../../classical-field-theory-soliton.md#anti-self-dual-yang-mills-equations) reduce to the single [ASDYM potential equation](../../../classical-field-theory-soliton.md#complex-potential-reduction-of-anti-self-dual-yang-mills)

$$
\boxed{K_{w\bar w}+K_{z\bar z}-[K_w,K_z]=0.}
$$

The sign follows directly from $A_{\bar z}=-K_w$; changing a potential convention would change the displayed commutator sign. Conversely, this equation and the displayed gauge reconstruction make all three curvature conditions vanish, subject to the inherited reality condition when a real [gauge field](../../../relativistic-quantum-field.md#gauge-field) is required.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
