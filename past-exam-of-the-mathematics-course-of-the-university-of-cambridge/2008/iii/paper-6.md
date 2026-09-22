# Paper 6

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper6.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper6.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $k=\overline{\mathbb F}_q$, and let $F_0$ be the entrywise $q$th-power [Frobenius endomorphism of an algebraic group](../../../lie-theory.md#frobenius-endomorphism-of-an-algebraic-group) on the [general linear group](../../../group-theory.md#general-linear-group) $G=\mathrm{GL}_2(k)$. The [algebraic closure](../../../algebra.md#algebraic-closure) is visible in the original PDF; it is lost in the converted TeX. Let $T_0$ be the diagonal [maximal algebraic torus](../../../toric-geometry.md#maximal-algebraic-torus) and $B_0$ the upper triangular [Borel subgroup](../../../lie-theory.md#borel-subgroup).

Choose $\beta\in k$ with $\beta-\beta^q=1$. Such a $\beta$ exists because $k$ is an [algebraic closure](../../../algebra.md#algebraic-closure), and $\beta\notin\mathbb F_q$. Put

$$
h_+=\begin{pmatrix}1&\beta\\0&1\end{pmatrix},\qquad h_-=\begin{pmatrix}1&0\\\beta&1\end{pmatrix},\qquad F_\pm=\operatorname{Int}(h_\pm)\circ F_0\circ\operatorname{Int}(h_\pm)^{-1}.
$$

Transporting the standard $\mathbb F_q$-model through the [algebraic group](../../../algebraic-geometry.md#algebraic-group) automorphism $\operatorname{Int}(h_\pm)$ gives a [rational structure on an algebraic group](../../../lie-theory.md#rational-structure-on-an-algebraic-group) over the same field $\mathbb F_q$. In particular these are genuine [Frobenius endomorphisms of an algebraic group](../../../lie-theory.md#frobenius-endomorphism-of-an-algebraic-group), and their fixed-point groups are

$$
G^{F_\pm}=h_\pm\mathrm{GL}_2(\mathbb F_q)h_\pm^{-1}.
$$

The auxiliary $\beta$ need not be rational for the original structure: it changes the identification with the geometric group, not the field over which the transported model is defined.

For either sign, take the [rational maximal torus](../../../toric-geometry.md#rational-maximal-torus) and [Borel subgroup](../../../lie-theory.md#borel-subgroup)

$$
\boxed{T_\pm=h_\pm T_0h_\pm^{-1}\ \subset\ B_\pm=h_\pm B_0h_\pm^{-1}.}
$$

Indeed $F_\pm(h_\pm Hh_\pm^{-1})=h_\pm F_0(H)h_\pm^{-1}$ for $H=T_0,B_0$, so both subgroups are $F_\pm$-stable. Conjugacy also preserves maximality of the [algebraic torus](../../../toric-geometry.md#algebraic-torus) and the property of being a [Borel subgroup](../../../lie-theory.md#borel-subgroup).

Finally,

$$
F_\pm=\operatorname{Int}(c_\pm)F_0,\qquad c_+=\begin{pmatrix}1&1\\0&1\end{pmatrix},\quad c_-=\begin{pmatrix}1&0\\1&1\end{pmatrix}.
$$

Neither $c_+$ nor $c_-$ is central, so neither endomorphism is $F_0$. If $F_+=F_-$, surjectivity of $F_0$ on $G(k)$ would imply that $c_-^{-1}c_+$ is central. But

$$
c_-^{-1}c_+=\begin{pmatrix}1&1\\-1&0\end{pmatrix}
$$

is not scalar in any characteristic. Thus **the two nonstandard rational structures have distinct Frobenius endomorphisms**, including when $q=2$.

## 2

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For the [special linear group](../../../group-theory.md#special-linear-group) $G=\mathrm{SL}_3(\overline{\mathbb F}_q)$, let $N=q-1$, and choose a generator $\chi$ of the [character group](../../../group.md#character-group) of $\mathbb F_q^\times$. Every [linear character](../../../representation-theory.md#linear-character) of the diagonal [rational maximal torus](../../../toric-geometry.md#rational-maximal-torus) has a unique expression

$$
\theta\bigl(\operatorname{diag}(a,b,(ab)^{-1})\bigr)=\chi(a)^r\chi(b)^s,\qquad r,s\in\mathbb Z/N\mathbb Z.
$$

The upper triangular [Borel subgroup](../../../lie-theory.md#borel-subgroup) $B=TU$ is rational. Consequently its [Deligne-Lusztig induction](../../../lie-theory.md#deligne-lusztig-induction) is the actual [principal series of a finite reductive group](../../../lie-theory.md#principal-series-of-a-finite-reductive-group)

$$
R_T^G(\theta)=\operatorname{Ind}_{B^F}^{G^F}\widetilde\theta,
$$

where $\widetilde\theta$ is the [inflation of a group representation](../../../representation-theory.md#inflation-of-a-group-representation) across $B^F\to T^F$. The geometric reason for this split case is $X(1)=G^F/B^F$: the associated torus covering supplies $\theta$, and the auxiliary unipotent fibres contribute a single even cohomological degree, hence no minus sign.

The rational [Bruhat decomposition](../../../lie-theory.md#bruhat-decomposition) indexes $B^F\backslash G^F/B^F$ by $W=S_3$. Applying the [Mackey restriction formula](../../../representation-theory.md#mackey-restriction-formula) and [Frobenius reciprocity](../../../representation-theory.md#frobenius-reciprocity) gives

$$
\left\langle R_T^G(\theta),R_T^G(\theta)\right\rangle_{G^F}=\sum_{w\in S_3}\dim\operatorname{Hom}_{B^F\cap{}^{\dot w}B^F}\bigl(\widetilde\theta,{}^{\dot w}\widetilde\theta\bigr)=|\operatorname{Stab}_{S_3}(\theta)|.
$$

Each intersection contains $T^F$, and the two [linear characters](../../../representation-theory.md#linear-character) are trivial on its unipotent part. Its contribution is therefore one exactly when $w$ fixes $\theta$, and zero otherwise. Complete reducibility over $\mathbb C$ makes this [character inner product](../../../representation-theory.md#character-inner-product) the sum of squares of [irreducible representation](../../../representation-theory.md#irreducible-representation) multiplicities. Thus the [principal series of a finite reductive group](../../../lie-theory.md#principal-series-of-a-finite-reductive-group) is irreducible exactly when the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) stabilizer is trivial.

To compute that stabilizer, represent $\theta$ by the triple $(\chi^r,\chi^s,1)$. Two triples give the same [linear character](../../../representation-theory.md#linear-character) on determinant-one diagonal matrices exactly when they differ by a common factor $(\nu,\nu,\nu)$. For example, triviality of $(\eta_1,\eta_2,\eta_3)$ on all such matrices first gives $\eta_1=\eta_3$ by varying $a$, and then $\eta_2=\eta_3$ by varying $b$. The [Weyl group](../../../semisimple-lie-algebra.md#weyl-group) permutes the three entries.

A transposition fixes $\theta$ precisely when its two interchanged entries coincide: the third, fixed entry forces the common factor to be one. These three obstructions are $r=0$, $s=0$, and $r=s$. A three-cycle can also fix $\theta$ without any two entries coinciding. Its common factor must satisfy $\nu^3=1$; in the nontrivial case the entries, up to order and common factor, are $(1,\nu,\nu^2)$. This happens exactly when $3\mid N$ and $\{r,s\}=\{N/3,2N/3\}$.

The complete condition is therefore

$$
\boxed{r\not\equiv0,\quad s\not\equiv0,\quad r-s\not\equiv0\pmod N,\qquad 3\mid N\Longrightarrow\{r,s\}\ne\{N/3,2N/3\}.}
$$

In particular **pairwise distinct coordinate characters alone are insufficient**. For $q=4$ the only distinct triples have the order-three symmetry, and no character of this split [rational maximal torus](../../../toric-geometry.md#rational-maximal-torus) gives an irreducible [principal series of a finite reductive group](../../../lie-theory.md#principal-series-of-a-finite-reductive-group).

## 3

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Fix a [Borel subgroup](../../../lie-theory.md#borel-subgroup) $B$ and a [maximal algebraic torus](../../../toric-geometry.md#maximal-algebraic-torus) $T\subset B$. Conjugacy of [Borel subgroups](../../../lie-theory.md#borel-subgroup) and the equality $N_G(B)=B$ identify the [flag variety](../../../lie-theory.md#generalized-flag-variety) with $G/B$, by $gB\mapsto{}^gB$.

Every simultaneous conjugacy orbit on pairs contains a pair $(B,{}^gB)$: first conjugate its first member to $B$. The remaining allowed conjugations are by $B$. Two such pairs are in the same orbit exactly when $g'$ belongs to $BgB$. Indeed ${}^{g'}B={} ^{bg}B$ is equivalent to $(bg)^{-1}g'\in N_G(B)=B$. Thus there is an explicit bijection

$$
\boxed{G\backslash(\mathcal B\times\mathcal B)\ \longleftrightarrow\ B\backslash G/B.}
$$

The [Bruhat decomposition](../../../lie-theory.md#bruhat-decomposition) is the disjoint partition $G=\coprod_{w\in W}B\dot wB$, with $W=N_G(T)/T$. Under the displayed bijection its double coset $B\dot wB$ becomes the orbit

$$
O(w)=G\cdot(B,{}^{\dot w}B).
$$

This proves that the orbits are indexed by the [Weyl group](../../../semisimple-lie-algebra.md#weyl-group). Conversely, the assertion that these particular $O(w)$ exhaust the orbits without repetitions says precisely that the $B\dot wB$ exhaust $G$ without repetitions. Hence the orbit description and the [Bruhat decomposition](../../../lie-theory.md#bruhat-decomposition) are equivalent, not merely two sets of the same cardinality. Their common index is the [relative position of Borel subgroups](../../../lie-theory.md#relative-position-of-borel-subgroups).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Choose a rational [Borel subgroup](../../../lie-theory.md#borel-subgroup) $B=TU$ with rational [maximal algebraic torus](../../../toric-geometry.md#maximal-algebraic-torus) $T$, and use the [Lang map](../../../lie-theory.md#lang-map) $\mathcal L(g)=g^{-1}F(g)$. Conjugating the pair $({}^gB,F({}^gB))$ by $g^{-1}$ gives $(B,{}^{\mathcal L(g)}B)$. Part (a) therefore gives

$$
({}^gB,F({}^gB))\in O(w)\quad\Longleftrightarrow\quad\mathcal L(g)\in B\dot wB.
$$

Moreover $\mathcal L(gb)=b^{-1}\mathcal L(g)F(b)$, and $F(B)=B$, so this inverse image is stable under right multiplication by $B$. The [flag variety](../../../lie-theory.md#generalized-flag-variety) identification consequently restricts to the required isomorphism

$$
\boxed{X(w)\cong\mathcal L^{-1}(B\dot wB)/B.}
$$

**The second printed isomorphism is false as written: it omits a unipotent quotient.** Take $G=\mathrm{SL}_2(\overline{\mathbb F}_q)$ with standard [Frobenius endomorphism of an algebraic group](../../../lie-theory.md#frobenius-endomorphism-of-an-algebraic-group) and $w=1$. Then $X(1)$ consists of the $q+1$ rational lines in $\mathbb F_q^2$, so has dimension zero. Every [Borel subgroup](../../../lie-theory.md#borel-subgroup) $B'$ has one-dimensional [unipotent radical](../../../lie-theory.md#unipotent-radical) $U'$. The [Lang map](../../../lie-theory.md#lang-map) is a finite surjective [étale morphism](../../../ringed-space.md#etale-morphism), so $\mathcal L^{-1}(U')$ has dimension one. Quotienting by the finite group $T'^F$ preserves that dimension. Thus no choices of $T'$ and $B'$ can make the asserted two varieties isomorphic in this example.

Here is the corrected construction, including the missing quotient. Choose $x$ by the [Lang theorem for algebraic groups](../../../lie-theory.md#lang-theorem-for-algebraic-groups) so that $x^{-1}F(x)=\dot w$. Define

$$
T'=xTx^{-1},\qquad U_x=xUx^{-1},\qquad B'=F(xBx^{-1}),\qquad U'=R_u(B')=F(U_x).
$$

Then $F(T')=x\dot wT\dot w^{-1}x^{-1}=T'$, so $T'$ is a [rational maximal torus](../../../toric-geometry.md#rational-maximal-torus) contained in $B'$. Put $J=U_x\cap U'=F^{-1}(U')\cap U'$. The correct [unipotent quotient in a Deligne-Lusztig variety](../../../lie-theory.md#unipotent-quotient-in-a-deligne-lusztig-variety) is

$$
\boxed{\mathcal L^{-1}(U')/(J\rtimes T'^F)\cong X(w),\qquad h\longmapsto hxB.}
$$

The semidirect product denotes the subgroup $JT'^F$ acting on the right. Both $U_x$ and $U'$ are normalized by $T'$, so the action is well defined. Also

$$
\mathcal L(hx)=x^{-1}\mathcal L(h)F(x)\in\dot wU\subset B\dot wB
$$

for $h\in\mathcal L^{-1}(U')$, showing directly that the map lands in the [Deligne-Lusztig variety](../../../lie-theory.md#deligne-lusztig-variety).

To prove surjectivity and identify its fibres, use the intermediate variety

$$
Y(\dot w)=\{g:\mathcal L(g)\in U\dot wU\}/U,\qquad F_w(t)=\dot wF(t)\dot w^{-1}\quad(t\in T).
$$

The right $U$-action follows from the twisted-translation identity for the [Lang map](../../../lie-theory.md#lang-map). Right multiplication by $T^{F_w}$ also acts, and $Y(\dot w)/T^{F_w}\cong X(w)$. Indeed if $\mathcal L(g)\in B\dot wB$, write it as $u_1t\dot wu_2$. Replacing $g$ by $ga$, with $a\in T$, changes its torus factor to $a^{-1}tF_w(a)$. Surjectivity of the twisted [Lang map](../../../lie-theory.md#lang-map) on the connected [algebraic torus](../../../toric-geometry.md#algebraic-torus) makes this factor one. Once the factor is one, two representatives of the same flag differ by $ua$ with $u\in U$ and $a\in T^{F_w}$. This proves both surjectivity and the asserted finite covering, including its group of fibres.

Now map $Z=\mathcal L^{-1}(U')$ to $Y(\dot w)$ by $h\mapsto hxU$. Given $\mathcal L(g)=u_1\dot wu_2$, replace $g$ by $gu_1$. Then

$$
\mathcal L(gu_1)=\dot wu_2F(u_1)\in\dot wU.
$$

Thus $h=gu_1x^{-1}$ belongs to $Z$ and maps to the original point $gU$. This proves surjectivity. Two preimages have the form $h$ and $hk$, where $k\in U_x$. Since $F(k)\in U'$ and $\mathcal L(h)\in U'$, the identity

$$
\mathcal L(hk)=k^{-1}\mathcal L(h)F(k)
$$

shows that $hk\in Z$ precisely when $k\in U'$, hence precisely when $k\in J$. Therefore the fibres are exactly the right $J$-orbits.

These are isomorphisms of [geometric quotients](../../../toric-geometry.md#geometric-quotient), not just bijections on points. The groups $U_x,U'$ contain root subgroups for the same [maximal algebraic torus](../../../toric-geometry.md#maximal-algebraic-torus), so their intersection $J$ is smooth. The map $Z\to Y(\dot w)$ is a smooth surjection with fibre $J$: the differential of the [Lang map](../../../lie-theory.md#lang-map) is invertible, and the kernel of the differential of $h\mapsto hxU$ on $Z$ is the translate of $\operatorname{Lie}(U_x)\cap\operatorname{Lie}(U')=\operatorname{Lie}(J)$. This gives $Z/J\cong Y(\dot w)$. Finally $xT^{F_w}x^{-1}=T'^F$, so quotienting the remaining finite torus action gives the displayed corrected formula.

For $w=1$, $J=U_x$ is exactly the affine-line factor in the counterexample. More generally $Z/T'^F\to X(w)$ retains unipotent fibres of dimension $\dim J$; it becomes the printed isomorphism only when this intersection is trivial. The missing factor is also recorded in the quotient construction in [Tiep's lectures, proof of Theorem 5.22](https://viasm.edu.vn/Cms_Data/Contents/viasm/Media/file/viasm_2016.pdf).

## 4

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $P=L\ltimes U$ and $Q=M\ltimes V$ be rational [parabolic subgroups](../../../lie-theory.md#parabolic-subgroup) with rational [Levi subgroups](../../../lie-theory.md#levi-subgroup). Work with complex representations of their [finite groups of Lie type](../../../lie-theory.md#finite-group-of-lie-type). Here [Harish-Chandra induction](../../../lie-theory.md#harish-chandra-induction) and [Harish-Chandra restriction](../../../lie-theory.md#harish-chandra-restriction) mean

$$
R_{L\subset P}^{G}(E)=\operatorname{Ind}_{P^F}^{G^F}\operatorname{Inf}_{L^F}^{P^F}E,\qquad {}^*R_{M\subset Q}^{G}(A)=A^{V^F}.
$$

The latter is an $M^F$-module, and it is adjoint to the former by [Frobenius reciprocity](../../../representation-theory.md#frobenius-reciprocity).

Define

$$
\mathcal S(M,L)=\{x\in G:M\cap{}^xL\text{ contains a maximal algebraic torus of }G\}.
$$

For $x\in\mathcal S(M,L)^F$, put $H_x=M\cap{}^xL$ and let $\operatorname{ad}x$ transport an $L^F$-module to a $({}^xL)^F$-module. The [Mackey formula for Harish-Chandra induction](../../../lie-theory.md#mackey-formula-for-harish-chandra-induction) is the natural functor isomorphism

$$
\boxed{{}^*R_{M\subset Q}^{G}R_{L\subset P}^{G}\cong\bigoplus_{x\in M^F\backslash\mathcal S(M,L)^F/L^F}R_{H_x\subset M\cap{}^xP}^{M}\ {}^*R_{H_x\subset Q\cap{}^xL}^{{}^xL}\ \operatorname{ad}x.}
$$

On [characters](../../../representation-theory.md#character-of-a-representation) the direct sum becomes a sum. The intersection parabolics displayed in the subscripts are important: they specify exactly which [Harish-Chandra induction](../../../lie-theory.md#harish-chandra-induction) and [Harish-Chandra restriction](../../../lie-theory.md#harish-chandra-restriction) occur.

We use the following parabolic-intersection lemmas, stating explicitly the geometric input to the proof. First, representatives of $M^F\backslash\mathcal S(M,L)^F/L^F$ represent exactly the double cosets $Q^F\backslash G^F/P^F$. Second, for such $x$, the groups $M\cap{}^xP$ and $Q\cap{}^xL$ are [parabolic subgroups](../../../lie-theory.md#parabolic-subgroup) of $M$ and ${}^xL$, respectively, with common [Levi subgroup](../../../lie-theory.md#levi-subgroup) $H_x$ and respective [unipotent radicals](../../../lie-theory.md#unipotent-radical) $M\cap{}^xU$ and $V\cap{}^xL$. If $K=Q\cap{}^xP$, projection $Q\to M$ maps $K$ onto $M\cap{}^xP$ with kernel $K\cap V$. Projection ${}^xP\to{}^xL$ maps $K\cap V$ onto $V\cap{}^xL$ with kernel $V\cap{}^xU$. These assertions hold on rational points as well. The surjectivity on rational points uses connectedness of the unipotent kernels and the [Lang theorem for algebraic groups](../../../lie-theory.md#lang-theorem-for-algebraic-groups). These are the compatible-Levi and rational double-coset lemmas; they follow by applying the root-subgroup decomposition after choosing the common [maximal algebraic torus](../../../toric-geometry.md#maximal-algebraic-torus).

For completeness, the representation-theoretic reduction is as follows. The [group algebra](../../../associative-algebra.md#group-algebra) realization of [induced representation](../../../representation-theory.md#induced-representation) splits according to the double cosets:

$$
\mathbb C[G^F]=\bigoplus_x\mathbb C[Q^FxP^F]
$$

as a $(Q^F,P^F)$-bimodule. Tensoring on the right with an inflated $L^F$-module $E$ identifies each summand with induction from $K^F=(Q\cap{}^xP)^F$. This proves the finite-group [Mackey restriction formula](../../../representation-theory.md#mackey-restriction-formula) in the form

$$
\operatorname{Res}_{Q^F}^{G^F}R_{L\subset P}^{G}(E)\cong\bigoplus_x\operatorname{Ind}_{K^F}^{Q^F}\left(\operatorname{Res}_{K^F}^{({}^xP)^F}{}^x\widetilde E\right).
$$

Here ${}^x\widetilde E$ is trivial on $({}^xU)^F$.

We next record the elementary normal-subgroup identity underlying [Harish-Chandra restriction](../../../lie-theory.md#harish-chandra-restriction). If $N\triangleleft D$ are finite groups, with $N$ a [normal subgroup](../../../group-theory.md#normal-subgroup), and $C\subset D$, then for a complex $C$-module $A$,

$$
\left(\operatorname{Ind}_C^D A\right)^N\cong\operatorname{Ind}_{CN/N}^{D/N} A^{C\cap N}.
$$

To see this, replace invariants by coinvariants using the averaging idempotent $|N|^{-1}\sum_{n\in N}n$. Taking coinvariants in $\mathbb C[D]\otimes_{\mathbb C[C]}A$ first replaces $\mathbb C[D]$ by $\mathbb C[D/N]$, and forces $C\cap N$ to act trivially on $A$. Thus it yields $\mathbb C[D/N]\otimes_{\mathbb C[CN/N]}A_{C\cap N}$; averaging over $C\cap N$ identifies this last module with the one displayed. This also shows why characteristic zero makes the argument exact.

Apply this identity to $D=Q^F$, $N=V^F$, $C=K^F$. By the intersection lemmas, $CN/N=(M\cap{}^xP)^F$. Since ${}^x\widetilde E$ is trivial on $({}^xU)^F$, its $(K\cap V)^F$-invariants are exactly

$$
({}^xE)^{(V\cap{}^xL)^F}={}^*R_{H_x\subset Q\cap{}^xL}^{{}^xL}({}^xE).
$$

Moreover $(M\cap{}^xU)^F$ acts trivially on this module, so induction from $(M\cap{}^xP)^F$ to $M^F$ is precisely [Harish-Chandra induction](../../../lie-theory.md#harish-chandra-induction) from $H_x$. Substituting into each double-coset summand gives the boxed formula. This proves the formula for rational parabolics; it does not assume a general Mackey formula for nonrational [Deligne-Lusztig induction](../../../lie-theory.md#deligne-lusztig-induction).

## 5

↑ **Parent:** [Paper 6](paper-6.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Write $\chi=\varepsilon R_T^G(\theta)$, where $\varepsilon\in\{1,-1\}$ and $\chi$ is the character of an [irreducible representation](../../../representation-theory.md#irreducible-representation). An irreducible representation is a [cuspidal representation of a finite reductive group](../../../lie-theory.md#cuspidal-representation-of-a-finite-reductive-group) exactly when its [Harish-Chandra restriction](../../../lie-theory.md#harish-chandra-restriction) to every proper rational [Levi subgroup](../../../lie-theory.md#levi-subgroup) of a rational [parabolic subgroup](../../../lie-theory.md#parabolic-subgroup) is zero.

The needed identity is the [Harish-Chandra restriction of a Deligne-Lusztig character](../../../lie-theory.md#harish-chandra-restriction-of-a-deligne-lusztig-character). For a rational [parabolic subgroup](../../../lie-theory.md#parabolic-subgroup) $P=M\ltimes V$, the torus case of the induction-restriction formula gives

$$
{}^*R_{M\subset P}^{G}R_T^G(\theta)=\sum_{x\in M^F\backslash\{g\in G^F:{}^gT\subset M\}/T^F}R_{{}^xT}^{M}({}^x\theta).
$$

Here ${}^x\theta(xtx^{-1})=\theta(t)$. The geometric meaning of the indexing condition is that only a rational conjugate of the inducing [maximal algebraic torus](../../../toric-geometry.md#maximal-algebraic-torus) lying in the Levi can survive taking $V^F$-invariants. This is the established torus case of [Deligne-Lusztig induction](../../../lie-theory.md#deligne-lusztig-induction), valid without a restriction on $q$; it is not an appeal to an unrestricted induction-restriction conjecture. See [Dudas and Michel's lectures, Theorem 14.4](https://webusers.imj-prg.fr/~jean.michel/papiers/lectures_beijing_2015.pdf).

Suppose first that $T$ is an [elliptic maximal torus](../../../toric-geometry.md#elliptic-maximal-torus), meaning it lies in no proper rational [parabolic subgroup](../../../lie-theory.md#parabolic-subgroup). For any proper rational $P=M\ltimes V$, the indexing set in the displayed sum is empty. Indeed ${}^xT\subset M$ with $x\in G^F$ would imply $T\subset{}^{x^{-1}}P$, itself a proper rational [parabolic subgroup](../../../lie-theory.md#parabolic-subgroup). Hence ${}^*R_{M\subset P}^{G}R_T^G(\theta)=0$, and multiplication by $\varepsilon$ gives ${}^*R_{M\subset P}^{G}\chi=0$. This proves cuspidality.

Conversely suppose $T\subset P$ for a proper rational [parabolic subgroup](../../../lie-theory.md#parabolic-subgroup). There is a unique [Levi subgroup](../../../lie-theory.md#levi-subgroup) of $P$ containing this particular [maximal algebraic torus](../../../toric-geometry.md#maximal-algebraic-torus): relative to $T$, it is generated by $T$ and those root subgroups for which both the root and its negative occur in $P$. Call it $M$. Uniqueness and $F(T)=T$, $F(P)=P$ imply $F(M)=M$, so this is a proper rational Levi. Transitivity of [Deligne-Lusztig induction](../../../lie-theory.md#deligne-lusztig-induction) through this rational parabolic says

$$
R_T^G(\theta)=R_{M\subset P}^{G}\bigl(R_T^M(\theta)\bigr).
$$

Set $\psi=R_T^M(\theta)$, allowing it to be a [virtual character](../../../representation-theory.md#virtual-character). Adjunction of [Harish-Chandra induction](../../../lie-theory.md#harish-chandra-induction) and [Harish-Chandra restriction](../../../lie-theory.md#harish-chandra-restriction), extended linearly to [virtual characters](../../../representation-theory.md#virtual-character), gives

$$
\left\langle{}^*R_{M\subset P}^{G}\chi,\psi\right\rangle_{M^F}=\left\langle\chi,R_{M\subset P}^{G}\psi\right\rangle_{G^F}=\left\langle\chi,R_T^G(\theta)\right\rangle_{G^F}=\varepsilon\langle\chi,\chi\rangle_{G^F}=\varepsilon\ne0.
$$

Thus this [Harish-Chandra restriction](../../../lie-theory.md#harish-chandra-restriction) cannot vanish, so $\chi$ is not cuspidal. No positivity or irreducibility of $\psi$ is needed, and the sign in $\chi$ causes no cancellation problem. We have proved

$$
\boxed{\varepsilon R_T^G(\theta)\text{ irreducible is cuspidal}\quad\Longleftrightarrow\quad T\text{ is elliptic}.}
$$

The term [elliptic maximal torus](../../../toric-geometry.md#elliptic-maximal-torus) is relative to the ambient group: split central factors are allowed. The actual condition is absence of a proper rational [parabolic subgroup](../../../lie-theory.md#parabolic-subgroup) containing $T$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
