# Paper 165

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_165.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_165.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
  - [vi](#2/vi)
    - [Solution](#2/vi/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 165](paper-165.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The [simplex category](../../../algebraic-topology.md#simplex-category) $\Delta$ has objects $[n]=\{0<1<\cdots<n\}$ for $n\geq0$ and order-preserving maps as morphisms. A [simplicial set](../../../algebraic-topology.md#simplicial-set) is a [functor](../../../category.md#functor) $X:\Delta^{\mathrm{op}}\to\mathbf{Set}$.

The [standard simplex](../../../algebraic-topology.md#standard-simplex) is the representable simplicial set

$$
\Delta^n_m=\operatorname{Hom}_\Delta([m],[n]).
$$

For $0\leq i\leq n$, the [simplicial horn](../../../algebraic-topology.md#simplicial-horn) $\Lambda_i^n\subseteq\Delta^n$ is the union of the images of all coface maps $\Delta^{n-1}\to\Delta^n$ except the face opposite vertex $i$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

A [quasicategory](../../../algebraic-topology.md#quasicategory) is a [simplicial set](../../../algebraic-topology.md#simplicial-set) having the right lifting property against every [inner horn](../../../algebraic-topology.md#inner-horn) inclusion

$$
\Lambda_i^n\hookrightarrow\Delta^n,
\qquad 0<i<n.
$$

A [Kan complex](../../../algebraic-topology.md#kan-complex) has the right lifting property against every [simplicial horn](../../../algebraic-topology.md#simplicial-horn) inclusion, including the two outer horns $i=0,n$.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

The [Yoneda lemma](../../../category.md#yoneda-lemma) and the definition of the [nerve of a category](../../../algebraic-topology.md#nerve-category-theory) give

$$
\operatorname{Hom}_{\mathbf{sSet}}(\Delta^n,N(\mathcal C))
\cong N(\mathcal C)_n
=\operatorname{Fun}([n],\mathcal C).
$$

Thus such a map is precisely a diagram of objects and composable morphisms

$$
C_0\longrightarrow C_1\longrightarrow\cdots\longrightarrow C_n
$$

in $\mathcal C$. The remaining edges and higher faces record the composites forced by this string.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Consider a lifting square with $\Lambda_1^3\hookrightarrow\Delta^3$ on the left, $Q\to N(\mathcal C)$ on the right, and prescribed bottom simplex $\sigma:\Delta^3\to N(\mathcal C)$. Since $Q$ is a [quasicategory](../../../algebraic-topology.md#quasicategory), the top horn has some filler $\widetilde\sigma:\Delta^3\to Q$.

The two simplices $p\widetilde\sigma$ and $\sigma$ of the [nerve of a category](../../../algebraic-topology.md#nerve-category-theory) restrict to the same inner horn. Inner horns in a category's nerve have unique fillers, because composition in a category is defined and unique. Hence $p\widetilde\sigma=\sigma$, so $\widetilde\sigma$ is the required lift.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

The contravariant [simplicial mapping space](../../../algebraic-topology.md#simplicial-mapping-space) functor takes the given pushout to the stated strict pullback. Since $X$ is a [Kan complex](../../../algebraic-topology.md#kan-complex), all four mapping spaces are [Kan complexes](../../../algebraic-topology.md#kan-complex). Moreover, the monomorphism $A\hookrightarrow B$ induces a Kan fibration

$$
\underline{\operatorname{Hom}}(B,X)
\longrightarrow\underline{\operatorname{Hom}}(A,X).
$$

Indeed, a lifting problem against a horn is adjoint to a lifting problem for $X$ against the pushout-product of $A\hookrightarrow B$ with that horn inclusion; this pushout-product is an anodyne monomorphism, and $X$ fills it.

A strict pullback of fibrant simplicial sets along a fibration computes the [homotopy pullback](../../../algebraic-topology.md#homotopy-pullback). The displayed pullback square is therefore also a homotopy pullback square.

## 2

↑ **Parent:** [Paper 165](paper-165.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For a [simplicial abelian group](../../../algebraic-topology.md#simplicial-abelian-group) $A$, its [normalized chain complex of a simplicial abelian group](../../../algebraic-topology.md#normalized-chain-complex-of-a-simplicial-abelian-group) is

$$
N_nA=\bigcap_{i=1}^n\ker(d_i:A_n\to A_{n-1}),
\qquad \partial_n=d_0|_{N_nA}.
$$

The simplicial identities give $\partial^2=0$. Equivalently, $N_nA$ is the quotient of $A_n$ by the subgroup generated by degenerate simplices, with differential induced by $\sum_i(-1)^id_i$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The [Dold–Kan correspondence](../../../algebraic-topology.md#dold-kan-correspondence) says that

$$
N_*:\mathbf{sAb}\longrightarrow\mathbf{Ch}_{\geq0}(\mathbf{Ab})
$$

is an equivalence from [simplicial abelian groups](../../../algebraic-topology.md#simplicial-abelian-group) to nonnegatively graded [chain complexes](../../../homology.md#chain-complex) of [abelian groups](../../../group.md#abelian-group). The restriction of the right adjoint $K$ to $\mathbf{Ch}_{\geq0}(\mathbf{Ab})$ is a quasi-inverse: both the unit $C_*\to N_*K(C_*)$ and counit $K(N_*A)\to A$ are natural isomorphisms.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Under the [Dold–Kan correspondence](../../../algebraic-topology.md#dold-kan-correspondence), a $1$-simplex of $K(C_*)$ is a pair $(a,x)\in C_0\oplus C_1$ with

$$
d_1(a,x)=a,
\qquad d_0(a,x)=a+\partial_1x.
$$

The horn $\Lambda_1^2$ consists of the edges $01$ and $12$, joined at vertex $1$. A map from it is therefore a pair of composable $1$-simplices, equivalently a triple

$$
(a,x,y)\in C_0\times C_1\times C_1,
$$

where the first edge is $(a,x)$ and the second is $(a+\partial_1x,y)$. Thus

$$
\boxed{\operatorname{Hom}_{\mathbf{sSet}}(\Lambda_1^2,K(C_*))
\cong C_0\times C_1\times C_1.}
$$

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Let $A[n]$ be the nonnegative [chain complex](../../../homology.md#chain-complex) having $A$ in degree $n$, zero in every other degree, and zero differential. The simplicial [Eilenberg–MacLane space](../../../algebraic-topology.md#eilenberg-maclane-space) is

$$
K(A,n):=K(A[n]).
$$

Its underlying [simplicial set](../../../algebraic-topology.md#simplicial-set) is a [Kan complex](../../../algebraic-topology.md#kan-complex), with $\pi_nK(A,n)\cong A$ and all other positive [homotopy groups](../../../algebraic-topology.md#homotopy-group) zero.

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

Regard the given [short exact sequence](../../../module-theory.md#short-exact-sequence) as a degreewise short exact sequence of [chain complexes](../../../homology.md#chain-complex) concentrated in degree $n$. The inverse functor in the [Dold–Kan correspondence](../../../algebraic-topology.md#dold-kan-correspondence) is exact, so it produces a degreewise short exact sequence of [simplicial abelian groups](../../../algebraic-topology.md#simplicial-abelian-group)

$$
0\longrightarrow K(A_1,n)\longrightarrow K(A_2,n)\longrightarrow K(A_3,n)\longrightarrow0.
$$

The last map is degreewise surjective and hence a Kan fibration. Its strict fiber is $K(A_1,n)$, and a strict fiber of a fibration computes the homotopy fiber. This proves the asserted [homotopy fiber sequence](../../../algebraic-topology.md#homotopy-fiber-sequence) of pointed [Kan complexes](../../../algebraic-topology.md#kan-complex).

<h3 id="2/vi">vi</h3>

↑ **Parent:** [2](#2)

<h4 id="2/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#2/vi)

Products of [Eilenberg–MacLane spaces](../../../algebraic-topology.md#eilenberg-maclane-space) satisfy

$$
K(\mathbb Z/4,3)\times K(\mathbb Z/5,3)
\simeq K(\mathbb Z/4\oplus\mathbb Z/5,3)
\cong K(\mathbb Z/20,3),
$$

where the last isomorphism uses the [Chinese remainder theorem](../../../mathematics.md#chinese-remainder-theorem). This space is $2$-connected, so the [Hurewicz theorem](../../../algebraic-topology.md#hurewicz-theorem) identifies

$$
H_3(-;\mathbb Z)\cong\pi_3(-)\cong\mathbb Z/20.
$$

The assumed surjection on $H_3$ is an isomorphism because the group is finite. Hence $f$ is an isomorphism on $\pi_3$; all other homotopy groups of the source and target vanish. Thus $f$ is a weak homotopy equivalence, and the [Whitehead theorem](../../../algebraic-topology.md#whitehead-theorem) for [Kan complexes](../../../algebraic-topology.md#kan-complex) makes it a [homotopy equivalence](../../../algebraic-topology.md#homotopy-equivalence).

## 3

↑ **Parent:** [Paper 165](paper-165.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Use the [path-loop fibration](../../../algebraic-topology.md#path-loop-fibration)

$$
\Omega S^4\longrightarrow PS^4\longrightarrow S^4
$$

and its rational [Serre spectral sequence](../../../algebraic-topology.md#serre-spectral-sequence). The total space is contractible, while $H^*(S^4;\mathbb Q)$ is $\mathbb Q$ in degrees $0$ and $4$ and zero otherwise. The only possible nonzero differential is

$$
d_4:E_4^{0,q}\longrightarrow E_4^{4,q-3}.
$$

Convergence to the cohomology of a point first forces $d_4:H^3(\Omega S^4;\mathbb Q)\to H^4(S^4;\mathbb Q)$ to be an isomorphism, and then inductively forces an isomorphism from each nonzero vertical group to the group three degrees below it in the other column. Therefore

$$
H^i(\Omega S^4;\mathbb Q)\cong
\begin{cases}
\mathbb Q,&i=0,3,6,9,\ldots,\\
0,&\text{otherwise}.
\end{cases}
$$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Apply the rational [Serre spectral sequence](../../../algebraic-topology.md#serre-spectral-sequence) to the path-loop fibration of $K(\mathbb Z,3)$. Its fiber is

$$
\Omega K(\mathbb Z,3)\simeq K(\mathbb Z,2)\simeq\mathbb{CP}^{\infty},
$$

whose rational [cohomology ring](../../../cohomology.md#cohomology-ring) is $\mathbb Q[c]$ with $|c|=2$. Since the path space is contractible, $c$ must transgress to a nonzero class $x\in H^3(K(\mathbb Z,3);\mathbb Q)$. Multiplicativity gives

$$
d_3(c^m)=m c^{m-1}x.
$$

Over $\mathbb Q$ these differentials pair and kill every positive-degree class except $x$, while graded commutativity gives $x^2=0$. Hence

$$
H^i(K(\mathbb Z,3);\mathbb Q)\cong
\begin{cases}
\mathbb Q,&i=0,3,\\
0,&\text{otherwise}.
\end{cases}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The [loop-space shift of homotopy groups](../../../algebraic-topology.md#loop-space-shift-of-homotopy-groups) gives

$$
\pi_i(\Omega S^4)\cong\pi_{i+1}(S^4).
$$

Thus $\Omega S^4$ is $2$-connected and its first nonzero homotopy group is

$$
\pi_3(\Omega S^4)\cong\pi_4(S^4)\cong\mathbb Z.
$$

The [Hurewicz theorem](../../../algebraic-topology.md#hurewicz-theorem) now gives

$$
H_3(\Omega S^4;\mathbb Z)\cong\mathbb Z,
$$

and every positive integral homology group below degree $3$ vanishes. The smallest requested degree is therefore $i=3$.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

The rational cohomology from part i has one generator in every degree divisible by $3$. Its connected graded-commutative Hopf algebra structure is

$$
H^*(\Omega S^4;\mathbb Q)
\cong\Lambda(x_3)\otimes\mathbb Q[y_6]
$$

as a graded vector-space-compatible algebra: the odd class has square zero and the degree-six class supplies the even multiples. The rational Hurewicz and Hopf-algebra correspondence for a connected loop space identifies the indecomposable generators with the duals of its [rational homotopy groups](../../../algebraic-topology.md#rational-homotopy-group). Hence, for $0\leq i\leq6$,

$$
\pi_i(\Omega S^4)\otimes\mathbb Q\cong
\begin{cases}
\mathbb Q,&i=3,6,\\
0,&i=0,1,2,4,5.
\end{cases}
$$

This also agrees with the [rational homotopy groups of a sphere](../../../algebraic-topology.md#rational-homotopy-groups-of-a-sphere) and the [loop-space shift of homotopy groups](../../../algebraic-topology.md#loop-space-shift-of-homotopy-groups).

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

By the [loop-space shift of homotopy groups](../../../algebraic-topology.md#loop-space-shift-of-homotopy-groups),

$$
\pi_7(S^4)\otimes\mathbb Q
\cong\pi_6(\Omega S^4)\otimes\mathbb Q.
$$

Part iv therefore gives

$$
\boxed{\pi_7(S^4)\otimes\mathbb Q\cong\mathbb Q.}
$$

## 4

↑ **Parent:** [Paper 165](paper-165.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Write $F=K(\mathbb Z/4,1)$, $E=K(\mathbb Z,2)$, and $B=K(\mathbb Z,2)$. In total degree at most two, the $E_2$ page of the mod-two [Serre spectral sequence](../../../algebraic-topology.md#serre-spectral-sequence) has

$$
E_2^{0,0}=E_2^{0,1}=E_2^{0,2}=E_2^{2,0}=\mathbb F_2,
$$

and $E_2^{1,0}=E_2^{1,1}=0$. A periodic free resolution of the cyclic group gives $H_1(F;\mathbb Z)=\mathbb Z/4$ and $H_2(F;\mathbb Z)=0$. Hence $H^1(F;\mathbb F_2)\cong\operatorname{Hom}(\mathbb Z/4,\mathbb F_2)$, while the [universal coefficient theorem for cohomology](../../../cohomology.md#universal-coefficient-theorem-for-cohomology) gives $H^2(F;\mathbb F_2)\cong\operatorname{Ext}(\mathbb Z/4,\mathbb F_2)$; both are one-dimensional.

The edge map $H^2(B;\mathbb F_2)\to H^2(E;\mathbb F_2)$ is induced by multiplication by $4$ and is therefore zero modulo two. Consequently

$$
d_2:E_2^{0,1}\longrightarrow E_2^{2,0}
$$

is an isomorphism. The differential out of $E_2^{0,2}$ is zero, because the total space has a one-dimensional $H^2$ which must survive in filtration zero. Thus for every $r\geq3$ and $p+q\leq2$,

$$
E_r^{0,0}=E_r^{0,2}=\mathbb F_2
$$

and all other groups in that range vanish.

It follows that

$$
H^0(F;\mathbb F_2)=H^1(F;\mathbb F_2)=H^2(F;\mathbb F_2)=\mathbb F_2.
$$

The surviving filtration-zero class is the restriction of the degree-two class of $E$, so

$$
\boxed{\operatorname{im}H^2(f;\mathbb F_2)=H^2(F;\mathbb F_2).}
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Let $P$ be the homotopy fiber of the map representing

$$
\operatorname{Sq}^1:K(\mathbb F_2,1)\longrightarrow K(\mathbb F_2,2).
$$

The long exact sequence of [homotopy groups](../../../algebraic-topology.md#homotopy-group) shows that every $\pi_i(P)$ except $\pi_1(P)$ vanishes and that

$$
0\longrightarrow\mathbb F_2\longrightarrow\pi_1(P)
\longrightarrow\mathbb F_2\longrightarrow0.
$$

Hence $P$ is either $K(\mathbb F_2\oplus\mathbb F_2,1)$ or $K(\mathbb Z/4,1)$.

The extension is classified by the degree-two class represented by the original map. If $t\in H^1(K(\mathbb F_2,1);\mathbb F_2)$ is the standard generator, that class is

$$
\operatorname{Sq}^1t=t^2\ne0
$$

in $H^*(\mathbb{RP}^{\infty};\mathbb F_2)=\mathbb F_2[t]$. It therefore classifies the non-split extension, whose middle group is $\mathbb Z/4$. Thus

$$
\boxed{P\simeq K(\mathbb Z/4,1).}
$$

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

The group $H^1(K(\mathbb Z/4,1);\mathbb F_2)$ is one-dimensional, so it suffices to consider its nonzero class $x$. This class is represented by the quotient homomorphism $\mathbb Z/4\to\mathbb Z/2$, which lifts to the identity homomorphism with coefficients in $\mathbb Z/4$. Its [Bockstein homomorphism](../../../homology.md#bockstein-homomorphism) for

$$
0\longrightarrow\mathbb Z/2\longrightarrow\mathbb Z/4
\longrightarrow\mathbb Z/2\longrightarrow0
$$

therefore vanishes. Since the first [Steenrod square](../../../cohomology.md#steenrod-square) is this Bockstein and $\operatorname{Sq}^1x=x^2$ for every degree-one class,

$$
x^2=0.
$$

The zero degree-one class plainly has square zero as well.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
