# Paper 5

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper5.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper5.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
    - [i](#3/iii/i)
      - [Solution](#3/iii/i/solution)
    - [ii](#3/iii/ii)
      - [Solution](#3/iii/ii/solution)
    - [iii](#3/iii/iii)
      - [Solution](#3/iii/iii/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)

## 1

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [topological group](../../../topological-group.md) is a [group](../../../group.md) with a [topology](../../../topology.md) for which multiplication $G\times G\to G$ and inversion $G\to G$ are continuous. A [profinite group](../../../topological-group.md#profinite-group) has either of the following equivalent descriptions: **a [compact](../../../topology.md#compact-space) [Hausdorff](../../../topology.md#hausdorff-space) [totally disconnected](../../../arithmetic.md#totally-disconnected-space) [topological group](../../../topological-group.md)**, or **an [inverse limit](../../../module-theory.md#inverse-limit) of finite discrete [groups](../../../group.md)**. [Totally disconnected](../../../arithmetic.md#totally-disconnected-space) means that every [connected component](../../../geometry-and-topology.md#connected-component) is a singleton.

For clarity, an [inverse system](../../../module-theory.md#inverse-system) over a [directed set](../../../set.md#directed-set) $I$ consists of [groups](../../../group.md) $G_i$ and maps $\phi_{ij}:G_j\to G_i$ for $i\le j$, with $\phi_{ii}=1$ and $\phi_{ik}=\phi_{ij}\phi_{jk}$. Its [inverse limit](../../../module-theory.md#inverse-limit) is

$$
\varprojlim G_i=\{(g_i)\in\prod_iG_i:\phi_{ij}(g_j)=g_i\text{ whenever }i\le j\},
$$

with coordinatewise multiplication and the [subspace topology](../../../topology.md#subspace-topology). Equivalently, it is a [group](../../../group.md) with compatible continuous projections such that every other compatible family of maps into the $G_i$ factors uniquely through it.

The displayed limit is a [closed subgroup](../../../topological-group.md#closed-subgroup) of the [compact](../../../topology.md#compact-space) [Hausdorff](../../../topology.md#hausdorff-space) product of the [finite groups](../../../group.md#finite-group), and is [totally disconnected](../../../arithmetic.md#totally-disconnected-space), since two different tuples are separated by a [clopen](../../../topology.md#clopen-set) coordinate condition. Conversely a [compact](../../../topology.md#compact-space) [Hausdorff](../../../topology.md#hausdorff-space) [totally disconnected](../../../arithmetic.md#totally-disconnected-space) [group](../../../group.md) has a [neighbourhood basis](../../../topology.md#neighbourhood-basis) of [open normal subgroups](../../../topological-group.md#open-normal-subgroup). One way to see the [group](../../../group.md) part of this standard clopen-basis fact is to choose a [clopen](../../../topology.md#clopen-set) identity [neighbourhood](../../../topology.md#neighbourhood-mathematics) $U$ inside a prescribed [neighbourhood](../../../topology.md#neighbourhood-mathematics). [Compactness](../../../topology.md#compact-space) of $U$ and [continuity](../../../calculus.md#continuous-function) give a symmetric identity [neighbourhood](../../../topology.md#neighbourhood-mathematics) $V$ with $VU\subseteq U$. The stabilizer $H=\{g:gU=U\}$ contains $V$, is open, and is contained in $U$ because $1\in U$. Its index is finite by part (ii); its [normal core](../../../group-theory.md#core-group-theory) is the intersection of finitely many conjugates and is open and normal. The canonical map

$$
G\longrightarrow\varprojlim_{N\trianglelefteq_oG}G/N
$$

is [injective](../../../algebra.md#injective-function) because these $N$ separate points, and [surjective](../../../algebra.md#surjective-function) because compatible [cosets](../../../group-theory.md#coset) have the [finite intersection property](../../../topology.md#finite-intersection-property) and $G$ is [compact](../../../topology.md#compact-space). It is a [homeomorphism](../../../topology.md#homeomorphism) by [compactness](../../../topology.md#compact-space) and the [Hausdorff](../../../topology.md#hausdorff-space) property. This explains the equivalence of the two definitions.

The [profinite Frattini subgroup](../../../topological-group.md#profinite-frattini-subgroup) is $\Phi(G)=\bigcap M$, where $M$ ranges over all maximal proper [open subgroups](../../../topological-group.md#open-subgroup); for the trivial [group](../../../group.md) the empty intersection is $G$. For a [pro-p group](../../../topological-group.md#pro-p-group),

$$
\boxed{\Phi(G)=\overline{G^p[G,G]}.}
$$

Here powers and [group commutators](../../../group.md#group-commutator) mean generated [subgroups](../../../group.md#subgroup) and the bar supplies [closure](../../../topology.md#closure-topology). Every maximal [open subgroup](../../../topological-group.md#open-subgroup) in a [pro-p group](../../../topological-group.md#pro-p-group) is normal of index $p$, as follows by passing to the [finite p-group](../../../finite-group-theory.md#finite-p-group) quotient by its [normal core](../../../group-theory.md#core-group-theory). Such a [subgroup](../../../group.md#subgroup) therefore contains all powers and [group commutators](../../../group.md#group-commutator). Conversely the quotient by $D=\overline{G^p[G,G]}$ is an abelian [pro-p group](../../../topological-group.md#pro-p-group) of exponent $p$. If an element of this quotient is nontrivial, some finite [elementary abelian](../../../group.md#elementary-abelian-group) quotient detects it; a [linear functional](../../../linear-algebra.md#linear-functional) to $\mathbb F_p$ then detects it as well. Its [group homomorphism kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) pulls back to a maximal [open subgroup](../../../topological-group.md#open-subgroup) of $G$. Thus the intersection of these kernels is exactly $D$.

We also use the topological generation criterion: a subset generates $G$ topologically if and only if its image generates $G/\Phi(G)$ topologically. To prove the nontrivial direction, a proper closed generated [subgroup](../../../group.md#subgroup) $K$ lies in a proper [open subgroup](../../../topological-group.md#open-subgroup) $KN$ for a suitably small open normal $N$, and hence in a maximal [open subgroup](../../../topological-group.md#open-subgroup) obtained from the finite quotient $G/N$. Since that maximal [subgroup](../../../group.md#subgroup) contains $\Phi(G)$, the image of $K$ cannot generate the [Frattini quotient](../../../finite-group-theory.md#frattini-quotient).

Now suppose $G$ is a nontrivial procyclic [pro-p group](../../../topological-group.md#pro-p-group). If it had distinct maximal [open subgroups](../../../topological-group.md#open-subgroup) $M_1,M_2$, the [homomorphism](../../../algebra.md#homomorphism) to $C_p\times C_p$ induced by the two quotient maps would be onto: its projections are onto, and a proper such [subgroup](../../../group.md#subgroup) would be a one-dimensional graph, forcing the two kernels to coincide. Hence $G/(M_1\cap M_2)\cong C_p^2$, contradicting procyclicity. Thus there is exactly one maximal [open subgroup](../../../topological-group.md#open-subgroup) $M$, and $\Phi(G)=M$. Any $g\notin M$ generates $G/\Phi(G)\cong C_p$, so the criterion gives

$$
\boxed{G=\overline{\langle g\rangle}.}
$$

For the trivial [group](../../../group.md) use its identity as generator. **The additive [group](../../../group.md) $\mathbb Z_p$ is an infinite example**, topologically generated by $1$: its finite continuous quotients are cyclic $\mathbb Z/p^n\mathbb Z$.

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

If $H$ is an [open subgroup](../../../topological-group.md#open-subgroup), each left [coset](../../../group-theory.md#coset) $gH$ is open because left translation is a [homeomorphism](../../../topology.md#homeomorphism) in a [topological group](../../../topological-group.md). Its complement is the union of all the other [cosets](../../../group-theory.md#coset),

$$
G\setminus H=\bigcup_{g\notin H}gH.
$$

This is open, so **$H$ is closed**. No [compactness](../../../topology.md#compact-space) or separation assumption is required.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The left [cosets](../../../group-theory.md#coset) of an [open subgroup](../../../topological-group.md#open-subgroup) $H$ form an [open cover](../../../topology.md#open-cover) of the [compact group](../../../topological-group.md#compact-group). A finite subfamily therefore covers the [group](../../../group.md). Distinct [cosets](../../../group-theory.md#coset) are disjoint, so every [coset](../../../group-theory.md#coset) must occur in this finite subfamily. Hence **$[G:H]<\infty$**.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Suppose $(L,(\pi_i))$ and $(L',(\pi'_i))$ are [inverse limits](../../../module-theory.md#inverse-limit) of the same system, in the universal-property sense. The compatible family $(\pi'_i)$ induces a unique continuous [homomorphism](../../../algebra.md#homomorphism) $u:L'\to L$ with $\pi_i u=\pi'_i$; similarly there is a unique $v:L\to L'$ with $\pi'_i v=\pi_i$. Then $uv$ and $1_L$ both induce the projections $(\pi_i)$, so uniqueness gives $uv=1_L$. Likewise $vu=1_{L'}$. Thus **the limits are uniquely isomorphic by an [isomorphism](../../../algebra.md#isomorphism) preserving every projection**. In particular the inverse maps are continuous, so this is an [isomorphism](../../../algebra.md#isomorphism) of [topological groups](../../../topological-group.md), not just abstract [groups](../../../group.md).

## 2

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For odd $p$, a [subgroup](../../../group.md#subgroup) $N$ is [powerfully embedded](../../../finite-group-theory.md#powerfully-embedded-subgroup) in $G$ if $[N,G]\le N^p$, where $N^p=\langle n^p:n\in N\rangle$. The condition implies normality since $n^g=n[n,g]\in N$. The [group](../../../group.md) $G$ is a [powerful p-group](../../../finite-group-theory.md#powerful-p-group) if $[G,G]\le G^p$, equivalently if $G$ itself is [powerfully embedded](../../../finite-group-theory.md#powerfully-embedded-subgroup). For a [finite p-group](../../../finite-group-theory.md#finite-p-group), the [Burnside basis theorem](../../../finite-group-theory.md#burnside-basis-theorem) gives $d(Q)=\dim_{\mathbb F_p}Q/\Phi(Q)$, and $\Phi(Q)=Q^p[Q,Q]$. Thus for powerful $Q$, $d(Q)=\dim Q/Q^p$.

We prove $d(H)\le d(G)$ by induction on $|G|$, with the trivial [group](../../../group.md) immediate. The supplied embedding result applied to $N=G$ makes $G^p$ [powerfully embedded](../../../finite-group-theory.md#powerfully-embedded-subgroup), and hence powerful. It is a proper [subgroup](../../../group.md#subgroup) when $G\ne1$, because $G^p=\Phi(G)$ is proper in a nontrivial [finite p-group](../../../finite-group-theory.md#finite-p-group). Set

$$
K=H\cap G^p,\quad V=G/G^p,\quad W=G^p/G^{p^2},\quad A=HG^p/G^p\le V.
$$

All the displayed quotients are [elementary abelian](../../../group.md#elementary-abelian-group). The supplied onto [homomorphism](../../../algebra.md#homomorphism) $\theta:V\to W$, $xG^p\mapsto x^pG^{p^2}$, is therefore linear. Write $v=\dim V=d(G)$, $w=\dim W=d(G^p)$, $r=\dim A$, and $t=\dim\theta(A)$.

Since $H/K$ embeds in $V$, $\Phi(H)\le K$. Also

$$
\Phi(K)\le\Phi(H),\qquad\Phi(K)=K^p[K,K]\le(G^p)^p[G^p,G^p]=G^{p^2}.
$$

Here $(G^p)^p=G^{p^2}$ is the iterated-power convention, valid for powerful [groups](../../../group.md). Hence the natural map $K/\Phi(K)\to W$ is defined. The image under this map of the subspace $\Phi(H)/\Phi(K)$ contains $\theta(A)$, because for every $h\in H$ its power $h^p$ lies in $\Phi(H)\cap K$. It follows that

$$
\dim K/\Phi(H)\le d(K)-t.
$$

The [exact sequence](../../../homology.md#exact-sequence) $1\to K/\Phi(H)\to H/\Phi(H)\to H/K\to1$ consists of [elementary abelian groups](../../../group.md#elementary-abelian-group), and $\dim H/K=r$. By induction inside $G^p$, $d(K)\le d(G^p)=w$. Therefore

$$
d(H)=r+\dim K/\Phi(H)\le r+w-t=w+\dim\ker(\theta|_A)\le w+\dim\ker\theta=v.
$$

This proves **$d(H)\le d(G)$**, including [subgroups](../../../group.md#subgroup) $H$ that are not themselves powerful.

The [rank of a profinite group](../../../topological-group.md#rank-of-a-profinite-group) is $\operatorname{rk}(P)=\sup\{d(K):K\le P\text{ closed}\}$, where $d(K)$ is its least topological generator number. If $P$ has finite rank then every [closed subgroup](../../../topological-group.md#closed-subgroup), including the [open subgroup](../../../topological-group.md#open-subgroup) $H$, has no larger rank. Conversely suppose $H$ has rank $r<\infty$. Its [normal core](../../../group-theory.md#core-group-theory) $C=\bigcap_{g\in P}H^g$ is an [open normal subgroup](../../../topological-group.md#open-normal-subgroup): there are finitely many conjugates because $H$ has finite index. It has rank at most $r$.

For every closed $K\le P$, the [subgroup](../../../group.md#subgroup) $K\cap C$ is normal in $K$ and has at most $r$ topological generators. The quotient $K/(K\cap C)$ embeds in the [finite group](../../../group.md#finite-group) $P/C$. A [finite group](../../../group.md#finite-group) of order at most $M=[P:C]$ has at most $\lfloor\log_2M\rfloor$ generators: in a minimal sequential generating list every strict enlargement at least doubles the [subgroup](../../../group.md#subgroup) order. Lift such quotient generators and adjoin generators of $K\cap C$. Their closed generated [subgroup](../../../group.md#subgroup) contains the [group homomorphism kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) and maps onto the quotient, so equals $K$. Consequently

$$
\boxed{\operatorname{rk}(P)\le r+\lfloor\log_2[P:C]\rfloor<\infty.}
$$

Thus **an [open subgroup](../../../topological-group.md#open-subgroup) has finite rank exactly when the whole [profinite group](../../../topological-group.md#profinite-group) does**.

## 3

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a [pro-p group](../../../topological-group.md#pro-p-group), the [lower p-series](../../../finite-group-theory.md#lower-p-series) is the descending sequence of closed [characteristic subgroups](../../../algebra.md#characteristic-subgroup)

$$
\boxed{P_1(G)=G,\qquad P_{i+1}(G)=\overline{P_i(G)^p[P_i(G),G]}.}
$$

The bar means [closure](../../../topology.md#closure-topology) of the [subgroup](../../../group.md#subgroup) generated by the displayed powers and [group commutators](../../../group.md#group-commutator). Throughout this question $p$ is odd. For a finitely generated [powerful pro-p group](../../../topological-group.md#powerful-pro-p-group), [group commutator](../../../group.md#group-commutator) collection gives $P_i(G)=G^{p^{i-1}}$, each $P_i$ is powerful, and $\Phi(P_i)=P_{i+1}$. All these [subgroups](../../../group.md#subgroup) are open. A [uniform pro-p group](../../../topological-group.md#uniform-pro-p-group) is such a [group](../../../group.md) with all [subgroup](../../../group.md#subgroup) indices $[P_i:P_{i+1}]$ equal to $[G:P_2]$. We use the standard powerful-group torsion criterion: a finitely generated [powerful pro-p group](../../../topological-group.md#powerful-pro-p-group) is uniform exactly when it is a [torsion-free group](../../../group.md#torsion-free-group). For a uniform [group](../../../group.md) of generator number $d$, the indices are $p^d$, and $x\mapsto x^{p^a}$ is a [homeomorphism](../../../topology.md#homeomorphism) from $G$ onto $G^{p^a}$.

We record explicitly the collection facts used for the operations below. With $U_b=G^{p^b}=P_{b+1}$, one has

$$
[U_a,U_b]\le U_{a+b+1},\qquad x\equiv y\pmod{U_b}\ \Longleftrightarrow\ x^{p^a}\equiv y^{p^a}\pmod{U_{a+b}}.
$$

The second statement is the power-congruence property: the $p$th-power map is an [isomorphism](../../../algebra.md#isomorphism) on adjacent uniform layers, and collection gives $(yu)^p\equiv y^pu^p\pmod{U_{b+2}}$ for $u\in U_b$. Thus the first nonzero layer of a difference moves down exactly one step under a $p$th power. Iterating gives the asserted equivalence and also justifies taking roots of congruences. These facts follow from powerful-group [group commutator](../../../group.md#group-commutator) collection, using divisibility by $p$ of $\binom p2$ and the successive-layer power isomorphisms; they are the uniform-group structure results being used here.

The [transported addition on a uniform pro-p group](../../../topological-group.md#transported-addition-on-a-uniform-pro-p-group) is

$$
\boxed{x+_ny=(x^{p^n}y^{p^n})^{p^{-n}}\qquad(n\ge1).}
$$

The product is in $U_n$ and has a unique $p^n$th root in $G$. For the comparison at $n=1$ define $x+_0y=xy$. The numbered proofs below establish [associativity](../../../group.md#associative-property), approximate [commutativity](../../../algebra.md#commutativity) and compatibility of these operations.

The intrinsic [Lie algebra of a uniform pro-p group](../../../lie-algebra.md#lie-algebra-of-a-uniform-pro-p-group) has underlying set $G$, zero equal to the [group](../../../group.md) identity, additive inverse $x^{-1}$, and operations

$$
\boxed{x+_Ly=\lim_{n\to\infty}(x^{p^n}y^{p^n})^{p^{-n}},\qquad [x,y]_L=\lim_{n\to\infty}[x^{p^n},y^{p^n}]^{p^{-2n}},\qquad \lambda x=x^\lambda\ (\lambda\in\mathbb Z_p).}
$$

Here the [group commutator](../../../group.md#group-commutator) is $[x,y]=x^{-1}y^{-1}xy$. For $\lambda\in\mathbb Z_p$, $x^\lambda$ is the limit of $x^{m_j}$ for integers $m_j\to\lambda$; the pro-$p$ [topology](../../../topology.md) makes it well defined. The addition sequence is [Cauchy](../../../real-analysis.md#cauchy-sequence) by the compatibility proved below. The [group commutator](../../../group.md#group-commutator) estimate puts $[x^{p^n},y^{p^n}]$ in $U_{2n+1}$, so its displayed root exists and lies in $U_1$. Collection of [group commutators](../../../group.md#group-commutator) shows that successive bracket approximants differ in layers tending to the identity, giving the other limit. The [group commutator](../../../group.md#group-commutator) identities give additivity of the limiting bracket, and the [Hall-Witt identity](../../../group.md#hall-witt-identity) gives its [Jacobi identity](../../../lie-algebra.md#jacobi-identity). Approximate [commutativity](../../../algebra.md#commutativity) makes limiting addition [commutative](../../../algebra.md#commutativity). The resulting lattice $L_G$ is a [free module](../../../module-theory.md#free-module) over $\mathbb Z_p$ of rank $d(G)$, and $[L_G,L_G]\le pL_G$.

A [powerful Lie algebra over p-adic integers](../../../lie-algebra.md#powerful-lie-algebra-over-p-adic-integers), in the convention relevant here, is a [Lie algebra](../../../lie-algebra.md) $L$ whose underlying [module](../../../module-theory.md#module-mathematics) is finite free over $\mathbb Z_p$ and whose bracket satisfies $[L,L]\le pL$. For $p=2$ the condition is instead $[L,L]\le4L$. For odd $p$, define multiplication on its underlying set by the convergent [Baker--Campbell--Hausdorff formula](../../../linear-operator-theory.md#baker-campbell-hausdorff-formula)

$$
x*y=\operatorname{BCH}(x,y)=x+y+\frac12[x,y]+\frac1{12}\bigl([x,[x,y]]+[y,[y,x]]\bigr)+\cdots.
$$

An iterated bracket of degree $m$ lies in $p^{m-1}L$. The BCH coefficient bound loses at most $\lfloor(m-1)/(p-1)\rfloor$ powers of $p$, so all higher-degree terms are integral, and their valuations tend to infinity. This explains both convergence and why multiplying a lattice with small bracket stays inside the lattice. Formal [associativity](../../../group.md#associative-property) of BCH passes to the convergent series, the identity is $0$, the inverse is $-x$, and every [group](../../../group.md) power satisfies $x^{*m}=mx$. The quotients by $p^aL$ are [finite p-groups](../../../finite-group-theory.md#finite-p-group). Hence the resulting [compact group](../../../topological-group.md#compact-group) is a finitely generated [torsion-free group](../../../group.md#torsion-free-group) and a [pro-p group](../../../topological-group.md#pro-p-group), and its [group commutator](../../../group.md#group-commutator) lies in $pL$. Thus **$(L,*)$ is a [uniform pro-p group](../../../topological-group.md#uniform-pro-p-group)**, with $P_i(L,*)=p^{i-1}L$ and successive index $p^{\operatorname{rank}_{\mathbb Z_p}L}$.

The standard uniform-group/Lie-lattice correspondence identifies these constructions as mutually inverse: **$L_{(L,*)}\cong L$ and $(L_G,*)\cong G$**. To see why the [inverse limits](../../../module-theory.md#inverse-limit) recover the lattice operations, the addition approximant for a BCH [group](../../../group.md) is $p^{-n}\operatorname{BCH}(p^nx,p^ny)$: its linear term is $x+y$ and every higher term tends to zero. Similarly its [group commutator](../../../group.md#group-commutator) approximant has limiting term $[x,y]$. In the other direction, a local [logarithm](../../../calculus.md#logarithm) in the complete normed [group algebra](../../../associative-algebra.md#group-algebra) identifies the intrinsic operations with algebra addition and [commutator](../../../lie-algebra.md#commutator) and identifies [group](../../../group.md) multiplication with BCH; the uniform power maps extend the identification from a sufficiently small power [subgroup](../../../group.md#subgroup) to all of $G$. Continuous [group homomorphisms](../../../group-theory.md#group-homomorphism) respect powers, unique roots and limits, while [Lie algebra homomorphisms](../../../lie-algebra.md#lie-algebra-homomorphism) respect every BCH term, so the equivalence also preserves morphisms.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For a [powerful pro-p group](../../../topological-group.md#powerful-pro-p-group), $\Phi(P_i)=P_{i+1}$. The [Burnside basis theorem](../../../finite-group-theory.md#burnside-basis-theorem) therefore gives

$$
d(P_i)=\dim_{\mathbb F_p}P_i/P_{i+1}=\log_p[P_i:P_{i+1}].
$$

If $G$ is uniform, all these indices equal $[G:P_2]=p^{d(G)}$. Hence **$d(P_i)=d(G)$ for every $i\ge1$**, proving (i)$\Rightarrow$(ii).

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Conversely, if all $d(P_i)$ equal $d(G)$, the same Frattini-quotient identity gives $[P_i:P_{i+1}]=p^{d(G)}$ for every $i$. This is exactly the index definition of a [uniform pro-p group](../../../topological-group.md#uniform-pro-p-group). Thus **(ii)$\Rightarrow$(i)**, completing the equivalence of the first two conditions.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Suppose first that $G$ is uniform and $H$ is a powerful [open subgroup](../../../topological-group.md#open-subgroup). The torsion criterion stated above makes $G$ a [torsion-free group](../../../group.md#torsion-free-group); so $H$ is a [torsion-free group](../../../group.md#torsion-free-group) too. It is finitely generated, for example by the [Schreier lemma](../../../geometric-group-theory.md#reidemeister-schreier-theorem), and hence is uniform by the same criterion. Put $d=d(G)$ and $e=d(H)$, and choose $k$ with $P_k(G)\le H$. For every $n\ge0$,

$$
P_{n+k}(G)\le H^{p^n}\le G^{p^n}=P_{n+1}(G).
$$

Uniformity of the two [groups](../../../group.md) gives

$$
p^{nd}\le [G:H^{p^n}]=[G:H]p^{ne}\le p^{(n+k-1)d}.
$$

Taking logarithms and dividing by $n$, then letting $n\to\infty$, proves $e=d$. This proves (i)$\Rightarrow$(iii) without assuming that $H$ is a power [subgroup](../../../group.md#subgroup). Conversely every $P_i(G)$ is powerful and open, so (iii) applied to these [subgroups](../../../group.md#subgroup) gives (ii). Therefore **all three conditions are equivalent**.

The remaining nested parts establish the stated properties of the transported operations $+_n$ defined in the root solution.

<h4 id="3/iii/i">i</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/i/solution">Solution</h5>

↑ **Parent:** [I](#3/iii/i)

The map $\sigma_n:G\to U_n$, $x\mapsto x^{p^n}$, is a [bijection](../../../function.md#bijection), and the operation $+_n$ is exactly multiplication transported through it. Explicitly,

$$
\begin{aligned}
((x+_ny)+_nz)^{p^n}&=x^{p^n}y^{p^n}z^{p^n},\\
(x+_n(y+_nz))^{p^n}&=x^{p^n}y^{p^n}z^{p^n}.
\end{aligned}
$$

[Injectivity](../../../algebra.md#injective-function) of $\sigma_n$ proves **$(x+_ny)+_nz=x+_n(y+_nz)$**. The approximate operation need not be [commutative](../../../algebra.md#commutativity); its [associativity](../../../group.md#associative-property) is exact.

<h4 id="3/iii/ii">ii</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/iii/ii)

The uniform [group commutator](../../../group.md#group-commutator) estimate gives

$$
[x^{p^n},y^{p^n}]\in[U_n,U_n]\le U_{2n+1}.
$$

Thus $x^{p^n}y^{p^n}$ and $y^{p^n}x^{p^n}$ are congruent modulo $U_{2n+1}$. Taking their unique $p^n$th roots and using the power-congruence property moves the error layer back by $n$, giving

$$
\boxed{x+_ny\equiv y+_nx\pmod{P_{n+2}(G)=U_{n+1}}.}
$$

<h4 id="3/iii/iii">iii</h4>

↑ **Parent:** [Iii](#3/iii)

<h5 id="3/iii/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/iii/iii)

Put $a=x^{p^{n-1}}$ and $b=y^{p^{n-1}}$, both in $U_{n-1}$. The collection formula gives

$$
(ab)^p\equiv a^pb^p\pmod{U_{2n}}.
$$

Indeed the weight-two [group commutator](../../../group.md#group-commutator) lies in $[U_{n-1},U_{n-1}]\le U_{2n-1}$, and its coefficient $\binom p2$ is divisible by $p$ since $p$ is odd, moving it into $U_{2n}$. A [group commutator](../../../group.md#group-commutator) of weight $j\ge3$ in $a,b$ lies in $U_{jn-1}\le U_{2n}$; all higher terms are therefore harmless as well. This also covers $n=1$.

Let $v=x+_{n-1}y$ and $u=x+_ny$. Their powers satisfy $v^{p^n}=(ab)^p$ and $u^{p^n}=a^pb^p$. Taking $p^n$th roots of the collected congruence gives $u\equiv v\pmod{U_n}$. Since $U_n=P_{n+1}\le P_n$, this proves the requested, slightly weaker, result

$$
\boxed{x+_ny\equiv x+_{n-1}y\pmod{P_n(G)}.}
$$

For $n=1$ the definition $+_0=$ ordinary multiplication makes the comparison meaningful.

## 4

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The objective is a continuous [faithful representation](../../../representation-theory.md#faithful-representation) of a [uniform pro-p group](../../../topological-group.md#uniform-pro-p-group) $G$ in some $\operatorname{GL}_N(\mathbb Z_p)$. The proof proceeds from the intrinsic Lie lattice to a small [matrix group](../../../group-theory.md#matrix-group), then extends the resulting representation to all of $G$. This last step matters: a representation defined only on an [open subgroup](../../../topological-group.md#open-subgroup) does not yet establish linearity of the original [group](../../../group.md).

Let $L=L_G$ be the [Lie algebra of a uniform pro-p group](../../../lie-algebra.md#lie-algebra-of-a-uniform-pro-p-group) and put $\mathfrak g=\mathbb Q_p\otimes_{\mathbb Z_p}L$. The uniform-group/Lie-lattice correspondence identifies the [group](../../../group.md) law on $L$ with BCH. The substantial finite-dimensional Lie-theoretic input is the [Ado theorem](../../../lie-algebra.md#ado-s-theorem): every finite-dimensional [Lie algebra](../../../lie-algebra.md) over a characteristic-zero [field](../../../algebra.md#field) admits a faithful finite-dimensional representation. Apply it to obtain

$$
\rho:\mathfrak g\hookrightarrow\operatorname{End}_{\mathbb Q_p}(V),\qquad\rho([x,y])=\rho(x)\rho(y)-\rho(y)\rho(x).
$$

An [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) would not suffice here, since it kills the centre; Ado supplies [injectivity](../../../algebra.md#injective-function) even in central directions.

Choose a [p-adic lattice](../../../arithmetic.md#integral-lattice-in-a-p-adic-vector-space) $\Lambda$ spanning $V$. Since $L$ has finitely many lattice generators, their representing [matrices](../../../vector-space.md#matrix) have bounded denominators. There is therefore an integer $a\ge0$ such that

$$
\rho(p^aL)\subseteq p^\epsilon\operatorname{End}_{\mathbb Z_p}(\Lambda),\qquad\epsilon=\begin{cases}1,&p\ne2,\\2,&p=2.\end{cases}
$$

On this [matrix](../../../vector-space.md#matrix) lattice the series $\exp X=\sum_{n\ge0}X^n/n!$ and $\log(1+Y)=\sum_{n\ge1}(-1)^{n+1}Y^n/n$ converge and are inverse. For example $v_p(n!)\le n/(p-1)$, so the valuations of the exponential terms tend to infinity with this choice of $\epsilon$; the [logarithm](../../../calculus.md#logarithm) terms do as well. They take values in $1+p^\epsilon\operatorname{End}(\Lambda)$ and in $p^\epsilon\operatorname{End}(\Lambda)$ respectively. The formal identity $\exp(\operatorname{BCH}(X,Y))=\exp X\exp Y$ holds for the convergent series.

Under the correspondence, $U=G^{p^a}$ has Lie lattice $p^aL$ and is an open [characteristic subgroup](../../../algebra.md#characteristic-subgroup). Define

$$
\eta:U\longrightarrow\operatorname{GL}(\Lambda),\qquad\eta(u)=\exp(\rho(\log_Gu)),
$$

where $\log_G$ denotes the identification of $U$ with $p^aL$. A Lie [homomorphism](../../../algebra.md#homomorphism) preserves BCH, so the exponential identity proves $\eta(uv)=\eta(u)\eta(v)$. If $\eta(u)=I$, the [matrix](../../../vector-space.md#matrix) [logarithm](../../../calculus.md#logarithm) gives $\rho(\log_Gu)=0$; faithfulness of $\rho$ gives $u=1$. Thus $\eta$ is a continuous faithful integral representation of $U$.

To extend it, take the [module](../../../module-theory.md#module-mathematics)

$$
W=\{f:G\to\Lambda:f(ux)=\eta(u)f(x)\text{ for all }u\in U,\ x\in G\}.
$$

Values on a transversal of $U\backslash G$ determine $f$, so $W$ is a [free module](../../../module-theory.md#free-module) over $\mathbb Z_p$ of rank $[G:U]\dim V$. These functions are continuous, since on each open [coset](../../../group-theory.md#coset) they are given by the continuous representation $\eta$. Define $(T_gf)(x)=f(xg)$. The equivariance condition is preserved, and $T_gT_h=T_{gh}$. In a transversal [basis](../../../vector-space.md#basis) each $T_g$ is a permutation of blocks followed by [matrices](../../../vector-space.md#matrix) from $\eta(U)$, so it belongs to $\operatorname{GL}(W)$ and depends continuously on $g$.

Faithfulness can be checked directly. If $g\notin U$, right multiplication moves the [coset](../../../group-theory.md#coset) $U$ to a different [coset](../../../group-theory.md#coset), so $T_g$ moves a function supported on one block and cannot be the identity. If $g\in U$ and $T_g=1$, evaluation at $1$ gives $f(g)=f(1)$ for every $f$, whereas equivariance gives $f(g)=\eta(g)f(1)$. Since $f(1)$ is arbitrary, $\eta(g)=I$, and hence $g=1$. Therefore

$$
\boxed{G\hookrightarrow\operatorname{GL}_{[G:U]\dim V}(\mathbb Z_p).}
$$

[Compactness](../../../topology.md#compact-space) of $G$ makes this continuous injection a [homeomorphism](../../../topology.md#homeomorphism) onto its closed image. This proves the [linearity of a uniform pro-p group](../../../topological-group.md#linearity-of-a-uniform-pro-p-group) for the full [group](../../../group.md), including its centre, and explains why taking a sufficiently small power lattice permits [matrix](../../../vector-space.md#matrix) integration before finite-index induction restores the whole [group](../../../group.md).

## 5

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Write $k=\mathbb F_p$. The [Nottingham group](../../../topological-group.md#nottingham-group) $\mathcal N$ is the set of formal series $f(t)=t+\sum_{i\ge2}a_it^i$ over $k$, with ordinary composition $f\circ g$ as multiplication and the $t$-adic [topology](../../../topology.md). The identity is $t$. A compositional inverse exists uniquely by solving its coefficients successively, since the linear coefficient is $1$.

Equivalently $\mathcal N$ is the [group](../../../group.md) of continuous $k$-automorphisms of $k((t))$ whose action on $(t)/(t^2)$ is the identity. Such an automorphism is determined by the image of $t$, which is $t+O(t^2)$. To identify this with ordinary series composition without reversing multiplication, send $f$ to the automorphism $h(t)\mapsto h(f^{-1}(t))$. Its composite with the automorphism for $g$ is the one for $f\circ g$.

The depth filtration is

$$
\mathcal N_m=\{f:f(t)\equiv t\pmod{t^{m+1}}\},\qquad m\ge1.
$$

Each $\mathcal N_m$ is open and normal, and the coefficient of $t^{m+1}$ identifies $\mathcal N_m/\mathcal N_{m+1}$ with $(k,+)$. Thus $[\mathcal N:\mathcal N_m]=p^{m-1}$, and $\mathcal N$ is the [inverse limit](../../../module-theory.md#inverse-limit) of its [finite p-group](../../../finite-group-theory.md#finite-p-group) truncations.

Here is a local-field proof that **every [finite p-group](../../../finite-group-theory.md#finite-p-group) embeds in $\mathcal N$**. We first establish the realization step rather than assume the Nottingham embedding itself. Put $F=k((t))$ and $\Gamma=\operatorname{Gal}(F^{\mathrm{sep}}/F)$, and let $I\trianglelefteq\Gamma$ be the inertia [subgroup](../../../group.md#subgroup), the [group homomorphism kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) of the action on the [algebraic closure](../../../algebra.md#algebraic-closure) of the [residue field](../../../commutative-algebra.md#residue-field). We use the standard additive [normal basis theorem](../../../galois-theory.md#normal-basis-theorem) consequence $H^j(\Gamma,F^{\mathrm{sep}})=0$ for $j>0$. It follows by taking direct limits of the finite-Galois normal-basis [modules](../../../module-theory.md#module-mathematics), whose additive [cohomology](../../../cohomology.md) vanishes. The Artin-Schreier sequence

$$
0\longrightarrow\mathbb F_p\longrightarrow F^{\mathrm{sep}}\xrightarrow{z\mapsto z^p-z}F^{\mathrm{sep}}\longrightarrow0
$$

then gives

$$
H^1(\Gamma,\mathbb F_p)=F/\{z^p-z:z\in F\},\qquad H^2(\Gamma,\mathbb F_p)=0.
$$

The classes $t^{-m}$ for positive $m$ prime to $p$ are [linearly independent](../../../vector-space.md#linear-independence): a nonzero finite linear combination has a most negative [valuation](../../../algebra.md#valuation) prime to $p$, whereas a negative [valuation](../../../algebra.md#valuation) of $z^p-z$ is divisible by $p$. Thus there are infinitely many independent continuous characters $\Gamma\to C_p$.

Induct on the order of a [finite p-group](../../../finite-group-theory.md#finite-p-group) $E$. Choose a central [subgroup](../../../group.md#subgroup) $C\cong C_p$ and put $Q=E/C$. By induction there is an onto map $\phi:\Gamma\to Q$ with $\phi(I)=Q$, corresponding to a [totally ramified](../../../arithmetic.md#totally-ramified-extension) $Q$-extension. The central extension $1\to C\to E\to Q\to1$ is specified by a [two-cocycle](../../../group-theory.md#two-cocycle). Its pullback along $\phi$ is a [coboundary](../../../algebra.md#coboundary) because $H^2(\Gamma,\mathbb F_p)=0$. Correcting a set-theoretic section by that [coboundary](../../../algebra.md#coboundary) gives a continuous [homomorphism](../../../algebra.md#homomorphism) $\rho_0:\Gamma\to E$ lifting $\phi$.

We must make the lift onto on inertia, not merely onto on the whole [Galois group](../../../galois-theory.md#galois-group). Let $A=I\cap\ker\phi$. On $A$, the lift $\rho_0$ takes values in $C$. Characters vanishing on $A$ form a finite-dimensional space: $\Gamma/A$ has a finite [subgroup](../../../group.md#subgroup) $I/A\cong Q$ and procyclic quotient $\Gamma/I\cong\widehat{\mathbb Z}$, so a character is determined by finitely many values on generators of these two pieces. The infinite-dimensional character space therefore has infinitely many distinct restrictions to $A$. Choose a character $\chi:\Gamma\to C$ whose restriction to $A$ does not cancel $\rho_0|_A$, and set $\rho(\gamma)=\chi(\gamma)\rho_0(\gamma)$. Centrality of $C$ makes this another [homomorphism](../../../algebra.md#homomorphism) lifting $\phi$. Its image on $A$ is nontrivial and hence all of $C$, while its image on $I$ maps onto $Q$. Therefore $\rho(I)=E$. The fixed [field](../../../algebra.md#field) of $\ker\rho$ is the required [totally ramified](../../../arithmetic.md#totally-ramified-extension) finite [Galois extension](../../../galois-theory.md#finite-galois-extension) $K/F$ with [group](../../../group.md) $E$. This proves the realization step for every [finite p-group](../../../finite-group-theory.md#finite-p-group).

Since the [residue field](../../../commutative-algebra.md#residue-field) of $K$ is still $k$, choosing a [uniformizer](../../../commutative-algebra.md#uniformizer) $u$ identifies $K$ with $k((u))$. Indeed successive subtraction of its residue coefficient and division by $u$ gives each element of its [valuation ring](../../../commutative-algebra.md#valuation-ring) a unique convergent expansion $\sum_{i\ge0}b_iu^i$ with $b_i\in k$, and fractions give the Laurent expansions. Each element of $E$ preserves the [valuation](../../../algebra.md#valuation) and fixes $k$, so sends $u$ to $a_1u+a_2u^2+\cdots$. The linear coefficient is a [homomorphism](../../../algebra.md#homomorphism) $E\to k^\times$. Since $E$ is a $p$-group and $|k^\times|=p-1$, that [homomorphism](../../../algebra.md#homomorphism) is trivial. Thus the faithful Galois action lies in $\mathcal N(k)$, completing the embedding proof.

An infinite [profinite group](../../../topological-group.md#profinite-group) is [hereditarily just infinite](../../../topological-group.md#hereditarily-just-infinite-profinite-group) when every [open subgroup](../../../topological-group.md#open-subgroup) is infinite and every nontrivial closed [normal subgroup](../../../group-theory.md#normal-subgroup) of each such [open subgroup](../../../topological-group.md#open-subgroup) is open. We sketch the normal-subgroup argument, giving the depth calculation in odd characteristic explicitly. For series of depths $r,s$,

$$
f=t+at^{r+1}+\cdots,\quad g=t+bt^{s+1}+\cdots\quad\Longrightarrow\quad[f,g]=t+ab(r-s)t^{r+s+1}+O(t^{r+s+2}),
$$

where $[f,g]=f^{-1}\circ g^{-1}\circ f\circ g$. The coefficient follows by comparing $f\circ g$ and $g\circ f$ in degree $r+s+1$: their cross terms are $ab(r+1)$ and $ab(s+1)$.

Let $H$ be open and $1\ne K\trianglelefteq H$ closed. Choose $m$ with $\mathcal N_m\le H$ and choose $f\in K$ of depth $r$. For every $j\ge m$ with $j\not\equiv r\pmod p$, commutation with $t+bt^{j+1}$ supplies an element of $K$ of depth $r+j$, with any prescribed nonzero [leading coefficient](../../../polynomial.md#leading-coefficient-of-a-polynomial) by varying $b$. Thus every sufficiently high layer except possibly depths congruent to $2r$ modulo $p$ occurs in $K$.

When $p$ is odd, choose one available depth $u\ge r+m$ with $u\not\equiv2r,r\pmod p$. Such a residue exists even for $p=3$. An element $h\in K$ of that depth can be commuted with $t+bt^{k-u+1}$ for every sufficiently large missing depth $k\equiv2r\pmod p$. The new [leading coefficient](../../../polynomial.md#leading-coefficient-of-a-polynomial) contains $2u-k\equiv2(u-r)\ne0$, so those missing layers occur too. Hence $K$ contains an element with any chosen coefficient in every depth $k\ge M$, for some $M$.

Successive coefficient correction now proves $\mathcal N_M\le K$: match the coefficient of an arbitrary target in depth $M$ by an element of $K$, correct the error in depth $M+1$, and continue. The partial products converge $t$-adically to the target and remain in $K$, which is closed. Thus $K$ is open. This proves hereditary just infiniteness for odd $p$.

For characteristic two, the [leading coefficient](../../../polynomial.md#leading-coefficient-of-a-polynomial) alone misses even depths. The standard characteristic-two normal-closure collection lemma supplies the needed extra input: for every $m\ge1$ and every nonidentity $f\in\mathcal N(\mathbb F_2)$, the [closed subgroup](../../../topological-group.md#closed-subgroup) generated by the conjugates $f^g$ with $g\in\mathcal N_m$ contains $\mathcal N_M$ for some $M$. Its proof retains the next coefficients in pairs of [group commutators](../../../group.md#group-commutator) to fill the parity gaps, then uses the same successive coefficient correction. Apply this lemma to $f\in K$ and $\mathcal N_m\le H$: every such conjugate lies in $K$, so $K$ contains the tail and is open. This states the additional collection result used in the characteristic-two sketch; the odd-prime leading-term argument is not being applied there. Since every [open subgroup](../../../topological-group.md#open-subgroup) contains a tail and is infinite, **the [Nottingham group](../../../topological-group.md#nottingham-group) is [hereditarily just infinite](../../../topological-group.md#hereditarily-just-infinite-profinite-group) for every prime $p$**.

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

The first alternative in the supplied analytic-group theorem would give a [faithful representation](../../../representation-theory.md#faithful-representation) of $\mathcal N$ in some $\operatorname{GL}_d(\mathbb Z_p)$ or $\operatorname{GL}_d(\mathbb F_p[[t]])$. The embedding proved above supplies cyclic [subgroups](../../../group.md#subgroup) of order $p^a$ for arbitrarily large $a$. Such orders are impossible in either fixed [matrix](../../../vector-space.md#matrix) [dimension](../../../vector-space.md#dimension-vector-space).

In [characteristic zero](../../../algebra.md#characteristic-zero), a [matrix](../../../vector-space.md#matrix) $A$ of order $p^a$ is diagonalizable over an algebraic [closure](../../../topology.md#closure-topology), because its [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) divides the [separable polynomial](../../../galois-theory.md#separable-polynomial) $X^{p^a}-1$. At least one [eigenvalue](../../../linear-operator-theory.md#eigenvalue) must be a primitive $p^a$th [root of unity](../../../algebra.md#root-of-unity); otherwise $A^{p^{a-1}}=I$. The [cyclotomic polynomial](../../../galois-theory.md#cyclotomic-polynomial) $\Phi_{p^a}$ is irreducible over $\mathbb Q_p$, since $\Phi_{p^a}(1+X)$ satisfies the [Eisenstein criterion](../../../commutative-algebra.md#eisenstein-criterion) at $p$. Consequently that [eigenvalue](../../../linear-operator-theory.md#eigenvalue) has degree $\varphi(p^a)=p^{a-1}(p-1)$ over $\mathbb Q_p$, which must be at most the [matrix](../../../vector-space.md#matrix) [dimension](../../../vector-space.md#dimension-vector-space) $d$. This bounds $a$.

In characteristic $p$, pass from the power-series ring to its fraction [field](../../../algebra.md#field). A [matrix](../../../vector-space.md#matrix) of $p$-power order satisfies $X^{p^a}-1=(X-1)^{p^a}$, so it is unipotent. Writing $A=I+B$, nilpotence gives $B^d=0$. For $p^e\ge d$,

$$
A^{p^e}=I+B^{p^e}=I.
$$

Thus its order is at most $p^{\lceil\log_pd\rceil}$, again a fixed bound. Therefore **the linear alternative is impossible** in both coefficient rings.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

We next bound the closed [derived series](../../../group-theory.md#derived-series). For odd $p$, the depth calculation yields

$$
[\mathcal N_m,\mathcal N_m]=\mathcal N_{2m+1}.
$$

For the inclusion from left to right, two series of depth at least $m$ commute modulo $\mathcal N_{2m+1}$: at depth $2m$ the only possible leading pair has equal depths and its coefficient vanishes. For the reverse inclusion, every depth $k\ge2m+1$ can be written $r+s=k$ with $r,s\ge m$ and $r\not\equiv s\pmod p$. Start with $r=m,s=k-m$; if their difference vanishes modulo $p$, replace them by $r=m+1,s=k-m-1$, which is allowed except at $k=2m+1$, where the original difference is already nonzero. The difference changes by $2$, nonzero for odd $p$. [Commutators](../../../lie-algebra.md#commutator) thus supply every high [leading coefficient](../../../polynomial.md#leading-coefficient-of-a-polynomial), and closed successive coefficient correction fills the tail.

With $\mathcal N^{(0)}=\mathcal N_1$, induction on $n$ gives

$$
\mathcal N^{(n)}=\mathcal N_{2^{n+1}-1},\qquad\log_p[\mathcal N:\mathcal N^{(n)}]=2^{n+1}-2.
$$

For $p=2$ use the standard characteristic-two derived-series collection bound, explicitly stated as an additional result:

$$
\log_2[\mathcal N:\mathcal N^{(n)}]\le C\kappa^n,\qquad\kappa=\frac{1+\sqrt{17}}2<3,
$$

for a fixed constant $C$. One can take a fixed enlarged constant from the tail estimate $\mathcal N^{(n)}\supseteq\mathcal N_{\lceil4\kappa^n\rceil+1}$. The more involved two-coefficient collection is necessary in characteristic two; the exact odd-prime tail formula is not asserted there.

In either case there are constants $C'>0$ and $\lambda<3$ such that $\log_p[\mathcal N:\mathcal N^{(n)}]\le C'\lambda^n$. If an analytic structure existed, its [dimension](../../../vector-space.md#dimension-vector-space) $d$ would be positive, since a zero-dimensional analytic [pro-p group](../../../topological-group.md#pro-p-group) is discrete and [compact](../../../topology.md#compact-space), hence finite. The second alternative of the supplied theorem would require

$$
\log_p[\mathcal N:\mathcal N^{(n)}]\ge d\,3^{n-s}
$$

for all sufficiently large $n$, for some fixed $s$. Combining the bounds gives $d3^{-s}\le C'(\lambda/3)^n$, impossible as $n\to\infty$.

The root solution proved hereditary just infiniteness, so the supplied theorem applies. Part (i) excluded its linear alternative, and this calculation excludes its growth alternative. Hence **the [Nottingham group](../../../topological-group.md#nottingham-group) is not analytic over any pro-$p$ ring**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
