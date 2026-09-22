# Paper 22

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper22.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper22.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Choose a [complex projective line](../../../algebraic-topology.md#complex-projective-line) in each [Complex projective plane](../../../algebraic-topology.md#complex-projective-plane) summand. Make the [connected sum](../../../differential-geometry.md#connected-sum-of-oriented-manifolds) at small disks on these lines, so the lines themselves join through the neck to form a smoothly embedded sphere $S\cong S^2$. Its class is the sum $h_1+h_2$ of the two line classes. The [intersection form](../../../homology.md#intersection-form) is diagonal with entries one, hence

$$
[S]^2=(h_1+h_2)^2=2.
$$

The oriented [normal bundle](../../../algebraic-geometry.md#normal-bundle) of $S$ is a rank-two real bundle with [Euler number](../../../fiber-bundle.md#euler-number-of-a-vector-bundle) two, because its Euler number equals the [self-intersection number](../../../algebraic-geometry.md#self-intersection-number). Oriented plane bundles over $S^2$ are classified by that integer, so this normal bundle is isomorphic to $TS^2$. The boundary of a closed [tubular neighborhood](../../../differential-geometry.md#tubular-neighborhood) $N$ is consequently the [unit tangent bundle](../../../fiber-bundle.md#unit-tangent-bundle) of $S^2$.

A unit tangent pair $(x,v)$ determines the oriented orthonormal frame $(x,v,x\times v)$ in $\mathbb R^3$. Thus $UTS^2\cong SO(3)\cong\mathbb{RP}^3$, the latter identification coming from the double covering by [unit quaternions](../../../algebra.md#unit-quaternion). Therefore **$\partial N$ is the required smoothly embedded $\mathbb{RP}^3$**. Its complement is disconnected: the nonempty interior of $N$ and the nonempty exterior $X\setminus N$ are disjoint open subsets of $X\setminus\partial N$ that exhaust it. The neighborhood can be chosen small enough that its exterior is nonempty. This is the construction of [separating projective three-space in a positive connected sum](../../../differential-geometry.md#separating-projective-three-space-in-a-positive-connected-sum).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In the [cohomology](../../../cohomology.md) basis $h_1,\ldots,h_n$ supplied by the projective lines in the summands, the [intersection form](../../../homology.md#intersection-form) is

$$
Q_X(h_i,h_j)=\delta_{ij}.
$$

For each [permutation](../../../combinatorics.md#permutation) $\sigma\in S_n$, the linear map $h_i\mapsto h_{\sigma(i)}$ preserves this pairing. Distinct permutations induce distinct maps, and their compositions agree with permutation composition. Hence **the permutation matrices give a subgroup $G\cong S_n$ of the isometry group of $Q_X$**.

To realize these isometries smoothly, describe $X$ as a punctured $S^4$ with $n$ punctured copies of $\mathbb{CP}^2$ attached to its boundary spheres. An orientation-preserving ambient isotopy of $S^4$ can interchange any two chosen disjoint attachment balls while carrying their parametrizations along with them: move their centers along disjoint arcs and extend the motion to small balls. There is room to make these arcs disjoint in dimension four. Extend the endpoint diffeomorphism across the two exchanged punctured copies using the chosen identifications of those identical oriented summands; use the identity on the remaining copies. Collar coordinates make the maps fit smoothly along the gluing spheres. This exchanges the two line classes without changing their signs. Since transpositions generate $S_n$, composing these [diffeomorphisms](../../../geometry-and-topology.md#diffeomorphism) realizes each element of $G$. Pullback permutes the [cohomology](../../../cohomology.md) basis by the inverse permutation, which still realizes the same subgroup and all its elements. These are [permutation diffeomorphisms of identical connected summands](../../../differential-geometry.md#permutation-diffeomorphisms-of-identical-connected-summands).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let $f:S^2\times S^2\to\mathbb{CP}^2\#\mathbb{CP}^2$ have [mapping degree](../../../homology.md#degree-of-a-continuous-mapping) $d$. Naturality of the [cup product](../../../cohomology.md#cup-product) and evaluation on the fundamental class imply

$$
Q_{S^2\times S^2}(f^*u,f^*v)=d\,Q_{\mathbb{CP}^2\#\mathbb{CP}^2}(u,v).
$$

The two factor classes give the source matrix $H=\begin{pmatrix}0&1\\1&0\end{pmatrix}$, while the target matrix is $I_2$. If $P$ is the integral matrix for the pullback in these bases, then

$$
P^{\mathsf T}HP=dI_2.
$$

Taking determinants gives $-(\det P)^2=d^2$, whose left side is nonpositive and whose right side is nonnegative. Thus $d=0$. **There is no map of nonzero degree**, including negative degree. This [degree constraint from intersection forms](../../../homology.md#degree-constraint-from-intersection-forms) is a cohomological argument and does not assume that $f$ is smooth.

## 2

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use the convention $\nabla=d+A$ with anti-Hermitian [connection one-forms](../../../fiber-bundle.md#connection-one-form). For a unitary [complex line bundle](../../../fiber-bundle.md#complex-line-bundle), $A$ is locally an $i\mathbb R$-valued one-form and $F_\nabla=dA$, since the Lie algebra is abelian. Under a change of unitary frame, the [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) transforms by conjugation, which is trivial for $U(1)$. Hence $F_\nabla$ is a globally defined imaginary-valued two-form, and **$iF_\nabla$ is an ordinary real two-form**. Equivalently, $\operatorname{End}(L)$ has its canonical scalar trivialization, so no nontrivial coefficient bundle remains.

Locally $dF_\nabla=d^2A=0$, and these equalities patch globally. If another [unitary connection](../../../fiber-bundle.md#unitary-connection) is $\nabla'=\nabla+i\beta$ for a global real one-form $\beta$, then

$$
F_{\nabla'}=F_\nabla+i\,d\beta,\qquad
\boxed{iF_{\nabla'}=iF_\nabla-d\beta.}
$$

Thus the real [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) is closed and its [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) class is independent of the [unitary connection](../../../fiber-bundle.md#unitary-connection).

With the [First Chern class](../../../complex-geometry.md#first-chern-class) normalization $c_1(L)_{\mathbb R}=[iF_\nabla/(2\pi)]$, the transverse section also identifies this class as $\operatorname{PD}[\Sigma]$. Indeed, the complex orientation of each normal disk makes the section wind positively once around a transverse zero. The [Euler class](../../../fiber-bundle.md#euler-class-of-a-vector-bundle) of the underlying oriented plane bundle counts these zeros with their induced orientation, and equals $c_1(L)$. This records the role of the section and orientation hypotheses; connection independence itself did not require choosing a section.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Start with any [unitary connection](../../../fiber-bundle.md#unitary-connection) $\nabla_0$. The [Hodge decomposition theorem](../../../differential-form.md#hodge-decomposition-theorem) gives a unique real [harmonic differential form](../../../differential-form.md#harmonic-differential-form) $\eta$ representing $[iF_{\nabla_0}]$. Since they have the same [de Rham cohomology](../../../differential-form.md#de-rham-cohomology) class, $\eta-iF_{\nabla_0}=d\beta$ for a smooth real one-form $\beta$. Set $\nabla=\nabla_0-i\beta$. The [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) difference formula gives

$$
\boxed{iF_\nabla=iF_{\nabla_0}+d\beta=\eta.}
$$

This proves existence of a [harmonic-curvature unitary line connection](../../../fiber-bundle.md#harmonic-curvature-unitary-line-connection) for any metric and any [complex line bundle](../../../fiber-bundle.md#complex-line-bundle).

Two such [unitary connections](../../../fiber-bundle.md#unitary-connection) have the same [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) because harmonic representatives are unique. Their difference is therefore $i\gamma$ with $d\gamma=0$. When $b_1(X)=0$, write $\gamma=d\varphi$ globally. The [bundle gauge transformation](../../../fiber-bundle.md#unitary-bundle-gauge-transformation) $u=e^{i\varphi}$ changes $\nabla$ to $u^{-1}\nabla u=\nabla+i\,d\varphi$. Thus **the harmonic-curvature connection is unique up to gauge**. On a general base, closed forms modulo the integral-period forms coming from circle-valued gauge transformations leave the torus $H^1(X;\mathbb R)/(2\pi H^1(X;\mathbb Z))$ of possible gauge classes; the hypothesis removes this freedom.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The reverse-oriented [Complex projective plane](../../../algebraic-topology.md#complex-projective-plane) has [intersection form](../../../homology.md#intersection-form) $(-1)$, so $b^+=0$, while $b_1=0$. The [Hodge star](../../../differential-form.md#hodge-star-operator) splits harmonic two-forms into self-dual and anti-self-dual subspaces, and their dimensions are the positive and negative indices of the [intersection form](../../../homology.md#intersection-form). Therefore every harmonic two-form is an [anti-self-dual two-form](../../../differential-form.md#anti-self-dual-differential-form) for every chosen metric.

By part (b), every [complex line bundle](../../../fiber-bundle.md#complex-line-bundle) has a [unitary connection](../../../fiber-bundle.md#unitary-connection) with harmonic real [vector-bundle curvature](../../../fiber-bundle.md#curvature-form), so this connection is an [ASD connection](../../../fiber-bundle.md#anti-self-dual-connection). Conversely, an [ASD connection](../../../fiber-bundle.md#anti-self-dual-connection) on a [complex line bundle](../../../fiber-bundle.md#complex-line-bundle) has $dF=0$ and $d*F=-dF=0$, so its [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) is harmonic. The uniqueness in part (b) therefore applies to all [ASD connections](../../../fiber-bundle.md#anti-self-dual-connection) on that fixed [complex line bundle](../../../fiber-bundle.md#complex-line-bundle). **Each [complex line bundle](../../../fiber-bundle.md#complex-line-bundle) has exactly one gauge orbit of ASD connections.**

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $a,b\in H^2(S^2\times S^2;\mathbb Z)$ be the two factor classes, normalized by $a^2=b^2=0$ and $\langle ab,[X]\rangle=1$. Choose the [complex line bundle](../../../fiber-bundle.md#complex-line-bundle) $L$ with $c_1(L)=a+b$, for example the tensor product of pullbacks of degree-one [complex line bundles](../../../fiber-bundle.md#complex-line-bundle) from the two factors. Then

$$
c_1(L)^2[X]=2.
$$

If $L$ had an [ASD connection](../../../fiber-bundle.md#anti-self-dual-connection), the real closed form $\alpha=iF/(2\pi)$ would represent this class and satisfy $*\alpha=-\alpha$. Hence

$$
2=\int_X\alpha\wedge\alpha=-\int_X|\alpha|^2\,d\mathrm{vol}_g\leq0,
$$

a contradiction. **This [complex line bundle](../../../fiber-bundle.md#complex-line-bundle) admits no ASD connection for any metric of the given product orientation.** For the reverse product orientation, take $c_1(L)=a-b$ instead, which then has square $+2$. This is the [positive-square obstruction to ASD line connections](../../../fiber-bundle.md#positive-square-obstruction-to-asd-line-connections).

The suggested rank-two construction gives the same obstruction. The split bundle $E=L\oplus L^*$ has trivial determinant and

$$
c(E)=(1+c_1(L))(1-c_1(L)),\qquad c_2(E)[X]=-c_1(L)^2[X]=-2.
$$

An [ASD connection](../../../fiber-bundle.md#anti-self-dual-connection) on $L$ would induce an [ASD connection](../../../fiber-bundle.md#anti-self-dual-connection) on $E$, but its [instanton number](../../../classical-field-theory-soliton.md#instanton-number) would be $\|F_E\|_2^2/(8\pi^2)\geq0$, contradicting $c_2(E)[X]=-2$.

## 3

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Write the [flat connection](../../../relativistic-quantum-field.md#flat-connection) as $d+A_x\,dx+A_y\,dy$ in a global unitary frame. Solve the matrix ordinary differential equation

$$
\partial_x u(x,y)=-A_x(x,y)u(x,y),\qquad u(0,y)=I.
$$

Smooth dependence on parameters gives a smooth solution on the entire open square. Since $A_x$ is skew-Hermitian and trace free, differentiating $u^*u$ and $\det u$ shows that $u(x,y)\in SU(2)$. Under the [bundle gauge transformation](../../../fiber-bundle.md#unitary-bundle-gauge-transformation) $u$, the transformed connection has

$$
A'_x=u^{-1}A_xu+u^{-1}\partial_xu=0.
$$

Its [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) is still zero. The remaining [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) equation is $\partial_xA'_y=0$, so $A'_y=B(y)$ is independent of $x$. Now solve $v'(y)=-B(y)v(y)$ with $v(0)=I$. Again $v\in SU(2)$; this second [bundle gauge transformation](../../../fiber-bundle.md#unitary-bundle-gauge-transformation), independent of $x$, leaves $A'_x=0$ and makes $A''_y=0$. Thus **the original connection is gauge equivalent to the trivial connection**. Both transformations exist on the whole square, not just in a small coordinate neighborhood.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For a connected base with a chosen frame at a base point, [flat connections](../../../relativistic-quantum-field.md#flat-connection) modulo the [based unitary gauge group](../../../fiber-bundle.md#based-unitary-gauge-group) correspond to [flat holonomy representations](../../../relativistic-quantum-field.md#holonomy-representation-of-a-flat-connection) $\pi_1(X,x)\to G$. Removing the frame, or allowing the full [unitary bundle gauge group](../../../fiber-bundle.md#unitary-bundle-gauge-group), also divides by conjugation in $G$. On a prescribed underlying bundle, retain only those representations whose associated flat bundle has that bundle type.

The correspondence can be seen directly. Zero [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) makes [parallel transport](../../../fiber-bundle.md#parallel-transport) invariant under homotopies of paths with fixed endpoints, giving a [group homomorphism](../../../group-theory.md#group-homomorphism) on loops. Conversely, a representation $\rho$ gives the flat bundle $(\widetilde X\times G)/\pi_1(X)$, with the deck action on the first factor and $\rho$ on the second, and the product horizontal distribution descends. If two framed connections have identical holonomies, compare their parallel transports along a path from the base point to each point. The comparison is path independent and defines a [bundle gauge transformation](../../../fiber-bundle.md#unitary-bundle-gauge-transformation) equal to the identity at the base point. These constructions are inverse. This is [framed flat connections and holonomy](../../../relativistic-quantum-field.md#framed-flat-connections-and-holonomy).

The punctured torus retracts onto a wedge of two circles, so its [fundamental group](../../../algebraic-topology.md#fundamental-group) is the [free group](../../../geometric-group-theory.md#free-group) $F_2$. A representation into $SU(2)$ is specified freely by the two generator images $(A,B)$, with no relation. Every resulting principal $SU(2)$ bundle is trivial, since a bundle with connected structure group over a graph is trivial. Thus no representation is excluded by the fixed trivial-bundle condition. Holonomy depends continuously on a connection, and the flat-bundle construction gives locally continuous choices of representatives as the two matrices vary; local choices of paths in $SU(2)$ give this continuity without requiring a global logarithm. Consequently

$$
\boxed{\widetilde M(T)\cong\operatorname{Hom}(F_2,SU(2))=SU(2)^2\cong S^3\times S^3.}
$$

The last identification is the description of $SU(2)$ by [unit quaternions](../../../algebra.md#unit-quaternion). The unbased quotient used next is simultaneous conjugation, not independent conjugation of the two generator images.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

By part (b), the [moduli space](../../../geometry-and-topology.md#moduli-space) is $M(T)=SU(2)^2/SU(2)$ under simultaneous conjugation. Regard $SU(2)$ as the [unit quaternions](../../../algebra.md#unit-quaternion) and write

$$
A=a+u,\qquad B=b+v,\qquad
|u|^2=1-a^2,\quad |v|^2=1-b^2,
$$

with $u,v\in\mathbb R^3$. Conjugation rotates both imaginary vectors by the same element of $SO(3)$. Their lengths and inner product determine an orbit, even when one vector vanishes or the vectors are collinear: an isometry between the two spanned planes can be extended to an orientation-preserving rotation of $\mathbb R^3$. Thus complete invariants are

$$
(a,b,c),\qquad c=u\cdot v,\qquad
-1\leq a,b\leq1,\quad c^2\leq(1-a^2)(1-b^2).
$$

Every allowed triple is realized by a pair of vectors with the prescribed lengths and dot product. The induced continuous bijection from the compact quotient to this closed subset of $\mathbb R^3$ is a [homeomorphism](../../../topology.md#homeomorphism).

Let $U$ be the subset where $A\ne\pm1$, equivalently $-1<a<1$. It is open and dense because the excluded first holonomies can be approximated by noncentral ones. Rotate $u$ to the positive $i$ axis, so $A=a+\sqrt{1-a^2}\,i$. Its remaining stabilizer rotates the $j,k$ plane. If $B=b+t i+yj+zk$, the orbit is determined by $(b,t)$, and

$$
b^2+t^2\leq1,
$$

with the remaining radius $\sqrt{1-b^2-t^2}$. These coordinates give the corrected result

$$
\boxed{U\cong\overline{\mathbb D}\times(-1,1)
\cong\overline{\mathbb D}\times(0,1).}
$$

Continuity of the inverse follows by taking $y=\sqrt{1-b^2-t^2}$ and $z=0$ as a representative. The complement consists of $A=1$ and $A=-1$, separately. In either case conjugation classes of $B$ are parametrized by its real part $b\in[-1,1]$. Therefore **$M(T)\setminus U$ is two disjoint closed intervals**, as requested.

**The printed $S^2$ factor is incorrect: the factor must be a closed disk.** The stabilizer acts by conjugation, fixing the circle of quaternions $b+ti$; it is not the free Hopf circle action on $S^3$. To rule out a different choice of dense open set with the printed topology, we can also identify the whole space. Replace $c$ by $d=ab+c$. The invariant region becomes

$$
\mathcal C=\left\{(a,b,d):
\begin{pmatrix}1&a&b\\a&1&d\\b&d&1\end{pmatrix}\text{ is positive semidefinite}\right\}.
$$

These are the Gram matrices of the three unit vectors $1,A,B$ in $\mathbb R^4$. Conversely, a positive-semidefinite matrix of this form can be realized by such vectors, hence by the original quaternion data. The set $\mathcal C$ is compact and convex and contains the identity matrix as an interior point in its three coordinates. Radial parametrization of a convex body therefore identifies it with a closed three-ball. Thus

$$
\boxed{M(T)\cong\overline B^3.}
$$

This also agrees with Theorem 6.5 of [the primary character-variety paper](https://arxiv.org/pdf/0807.3317).

An open subset homeomorphic to the boundaryless three-manifold $S^2\times(0,1)$ cannot contain a boundary point of this closed ball. Otherwise a local chart, followed by inclusion into $\mathbb R^3$, would be a continuous injection from an open subset of $\mathbb R^3$ whose image contains a ball-boundary point while staying inside the closed ball, contradicting [invariance of domain](../../../topology.md#invariance-of-domain). Its complement would therefore contain the entire boundary sphere. But a sphere cannot embed in two disjoint intervals: its connected image would lie in one interval and be a nondegenerate compact interval, whose interior points disconnect it, unlike $S^2$. This proves that the literal printed pair of claims is impossible, and supplies the complete corrected [SU2 character variety of the punctured torus](../../../geometry-and-topology.md#su2-character-variety-of-the-punctured-torus) description.

## 4

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use anti-Hermitian $SU(2)$ [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) and the fundamental [matrix trace](../../../linear-algebra.md#matrix-trace), so

$$
k(E)=c_2(E)[X]=\frac1{8\pi^2}\int_X\operatorname{Tr}(F\wedge F)
$$

is an integer on a closed oriented four-manifold. The supplied formula's phrase “extending $W$” is a typographical error in the original PDF: the connection extends the boundary connection $\nabla$. An extension exists, for example on the trivial bundle over $B^4$, by extending a boundary connection through a collar and cutting it off farther inside.

For well-definedness, glue two choices $W_0$ and $-W_1$ along their identified boundary bundles. Connections may be made product connections on a collar while keeping their boundary values, and the transgression identity below shows that this does not alter the relevant integral. The glued bundle over the resulting closed four-manifold has an integer [Second Chern number](../../../geometry-and-topology.md#second-chern-number). Therefore the two extension integrals differ by an integer, proving **the value of $\operatorname{CS}$ is independent of all choices in $\mathbb R/\mathbb Z$**. In particular, different extensions on one fixed bundle with the same boundary value have zero difference by transgression and [Stokes theorem](../../../calculus.md#stokes-theorem).

To compute the derivative, extend the boundary variation $a$ to an adjoint-valued one-form $\widetilde a$ on $W$ and set $\widetilde\nabla_t=\widetilde\nabla+t\widetilde a$. The [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) derivative is $\dot F=d_{\widetilde\nabla}\widetilde a$. Invariance of the trace and the [Bianchi identity](../../../fiber-bundle.md#bianchi-identity) give

$$
\begin{aligned}
\left.\frac d{dt}\right|_0\operatorname{Tr}(F_t\wedge F_t)
&=2\operatorname{Tr}(d_{\widetilde\nabla}\widetilde a\wedge F)\\
&=2d\operatorname{Tr}(\widetilde a\wedge F).
\end{aligned}
$$

The second equality follows from the covariant product rule; its other term contains $d_{\widetilde\nabla}F=0$. Integrating and applying [Stokes theorem](../../../calculus.md#stokes-theorem), with the given boundary orientation, yields

$$
\boxed{\left.\frac d{dt}\right|_0\operatorname{CS}(\nabla+ta)
=\frac1{4\pi^2}\int_{S^3}\operatorname{Tr}(F_\nabla\wedge a).}
$$

This derivative means the derivative of any local real lift of the circle-valued functional; changing that lift by an integer changes no derivative.

If a [bundle gauge transformation](../../../fiber-bundle.md#unitary-bundle-gauge-transformation) $u$ extends to $\widetilde u$ on $W$, use $\widetilde u^{-1}\widetilde\nabla\widetilde u$ as the extension of the transformed boundary connection. [Vector-bundle curvature](../../../fiber-bundle.md#curvature-form) is conjugated, so its trace square is unchanged pointwise. **$\operatorname{CS}(u\cdot\nabla)=\operatorname{CS}(\nabla)$.** This proof even preserves the chosen extension's real integral, before reducing modulo integers. The local [Chern-Simons three-form](../../../geometry-and-topology.md#chern-simons-3-form) transgresses the same characteristic form and is the boundary expression used in the compactness argument below.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $k=e(E)=c_2(E)[X]=1$, where the underlying oriented real rank-four bundle has its complex orientation. The charge-one [Uhlenbeck-Donaldson compactness for charge-one ASD connections](../../../fiber-bundle.md#uhlenbeck-donaldson-compactness-for-charge-one-asd-connections) assertion is that any sequence of [ASD connections](../../../fiber-bundle.md#anti-self-dual-connection) $A_n$ has a subsequence with one of these alternatives: modulo [bundle gauge transformations](../../../fiber-bundle.md#unitary-bundle-gauge-transformation), it converges smoothly on all of $X$ to an [ASD connection](../../../fiber-bundle.md#anti-self-dual-connection) of charge one; or it converges smoothly on compact subsets of $X\setminus\{x\}$ to a connection that extends smoothly on a charge-zero bundle and is flat, with

$$
\boxed{|F_{A_n}|^2\,d\mathrm{vol}_g\ \rightharpoonup\ 8\pi^2\delta_x.}
$$

Bundle identifications are made on the complement of the bubble point in the second alternative. In general the flat limit can have nontrivial holonomy; trivial charge does not imply trivial connection on an arbitrary base. The closure of the charge-one moduli space in the ideal-instanton topology adds only a subset of $M_0\times X$, and is compact. Here $M_0$ denotes flat gauge classes on charge-zero bundles.

The local analytic inputs are the following, stated so that the compactness conclusion is not itself assumed. A [Uhlenbeck small-energy Coulomb gauge](../../../fiber-bundle.md#uhlenbeck-small-energy-coulomb-gauge) on a four-ball exists whenever $\int_B|F_A|^2$ is below a universal local threshold; it obeys $d^*a=0$, the usual normal boundary condition, and $\|a\|_{W^{1,2}}\leq C\|F_A\|_2$ after rescaling. For [ASD connections](../../../fiber-bundle.md#anti-self-dual-connection), the local small-energy regularity estimates bound every [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) derivative on a smaller ball:

$$
\sup_{B_{r/2}}|\nabla_A^mF_A|
\leq C_m r^{-2-m}\|F_A\|_{L^2(B_r)}.
$$

Together with [elliptic regularity](../../../distribution-theory.md#elliptic-regularity) in the Coulomb gauge, these give bounds on all derivatives of local [connection matrices](../../../fiber-bundle.md#connection-one-form) on smaller balls. Smooth fixed metrics permit these estimates on sufficiently small coordinate balls. Finally, the [Uhlenbeck removable singularity theorem for ASD connections](../../../fiber-bundle.md#uhlenbeck-removable-singularity-theorem-for-asd-connections) states that a smooth finite-energy [ASD connection](../../../fiber-bundle.md#anti-self-dual-connection) on a punctured four-ball extends smoothly after a gauge change and bundle extension. Rellich compactness and elliptic bootstrapping are used in passing from bounded local representatives to smooth subsequential limits. These are local estimates and an extension theorem, not the global bubbling theorem being proved.

For the proof, put the inner product $\langle U,V\rangle=-\operatorname{Tr}(UV)$ on the anti-Hermitian Lie algebra. Since $*F_A=-F_A$,

$$
\operatorname{Tr}(F_A\wedge F_A)
=-\operatorname{Tr}(F_A\wedge*F_A)=|F_A|^2\,d\mathrm{vol}_g.
$$

Thus every $A_n$ has energy $8\pi^2$. Pass to a weakly convergent subsequence of the nonnegative curvature-energy measures. Let $S$ be the points at which the limit measure has an atom at least the small-energy threshold. There are finitely many, because the total mass is fixed.

At every point outside $S$, a sufficiently small ball has limit mass less than the threshold; choose its boundary to have zero limit mass. The corresponding energies for all large $n$ are then below the threshold. The local Coulomb gauges and the stated estimates yield smooth subsequential convergence on smaller balls. A countable cover and diagonal extraction give these limits everywhere outside $S$. On overlaps, the transition gauges satisfy the first-order equation relating the two [connection matrices](../../../fiber-bundle.md#connection-one-form). Their derivatives are bounded by the already controlled matrices, and the compactness of $SU(2)$ controls their zeroth-order values. Extracting limits of these transitions patches the local limits into a smooth bundle and [ASD connection](../../../fiber-bundle.md#anti-self-dual-connection) $A_\infty$ on $X\setminus S$. On a fixed compact subset, close transition cocycles identify the original and limiting bundles by smooth near-identity isomorphisms; one can construct these by embedding the bundles into one trivial Hermitian bundle and using the polar decomposition of the nearby orthogonal projections. This yields actual bundle identifications for the convergent connections, not merely separate local limits.

The limiting [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) has finite energy by lower semicontinuity. Apply the removable-singularity input at each point of $S$. We obtain a smooth extended bundle $E_\infty$ and [ASD connection](../../../fiber-bundle.md#anti-self-dual-connection) on all of $X$. Strong convergence away from $S$ shows that the remaining measure is a nonnegative sum of atoms:

$$
|F_{A_n}|^2d\mathrm{vol}_g\ \rightharpoonup\
|F_{A_\infty}|^2d\mathrm{vol}_g+\sum_{p\in S}\beta_p\delta_p,
\qquad \beta_p>0.
$$

Discard any artificial zero-defect points if they occur in a preliminary choice of exceptional set.

Here is the topological argument that makes the defects integral, rather than merely small positive real numbers. Around one point $p$, choose a ball $B$ whose boundary contains no exceptional point. Both the original and the extended limiting bundles are trivial over $B$, but their gauges identifying the boundary can differ by a map $S^3\to SU(2)$. The [Second Chern number](../../../geometry-and-topology.md#second-chern-number) of the clutching bundle obtained by gluing two copies of $B$ is an integer. Using the [Chern-Simons three-form](../../../geometry-and-topology.md#chern-simons-3-form) on the boundary gives

$$
\frac1{8\pi^2}\left(\int_B\operatorname{Tr}(F_{A_n}\wedge F_{A_n})
-\int_B\operatorname{Tr}(F_{A_\infty}\wedge F_{A_\infty})\right)
=N_n+o(1),\qquad N_n\in\mathbb Z.
$$

The $o(1)$ term is the difference of the boundary Chern-Simons integrals in the convergent gauges, hence tends to zero by smooth boundary convergence. The integer is the clutching contribution. The left side tends to $\beta_p/(8\pi^2)$, so the closedness of $\mathbb Z$ gives $\beta_p=8\pi^2m_p$ for an integer $m_p\geq1$.

Taking total masses now gives

$$
\boxed{1=k(E_\infty)+\sum_{p\in S}m_p},\qquad
k(E_\infty)=\frac{\|F_{A_\infty}\|_2^2}{8\pi^2}\in\mathbb Z_{\geq0}.
$$

There are only two possibilities. If the sum is zero, there is no concentration; the same local gauges cover all of $X$, giving smooth gauge convergence on the original bundle. If the sum is nonzero, it consists of one integer one, and $k(E_\infty)=0$. The limiting [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) therefore vanishes, and all energy is the single atom $8\pi^2\delta_x$. This proves the alternatives.

Finally, flat gauge classes on a compact base form a compact space: choose finitely many generators of its [fundamental group](../../../algebraic-topology.md#fundamental-group), identify flat classes with the closed representation subset of a finite product of $SU(2)$ subject to its relations, and quotient by the compact conjugation action. All flat $SU(2)$ bundles here have zero second Chern class and the corresponding charge-zero topological type. Thus the ideal stratum $M_0\times X$ is compact. Combining its subsequential compactness with the two alternatives proves compactness of the closure in the ideal-instanton topology. No gluing theorem asserting that every formal ideal point is realized is needed for this compactness statement.

## 5

↑ **Parent:** [Paper 22](paper-22.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For the adjoint real bundle $\operatorname{ad}E$, the [ASD deformation complex](../../../fiber-bundle.md#asd-deformation-complex) is

$$
\boxed{0\longrightarrow\Omega^0(\operatorname{ad}E)
\xrightarrow{\ d_A\ }\Omega^1(\operatorname{ad}E)
\xrightarrow{\ d_A^+\ }\Omega^{2,+}(\operatorname{ad}E)
\longrightarrow0,}
$$

where $d_A^+=P_+d_A$ and $P_+=(1+*)/2$. On an adjoint section $\xi$, the [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) identity gives $d_A^2\xi=[F_A,\xi]$. Since $P_+$ acts only on the two-form part and $F_A^+=0$,

$$
d_A^+d_A\xi=P_+[F_A,\xi]=[F_A^+,\xi]=0.
$$

This proves it is a complex. Its three [cohomology](../../../cohomology.md) spaces are the infinitesimal stabilizers $H_A^0$, infinitesimal deformations modulo gauge $H_A^1$, and obstructions $H_A^2$.

The associated gauge-fixed [elliptic differential operator](../../../distribution-theory.md#elliptic-differential-operator) is

$$
D_A=d_A^*\oplus d_A^+:\Omega^1(\operatorname{ad}E)
\longrightarrow\Omega^0(\operatorname{ad}E)\oplus\Omega^{2,+}(\operatorname{ad}E).
$$

The [ASD deformation index](../../../fiber-bundle.md#asd-deformation-index) formula is

$$
\begin{aligned}
\operatorname{ind}D_A
&=\dim H_A^1-\dim H_A^0-\dim H_A^2\\
&=-2\langle p_1(\operatorname{ad}E),[X]\rangle
-\frac32\bigl(\chi(X)+\sigma(X)\bigr)\\
&=8e(E)-3(1-b_1(X)+b^+(X)).
\end{aligned}
$$

Here the [Atiyah-Singer index theorem](../../../riemannian-geometry.md#atiyah-singer-index-theorem) is used for the formula, with $p_1(\operatorname{ad}E)=-4c_2(E)$ and $e(E)=c_2(E)[X]$. For the simply connected negative-definite base in this question, $b_1=b^+=0$, so **$\operatorname{ind}D_A=8e(E)-3$**. The alternating Euler characteristic of the three-term complex is the negative of this operator index; stating which index is being used avoids a sign ambiguity.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

By definition $H_A^0=\ker d_A$ consists of parallel adjoint sections. Evaluation at one point identifies it with the subspace of $\mathfrak{su}(2)$ fixed by the full [holonomy](../../../fiber-bundle.md#holonomy) group. For holonomy equal to a maximal circle, write its elements as $\operatorname{diag}(\lambda,\lambda^{-1})$. The fixed Lie algebra is

$$
\left\{\begin{pmatrix}it&0\\0&-it\end{pmatrix}:t\in\mathbb R\right\}.
$$

The off-diagonal real plane rotates with weight two and has no nonzero vector fixed by the whole circle. A parallel section is uniquely determined by its value, and every invariant value gives a globally well-defined parallel section by [parallel transport](../../../fiber-bundle.md#parallel-transport). Therefore **$\dim_{\mathbb R}H_A^0=1$**. The full-circle holonomy hypothesis is essential: central holonomy would fix all of $\mathfrak{su}(2)$.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The [Fredholm Kuranishi reduction](../../../functional-analysis.md#fredholm-kuranishi-reduction) has the following form. Let $F$ be a smooth map between real Hilbert spaces with $F(0)=0$ whose derivative $L=DF(0)$ is a [Fredholm operator](../../../functional-analysis.md#fredholm-operator). Split the source as $K\oplus V$, where $K=\ker L$, and the target as $R\oplus C$, where $R=\operatorname{im}L$ and $C$ represents the finite-dimensional cokernel. The restriction $L:V\to R$ is a bounded isomorphism. The [implicit function theorem](../../../calculus.md#implicit-function-theorem) applied to $P_RF(k+v)=0$ solves it uniquely near zero as $v=v(k)$, with $v(0)=Dv(0)=0$. Thus

$$
\kappa(k)=P_CF(k+v(k)),\qquad
\kappa:K\longrightarrow C,\qquad
\kappa(0)=D\kappa(0)=0,
$$

is a smooth finite-dimensional obstruction map, and **the local zero set of $F$ is the graph over $\kappa^{-1}(0)$**. If a compact group acts preserving the problem, average inner products to choose invariant splittings; uniqueness in the [implicit function theorem](../../../calculus.md#implicit-function-theorem) makes the construction equivariant.

Apply this to the [vector-bundle curvature](../../../fiber-bundle.md#curvature-form) equation near $A$. Complete connections in $L^2_\ell$ and the [unitary bundle gauge group](../../../fiber-bundle.md#unitary-bundle-gauge-group) in $L^2_{\ell+1}$ with integer $\ell\geq3$, so the required multiplication and gauge operations are smooth. The [Coulomb slice for unitary connections](../../../fiber-bundle.md#coulomb-slice-for-unitary-connections) imposes $d_A^*a=0$. Its local existence follows from the gauge-fixing equation: the derivative in the gauge direction is $d_A^*d_A$, invertible on the orthogonal complement of its parallel kernel by the elliptic estimate. The local slice theorem then says that its remaining identifications are precisely by $\operatorname{Stab}(A)$.

On this slice the equation is

$$
F_{A+a}^+=d_A^+a+(a\wedge a)^+=0.
$$

Its kernel is the harmonic representative space $H_A^1$, and its cokernel is $H_A^2$. The hypothesis $H_A^2=0$ makes the obstruction target zero. Therefore the solutions near $A$ are an equivariant smooth graph over $H_A^1$, and the gauge-orbit neighborhood is a neighborhood of zero in $H_A^1/\operatorname{Stab}(A)$.

It remains to compute this representation, not just its dimension. A [reducible SU2 connection](../../../fiber-bundle.md#reducible-su2-connection) with circle holonomy preserves $E=L\oplus L^{-1}$. In this splitting,

$$
\operatorname{ad}E\cong\underline{\mathbb R}\oplus(L^2)_{\mathbb R},\qquad
\begin{pmatrix}it&z\\-\overline z&-it\end{pmatrix}
\longleftrightarrow(t,z).
$$

The diagonal part is a trivial real connection. Its degree-one deformation space is the space of ordinary harmonic one-forms. To check this directly, if $d^*a=0$ and $d^+a=0$, then $da$ is an exact [anti-self-dual two-form](../../../differential-form.md#anti-self-dual-differential-form). [Stokes theorem](../../../calculus.md#stokes-theorem) gives

$$
\|da\|_2^2=-\int_Xda\wedge da=-\int_Xd(a\wedge da)=0,
$$

so $da=0$ and $a$ is harmonic. This neutral deformation space vanishes because $b_1(X)=0$. Hence all of $H_A^1$ is in the off-diagonal part, where the complex structure of $L^2$ commutes with both operators; it is a complex vector space.

Using part (a), part (b), and $H_A^2=0$,

$$
\dim_{\mathbb R}H_A^1=\operatorname{ind}D_A+\dim H_A^0
=8e(E)-2,
\qquad
\boxed{d=\dim_{\mathbb C}H_A^1=4e(E)-1.}
$$

Parameterize the stabilizer by $u_\lambda=\operatorname{diag}(\lambda^{-1},\lambda)$, with $\lambda\in S^1$. Under our convention $A^u=u^{-1}Au+u^{-1}du$, its action on an off-diagonal perturbation is

$$
\begin{pmatrix}0&z\\-\overline z&0\end{pmatrix}
\longmapsto
\begin{pmatrix}0&\lambda^2z\\-\overline{\lambda^2z}&0\end{pmatrix}.
$$

Consequently the equivariant graph identifies a neighborhood of $[A]$ with a neighborhood of the origin in

$$
\boxed{\mathbb C^{\,4e(E)-1}/S^1,\qquad \lambda\cdot z=\lambda^2z.}
$$

This proves the exact scalar weight requested, with a stabilizer parametrization consistent with the chosen gauge convention. The ineffective kernel is $\{\pm1\}$. The orbit space is also the cone on $\mathbb{CP}^{d-1}$, because the weight-two circle has the same nonzero orbits as the ordinary scalar circle. This is the [local cone at an unobstructed reducible SU2 instanton](../../../fiber-bundle.md#local-cone-at-an-unobstructed-reducible-su2-instanton).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
