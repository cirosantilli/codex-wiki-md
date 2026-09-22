# Paper 2

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper2.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper2.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Frattini subgroup](../../../finite-group-theory.md#frattini-subgroup) is the intersection of the [maximal subgroups](../../../group.md#maximal-subgroup) of $G$, with $\Phi(1)=1$. A useful equivalent property is

$$
H\Phi(G)=G\quad\Longrightarrow\quad H=G\qquad(H\le G).
$$

Indeed, a proper [subgroup](../../../group.md#subgroup) $H$ lies in a [maximal subgroup](../../../group.md#maximal-subgroup), which also contains $\Phi(G)$. The [Frattini subgroup](../../../finite-group-theory.md#frattini-subgroup) is a [characteristic subgroup](../../../algebra.md#characteristic-subgroup), since [automorphisms](../../../algebra.md#automorphism) permute the [maximal subgroups](../../../group.md#maximal-subgroup).

The [Fitting subgroup](../../../finite-group-theory.md#fitting-subgroup) is the largest [nilpotent normal subgroup](../../../finite-group-theory.md#nilpotent-normal-subgroup). To prove its existence, first form the [p-core](../../../finite-group-theory.md#p-core) $O_p(G)$: the product of all normal [p-subgroups](../../../finite-group-theory.md#p-subgroup). For two such [subgroups](../../../group.md#subgroup), their product is normal and has order $|AB|=|A||B|/|A\cap B|$, a power of $p$. There are only finitely many [subgroups](../../../group.md#subgroup), so $O_p(G)$ exists. For distinct primes $p,r$,

$$
[O_p(G),O_r(G)]\le O_p(G)\cap O_r(G)=1.
$$

Thus the product of the [p-cores](../../../finite-group-theory.md#p-core) is a [nilpotent normal subgroup](../../../finite-group-theory.md#nilpotent-normal-subgroup), a [direct product of groups](../../../group-theory.md#direct-product-of-groups) of its [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup). Conversely, a finite [nilpotent normal subgroup](../../../finite-group-theory.md#nilpotent-normal-subgroup) $K$ has unique [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup), each a [characteristic subgroup](../../../algebra.md#characteristic-subgroup) of $K$. Each is normal in $G$ and lies in the corresponding [p-core](../../../finite-group-theory.md#p-core). Consequently **the required largest [subgroup](../../../group.md#subgroup) exists**, and

$$
\boxed{F(G)=\prod_{p\mid |G|}O_p(G).}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $\Phi=\Phi(G)$ and choose a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) $P$ of $\Phi$. Since $\Phi$ is normal, the [Frattini argument](../../../finite-group-theory.md#frattini-argument) gives $G=\Phi N_G(P)$: for $g\in G$, the [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) $P^g$ and $P$ of $\Phi$ are conjugate by an element of $\Phi$, leaving an element of $N_G(P)$. The non-generator property of the [Frattini subgroup](../../../finite-group-theory.md#frattini-subgroup) proved above forces $N_G(P)=G$. Thus every [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) of $\Phi$ is normal. Distinct such [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) commute because their [group commutators](../../../group.md#group-commutator) lie in their trivial intersection. Hence $\Phi$ is a [nilpotent normal subgroup](../../../finite-group-theory.md#nilpotent-normal-subgroup), and

$$
\boxed{\Phi(G)\le F(G).}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write $F=F(G)$, $C=C_G(F)$ and $D=C\cap F=Z(F)$. Both $C$ and $D$ are normal in $G$. Suppose $C>D$. Choose a [minimal normal subgroup](../../../group-theory.md#minimal-normal-subgroup) $K/D$ of $G/D$ contained in $C/D$. In a finite [soluble group](../../../group-theory.md#solvable-group), such a [minimal normal subgroup](../../../group-theory.md#minimal-normal-subgroup) is [elementary abelian](../../../group.md#elementary-abelian-group): the last nontrivial term of its [derived series](../../../group-theory.md#derived-series) is an abelian [characteristic subgroup](../../../algebra.md#characteristic-subgroup), so minimality makes the whole [subgroup](../../../group.md#subgroup) abelian; its primary components and [subgroup](../../../group.md#subgroup) of elements killed by $p$ then force one prime and exponent $p$.

It follows that $K'\le D$. Moreover $K\le C$ centralizes $D\le F$, so $K'\le Z(K)$. Therefore $K$ is a [nilpotent group](../../../group-theory.md#nilpotent-group) of class at most two. Since $K$ is normal in $G$, the definition of the [Fitting subgroup](../../../finite-group-theory.md#fitting-subgroup) gives $K\le F$. But then $K\le C\cap F=D$, a contradiction. This proves the [Fitting subgroup is self-centralizing in soluble groups](../../../finite-group-theory.md#fitting-subgroup-is-self-centralizing-in-soluble-groups):

$$
\boxed{C_G(F(G))\le F(G),\qquad C_G(F(G))=Z(F(G)).}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

It suffices to centralize each [minimal normal subgroup](../../../group-theory.md#minimal-normal-subgroup) $M$. The [subgroup](../../../group.md#subgroup) $M\cap F(G)$ is normal in $G$, so it is either $1$ or $M$. In the first case

$$
[M,F(G)]\le M\cap F(G)=1.
$$

In the second case $M$ is a [nilpotent group](../../../group-theory.md#nilpotent-group). Its nontrivial [group center](../../../group-theory.md#center-of-a-group) is a [characteristic subgroup](../../../algebra.md#characteristic-subgroup) of $M$, hence normal in $G$, so minimality makes $M$ abelian. The primary components, which are [characteristic subgroups](../../../algebra.md#characteristic-subgroup), and the [subgroup](../../../group.md#subgroup) killed by a prime show that $M$ is [elementary abelian](../../../group.md#elementary-abelian-group) of exponent $p$. Thus $M\le O_p(G)$.

The [finite p-group](../../../finite-group-theory.md#finite-p-group) $O_p(G)$ acts by [conjugation](../../../group-theory.md#conjugation) on $M$. Its orbits have prime-power sizes; hence the number of fixed elements is congruent to $|M|=0$ modulo $p$. The identity is fixed, so there is a nonidentity fixed element. Therefore $M\cap Z(O_p(G))\ne1$. This intersection is normal in $G$, and minimality makes it $M$. The other [p-cores](../../../finite-group-theory.md#p-core) commute with $O_p(G)$, and hence with $M$. Thus every factor of $F(G)$ centralizes $M$. Since the [group socle](../../../group-theory.md#socle-of-a-finite-group) is generated by these [minimal normal subgroups](../../../group-theory.md#minimal-normal-subgroup),

$$
\boxed{F(G)\le C_G(\operatorname{Soc}(G)).}
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Put $\Phi=\Phi(G)$ and let $H$ be the full preimage of $F(G/\Phi)$ in $G$. The preceding part gives $\Phi\le F(G)$, so the normal nilpotent [image](../../../set-theory.md#image-of-a-function) $F(G)/\Phi$ lies in $F(G/\Phi)$.

For the reverse inclusion, choose a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) $P$ of $H$. Its [image](../../../set-theory.md#image-of-a-function) $P\Phi/\Phi$ is the unique [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) of the [nilpotent group](../../../group-theory.md#nilpotent-group) $H/\Phi$, hence a [characteristic subgroup](../../../algebra.md#characteristic-subgroup) there and normal in $G/\Phi$. Thus $P\Phi\trianglelefteq G$. The [subgroup](../../../group.md#subgroup) $P$ is also a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) of $P\Phi$: the p-part of $\Phi$ lies in $P$, because $P\cap\Phi$ is a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) of the [normal subgroup](../../../group-theory.md#normal-subgroup) $\Phi$ of $H$. Apply the [Frattini argument](../../../finite-group-theory.md#frattini-argument) to $P\Phi$:

$$
G=(P\Phi)N_G(P)=\Phi N_G(P).
$$

The [Frattini subgroup](../../../finite-group-theory.md#frattini-subgroup) property forces $N_G(P)=G$. Hence every [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) of $H$ is normal, so $H$ is a [nilpotent group](../../../group-theory.md#nilpotent-group) and $H\le F(G)$. Together the inclusions prove

$$
\boxed{F(G/\Phi(G))=F(G)/\Phi(G).}
$$

This is [Frattini lifting of nilpotence](../../../finite-group-theory.md#frattini-lifting-of-nilpotence); simply calling an extension of [nilpotent groups](../../../group-theory.md#nilpotent-group) nilpotent would not establish it.

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [soluble group](../../../group-theory.md#solvable-group) is a [group](../../../group.md) whose [derived series](../../../group-theory.md#derived-series) $G^{(0)}=G$, $G^{(i+1)}=[G^{(i)},G^{(i)}]$ terminates at $1$. Equivalently, it has a finite [subnormal series](../../../group-theory.md#subnormal-series) with abelian factors. For the reverse implication, if $G/N$ has derived length $r$, then $G^{(r)}\le N$; if $N$ has derived length $s$, then $G^{(r+s)}=1$. Iterating this observation through the series proves the equivalence. For a finite [group](../../../group.md), refining the abelian factors to [composition factors](../../../module-theory.md#composition-factor) says that solubility is equivalent to all [composition factors](../../../module-theory.md#composition-factor) being cyclic of prime order.

[Subgroups](../../../group.md#subgroup) and [quotient groups](../../../group-theory.md#quotient-group) of [soluble groups](../../../group-theory.md#solvable-group) are soluble, since their [derived series](../../../group-theory.md#derived-series) lie in, or are images of, the original series. The same calculation proves closure under [group extensions](../../../group-theory.md#group-extension). [Finite p-groups](../../../finite-group-theory.md#finite-p-group) are [nilpotent groups](../../../group-theory.md#nilpotent-group), hence soluble: their nontrivial centers allow induction to construct a [central series](../../../group-theory.md#central-series). Every finite [nilpotent group](../../../group-theory.md#nilpotent-group) is a [direct product of groups](../../../group-theory.md#direct-product-of-groups) of its [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup). The converse fails: $S_3$ has the abelian-factor series $1<C_3<S_3$, but its order-two [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) are not normal. The [symmetric group](../../../finite-group-theory.md#symmetric-group) $S_4$ is also soluble, with series $1<V_4<A_4<S_4$ and abelian factors. A finite [soluble group](../../../group-theory.md#solvable-group) has elementary abelian [minimal normal subgroups](../../../group-theory.md#minimal-normal-subgroup), by the argument in 1(c). In contrast, a nonabelian [simple group](../../../finite-group-theory.md#simple-group) is a [perfect group](../../../group-theory.md#perfect-group) and is not soluble.

The [Fitting subgroup](../../../finite-group-theory.md#fitting-subgroup) collects the normal nilpotent structure. For a nontrivial finite [soluble group](../../../group-theory.md#solvable-group) it is nontrivial, since it contains an elementary abelian [minimal normal subgroup](../../../group-theory.md#minimal-normal-subgroup). Part 1(c) proves $C_G(F)\le F$, so [conjugation](../../../group-theory.md#conjugation) embeds $G/C_G(F)$ in $\operatorname{Aut}(F)$. This shows why controlling a [soluble group](../../../group-theory.md#solvable-group) through normal abelian or nilpotent layers is effective, even when the whole [group](../../../group.md) is not a [nilpotent group](../../../group-theory.md#nilpotent-group).

For a set of primes $\pi$, a [Hall subgroup](../../../group.md#hall-subgroup) of type $\pi$ has order divisible only by primes in $\pi$ and index divisible only by primes outside $\pi$. The [Hall theorem for soluble groups](../../../group.md#hall-conjugacy-and-embedding-in-finite-soluble-groups) says that a finite [soluble group](../../../group-theory.md#solvable-group) has such [subgroups](../../../group.md#subgroup), any two are conjugate, and every [subgroup](../../../group.md#subgroup) of $\pi$-order is contained in one. These assertions generalize the [Sylow theorems](../../../finite-group-theory.md#sylow-theorems), which treat a single prime. Here is a proof of all three assertions.

First we need [coprime splitting over an elementary abelian normal subgroup](../../../group-theory.md#coprime-splitting-over-an-elementary-abelian-normal-subgroup). Suppose $V\trianglelefteq E$ is an elementary abelian p-group and $Q=E/V$ has order $h$ prime to $p$. A section $s:Q\to E$ defines an action on $V$ and an additive factor set $f(x,y)$ by $s(x)s(y)=f(x,y)s(xy)$. Associativity says

$$
f(x,y)+f(xy,z)=x f(y,z)+f(x,yz).
$$

Summing over $z\in Q$ and dividing by $h$ in $V$ gives $f(x,y)=b(x)+xb(y)-b(xy)$, where $b(x)=h^{-1}\sum_zf(x,z)$. Replacing $s(x)$ by $-b(x)s(x)$ removes the factor set, giving a complement. Two complements differ by a map $d$ satisfying $d(xy)=d(x)+xd(y)$. Averaging over $y$ gives $d(x)=b-xb$, so the complements are conjugate by an element of $V$. This proves both splitting and conjugacy, without assuming that an arbitrary extension splits.

Induct on $|G|$, taking an elementary abelian [minimal normal subgroup](../../../group-theory.md#minimal-normal-subgroup) $V$ of exponent $p$. Choose a quotient [Hall subgroup](../../../group.md#hall-subgroup) $\bar H\le G/V$ and let $K$ be its preimage. If $p\in\pi$, then $K$ itself is a [Hall subgroup](../../../group.md#hall-subgroup). If $p\notin\pi$, the preceding splitting argument gives a complement $H$ to $V$ in $K$, and that complement is a [Hall subgroup](../../../group.md#hall-subgroup) of $G$.

For conjugacy, the images of two [Hall subgroups](../../../group.md#hall-subgroup) are quotient [Hall subgroups](../../../group.md#hall-subgroup), so induction allows them to have the same [image](../../../set-theory.md#image-of-a-function) and lie in the same $K$. If $p\in\pi$, every [Hall subgroup](../../../group.md#hall-subgroup) contains $V$: its product with $V$ is a $\pi$-subgroup and cannot be larger by the subgroup-order formula. Both are then $K$. If $p\notin\pi$, both are complements to $V$ in $K$, so the averaging argument conjugates them.

Finally let $U\le G$ be any $\pi$-subgroup. By induction its [image](../../../set-theory.md#image-of-a-function) lies in a quotient [Hall subgroup](../../../group.md#hall-subgroup), so $U\le K$. If $p\in\pi$, $K$ is already a [Hall subgroup](../../../group.md#hall-subgroup) containing $U$. Otherwise write $K=V\rtimes H$. In $VU$, both $U$ and the inverse [image](../../../set-theory.md#image-of-a-function) in $H$ of the [image](../../../set-theory.md#image-of-a-function) of $U$ are complements to $V$. Complement conjugacy therefore places $U$ in a conjugate of $H$. This proves embedding and completes the induction.

**Thus existence, conjugacy and containment all hold for every prime set in a finite [soluble group](../../../group-theory.md#solvable-group).** The solubility hypothesis matters: $A_5$ has no [Hall subgroup](../../../group.md#hall-subgroup) for $\pi=\{2,5\}$. Such a [subgroup](../../../group.md#subgroup) would have index three; its coset action would give a nontrivial [group homomorphism](../../../group-theory.md#group-homomorphism) $A_5\to S_3$, impossible because $A_5$ is a [simple group](../../../finite-group-theory.md#simple-group) and has order $60$. This example also distinguishes a [Hall subgroup](../../../group.md#hall-subgroup) from a merely arbitrary [subgroup](../../../group.md#subgroup) whose order uses the chosen primes.

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Since the [two-transitive group action](../../../group-theory.md#two-transitive-group-action) is primitive, the orbits of any nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) form only the single block $\Omega$. Thus $N$ is transitive. If $N$ is regular, identify $\Omega$ with $N$ by $x\mapsto x\alpha$. Then $G=NG_\alpha$, $N\cap G_\alpha=1$, and [conjugation](../../../group-theory.md#conjugation) by $G_\alpha$ gives [automorphisms](../../../algebra.md#automorphism) of $N$. The [two-transitive group action](../../../group-theory.md#two-transitive-group-action) makes these [automorphisms](../../../algebra.md#automorphism) transitive on $N\setminus\{1\}$. All nonidentity elements therefore have the same order, which must be a prime $p$: a suitable power of an element of composite order would have a smaller nontrivial order. [Cauchy's theorem for finite groups](../../../finite-group-theory.md#cauchy-theorem-for-groups) now shows $|N|=p^d$.

The [center of a group](../../../group-theory.md#center-of-a-group) of prime-power order is nontrivial and is a [characteristic subgroup](../../../algebra.md#characteristic-subgroup). The transitive [conjugation](../../../group-theory.md#conjugation) action on nonidentity elements therefore forces $Z(N)=N$. Hence $N$ is an [elementary abelian group](../../../group.md#elementary-abelian-group), which we identify with the additive [vector space](../../../vector-space.md) $\mathbb F_p^d$. [Conjugation](../../../group-theory.md#conjugation) by $G_\alpha$ is linear on this [vector space](../../../vector-space.md). It is faithful: an element fixing $\alpha$ and centralizing $N$ fixes every $x\alpha$, hence is the identity permutation. Consequently

$$
\boxed{n=p^d,\qquad G=N\rtimes G_\alpha\le AGL_d(p).}
$$

Here the [general affine group](../../../group-theory.md#general-affine-group) acts by translations followed by invertible [linear maps](../../../vector-space.md#linear-map).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The orbits of $N_\alpha\trianglelefteq G_\alpha$ on $\Omega\setminus\{\alpha\}$ have a common size $r$, because $G_\alpha$ is transitive there. Suppose $N$ has a [block system](../../../group-theory.md#block-system) of block size $b$, $1<b<n$. Since $r\mid n-1$ and $b\mid n$, $\gcd(r,b)=1$. Let $B$ be the block of $\alpha$ and $C\ne B$ another block. The union $N_\alpha C$ is a union of blocks and of r-element point-orbits, so its size is divisible by $br$; it is at most $br$. Equality means each of the b point-orbits meets $C$ once. Thus $N_{\alpha\beta}$ fixes $C$ pointwise for $\beta\in C$. Interchanging $\alpha,\beta$ also makes it fix $B$. All two-point stabilizers have order $|N_\alpha|/r$. Therefore $N_{\alpha\beta}=N_{\alpha\gamma}$ for every $\gamma\in B\setminus\{\alpha\}$. Varying $\beta$ outside $B$ shows this same [subgroup](../../../group.md#subgroup) fixes every point, so it is trivial. We have proved [uniform subdegrees force an imprimitive action to be Frobenius](../../../group-theory.md#uniform-subdegrees-force-an-imprimitive-action-to-be-frobenius): no nonidentity element of $N$ fixes two points.

Write $|N_\alpha|=h$. The distinct [point stabilizers](../../../group-theory.md#stabilizer-subgroup) meet only at $1$, and $|N|=nh$. Thus the set $D$ of fixed-point-free elements of $N$ has size

$$
|D|=nh-\bigl(1+n(h-1)\bigr)=n-1.
$$

Count triples $(\alpha,\beta,x)$ with $x\in D$ and $x\alpha=\beta$: there are $n(n-1)$, exactly the number of ordered distinct pairs. [Conjugation](../../../group-theory.md#conjugation) by the [two-transitive](../../../group-theory.md#two-transitive-group-action) [group](../../../group.md) makes every pair occur, hence each pair has a unique such $x$. It follows that $G$ conjugates all elements of $D$ transitively.

Also $h\mid n-1$, since $N_\alpha$ acts freely on the remaining points. For each prime $p\mid n$, [Cauchy's theorem for finite groups](../../../finite-group-theory.md#cauchy-theorem-for-groups) supplies an order-p element of $N$; it cannot fix a point, since $p\nmid h$. Conjugacy of $D$ forces all these primes to coincide, so $n=p^d$ and every element of $D$ has order $p$. A [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) $P$ of $N$ has order $n$, because $p\nmid h$. Every nonidentity element of $P$ is fixed-point-free, so $P=\{1\}\cup D$. This uniquely described [subgroup](../../../group.md#subgroup) is normal in $G$. Minimal normality of $N$ gives $P=N$, and $|N|=n$. **Therefore $N$ is regular.** The proof establishes closure through a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup); it does not assume that a set of derangements is automatically a [subgroup](../../../group.md#subgroup).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

A finite [minimal normal subgroup](../../../group-theory.md#minimal-normal-subgroup) is a [characteristically simple group](../../../algebra.md#characteristically-simple-group), and has the [direct-product structure of a finite minimal normal subgroup](../../../group-theory.md#direct-product-structure-of-a-finite-minimal-normal-subgroup)

$$
N=T_1\times\cdots\times T_k
$$

with isomorphic [simple groups](../../../finite-group-theory.md#simple-group) $T_i$. For completeness, choose a minimal nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) $T$ of $N$. Its distinct $G$-conjugates are [minimal normal subgroups](../../../group-theory.md#minimal-normal-subgroup) of $N$, so they centralize one another. Their product is normal in $G$, hence equals $N$. If $T$ is abelian the product is abelian and minimal primary [characteristic subgroups](../../../algebra.md#characteristic-subgroup) make $N$ elementary abelian. Otherwise each $T$ has trivial center: its center is a [characteristic subgroup](../../../algebra.md#characteristic-subgroup) of $T$, hence normal in $N$, and minimality would make $T$ abelian. Each new conjugate then meets the product of previous conjugates trivially, because it centralizes that product and is centerless. The product is direct. Every [normal subgroup](../../../group-theory.md#normal-subgroup) of a direct factor is normal in $N$, so minimality of that factor makes it simple.

Assume now that $N$ acts primitively and nonregularly. Any nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) of this faithful primitive action is transitive. Thus each $T_i$ is transitive. If $k\ge2$, the transitive commuting [groups](../../../group.md) $T_1$ and $T_2$ are regular: an element of one fixing $\alpha$ commutes with the other and hence fixes its entire orbit. But the [centralizer](../../../group-theory.md#centralizer) of a regular [group](../../../group.md) has order $n$, as its elements are determined by the [image](../../../set-theory.md#image-of-a-function) of $\alpha$. Therefore all remaining factors lie in the order-n [centralizer](../../../group-theory.md#centralizer) of $T_1$, and the transitive [group](../../../group.md) $T_2$ already fills it. There can be only two factors, with $|N|=n^2$. Now $|N_\alpha|=n$, whereas its common nontrivial subdegree $r$ divides both $n$ and $n-1$. Hence $r=1$, making $N_\alpha$ trivial, a contradiction. Thus $k=1$, and $N$ is simple. An abelian transitive [group](../../../group.md) is regular, so $N$ is nonabelian.

Finally $C_G(N)$ is normal in the primitive [group](../../../group.md) $G$. If nontrivial it would be transitive, and commuting with transitive $N$ would force $N$ regular. Thus $C_G(N)=1$, and [conjugation](../../../group-theory.md#conjugation) embeds $G$ in $\operatorname{Aut}(N)$. The centerless simple [group](../../../group.md) $N$ is identified with its [inner automorphism group](../../../group-theory.md#inner-automorphism). Therefore

$$
\boxed{N\text{ is nonabelian simple},\qquad N\le G\le\operatorname{Aut}(N).}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

By 3(a), identify $\Omega$ with $V=\mathbb F_p^d$ and let $H=G_0\le GL_d(p)$. Four-transitivity means $H$ is transitive on ordered triples of distinct nonzero [vectors](../../../vector-space.md#vector), and in particular on ordered pairs of distinct nonzero [vectors](../../../vector-space.md#vector).

If $p>2$ and $d\ge2$, the pairs $(u,au)$ with $a\ne0,1$ and $(u,v)$ with $u,v$ [linearly independent](../../../vector-space.md#linear-independence) cannot be interchanged by a [linear map](../../../vector-space.md#linear-map). Thus $d=1$ if $p>2$. Then $|H|\le p-1$, whereas pair-transitivity on the $p-1$ nonzero points requires $(p-1)(p-2)\le |H|$. This forces $p\le3$, incompatible with four-transitivity, whose degree is at least four.

Hence $p=2$. If $d\ge3$, the triples $(u,v,u+v)$ and $(u,v,w)$ for [linearly independent](../../../vector-space.md#linear-independence) $u,v,w$ cannot be interchanged: the first is [linearly dependent](../../../vector-space.md#linear-dependence) and the second is not. Thus $d=2$. The [general affine group](../../../group-theory.md#general-affine-group) $AGL_2(2)$ has order $4(4-1)(4-2)=24$. Four-transitivity on four points requires $24\mid |G|$, and $G\le AGL_2(2)\le S_4$. Consequently

$$
\boxed{n=4,\qquad G=AGL_2(2)\cong S_4.}
$$

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The orbits of a [normal subgroup](../../../group-theory.md#normal-subgroup) $N$ are blocks for the [primitive group action](../../../group-theory.md#primitive-group-action). If every orbit is a singleton then $N\le G_{[\Omega]}$, giving the second alternative. Otherwise $N$ is transitive, and $G=NG_\alpha$.

Work in $G/N$. Every $g\in G$ can be written $nh$ with $n\in N$, $h\in G_\alpha$. [Conjugation](../../../group-theory.md#conjugation) by $n$ has no effect on the [image](../../../set-theory.md#image-of-a-function) of a [subgroup](../../../group.md#subgroup) in this quotient, while $h$ normalizes $A$. Thus every conjugate of $A$ has the same [image](../../../set-theory.md#image-of-a-function) $AN/N$. The generation hypothesis says this [image](../../../set-theory.md#image-of-a-function) generates all of $G/N$. But it is already an abelian [subgroup](../../../group.md#subgroup), so $G/N$ is abelian and $G'\le N$. This proves the [Iwasawa simplicity lemma](../../../finite-group-theory.md#iwasawa-simplicity-lemma) in its possibly nonfaithful form:

$$
\boxed{G'\le N\quad\text{or}\quad N\le G_{[\Omega]}.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For $i\ne j$, put $x_{ij}(a)=I+aE_{ij}$. When $a\ne0$ this is a [transvection](../../../vector-space.md#transvection): it fixes the [hyperplane](../../../vector-space.md#hyperplane) $v_j=0$ pointwise and has rank-one difference from the identity. Its inverse is $x_{ij}(-a)$ and its [determinant](../../../linear-algebra.md#determinant) is one.

Left multiplication performs a row addition. For an invertible [matrix](../../../vector-space.md#matrix), bring a nonzero entry into a pivot position by a signed interchange, then clear its column by row additions. A signed interchange on two coordinates is itself a product of row additions, because

$$
w(a)=x_{12}(a)x_{21}(-a^{-1})x_{12}(a)
=\begin{pmatrix}0&a\\-a^{-1}&0\end{pmatrix}\qquad(a\ne0).
$$

Repeating the pivot construction and then clearing above the pivots reduces any determinant-one [matrix](../../../vector-space.md#matrix) to a diagonal [matrix](../../../vector-space.md#matrix) of [determinant](../../../linear-algebra.md#determinant) one. Finally

$$
w(a)w(-1)=\operatorname{diag}(a,a^{-1}).
$$

A determinant-one diagonal [matrix](../../../vector-space.md#matrix) is a product of such two-coordinate matrices, using the last coordinate to compensate each of the first $n-1$ diagonal entries. Each displayed [matrix](../../../vector-space.md#matrix) is a product of [elementary transvection matrices](../../../vector-space.md#elementary-transvection-matrix). Hence reversing the elimination proves

$$
\boxed{SL_n(F)=\langle x_{ij}(a):i\ne j,\ a\in F\rangle.}
$$

This argument works over every [field](../../../algebra.md#field), including [characteristic](../../../algebra.md#characteristic-of-a-field) two.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let $S=SL_n(F)$ and let $Z$ be its scalar center. Its action on the lines of $F^n$ has [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) exactly $Z$: a [linear map](../../../vector-space.md#linear-map) fixing every line is diagonal in a basis, and fixing the lines spanned by $e_i+e_j$ makes all its diagonal entries equal. The action is two-transitive. Indeed an ordered pair of distinct lines can be represented by two independent [vectors](../../../vector-space.md#vector) and extended to a basis. A [linear map](../../../vector-space.md#linear-map) between two such bases can be adjusted to [determinant](../../../linear-algebra.md#determinant) one by scaling one target basis [vector](../../../vector-space.md#vector); this preserves both target lines. Therefore $S/Z$ has a faithful [primitive group action](../../../group-theory.md#primitive-group-action).

Fix $L=Fv$. The maps

$$
A_L=\{I+vf:f\in(F^n)^*,\ f(v)=0\}
$$

form an abelian [subgroup](../../../group.md#subgroup): all products of the rank-one terms vanish. It is normal in the line stabilizer, since [conjugation](../../../group-theory.md#conjugation) replaces $v$ by a [scalar multiple](../../../vector-space.md#scalar-multiple) and transports $f$. Its conjugates contain every [transvection](../../../vector-space.md#transvection), and hence generate $S$ by 4(b). The same statements hold for its [image](../../../set-theory.md#image-of-a-function) in $S/Z$.

It remains to prove perfectness rather than assume it. Use the [group commutator](../../../group.md#group-commutator) convention $[x,y]=xyx^{-1}y^{-1}$. If $n\ge3$, distinct $i,j,k$ give

$$
[x_{ik}(a),x_{kj}(b)]=x_{ij}(ab).
$$

Every elementary generator is consequently in $S'$. If $n=2$ and $|F|>3$, choose $a\in F^*$ with $a^2\ne1$. There are at most two roots of $a^2=1$, so such a choice exists. For $h=\operatorname{diag}(a,a^{-1})$,

$$
[h,x_{12}(b)]=x_{12}((a^2-1)b).
$$

Varying $b$ gives every upper [transvection](../../../vector-space.md#transvection); conjugating by $w(1)$ gives every lower one. Again $S'=S$, and its projective quotient is a [perfect group](../../../group-theory.md#perfect-group).

Apply 4(a) to this faithful primitive projective action. Every nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) contains the [commutator subgroup](../../../group-theory.md#commutator-subgroup), which is the whole quotient. Thus

$$
\boxed{PSL_n(F)\text{ is simple if }n\ge3\text{ or if }n=2,\ |F|>3.}
$$

The restriction is real: $PSL_2(2)\cong S_3$ and $PSL_2(3)\cong A_4$ are not simple.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Replace $F^n$ by a [symplectic vector space](../../../linear-algebra.md#symplectic-vector-space) $(V,B)$ of dimension $2m$, and elementary row operations by [symplectic transvections](../../../finite-group-theory.md#symplectic-transvection)

$$
T_{v,c}(x)=x+cB(x,v)v.
$$

The cross terms in $B(Tx,Ty)$ cancel, and $B(v,v)=0$, so these maps preserve $B$. Their inverses are $T_{v,-c}$.

They generate $Sp(V)$ by the following [symplectic basis](../../../linear-algebra.md#symplectic-basis) elimination. If $B(u,v)\ne0$, a single [transvection](../../../vector-space.md#transvection) with direction $v-u$ and parameter $1/B(u,v)$ sends $u$ to $v$. If $B(u,v)=0$ and $u\ne v$, choose $w$ with both $B(u,w)$ and $B(w,v)$ nonzero: the union of two proper [hyperplanes](../../../vector-space.md#hyperplane) does not exhaust a [vector space](../../../vector-space.md), even over $\mathbb F_2$. Two [transvections](../../../vector-space.md#transvection) then suffice. Thus one can make a form-preserving [linear map](../../../vector-space.md#linear-map) fix the first basis [vector](../../../vector-space.md#vector) $e$. Next align its partner $f$, while keeping $e$ fixed. Two partners have difference in $e^\perp$, so the preceding single-transvection construction uses a direction in $e^\perp$ whenever their mutual pairing is nonzero. If it is zero, the intermediate partner $f+ae$, $a\ne0$, has nonzero pairing with both. All these [transvections](../../../vector-space.md#transvection) fix $e$. Once both $e,f$ are fixed, recurse on their [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) [symplectic orthogonal complement](../../../linear-algebra.md#symplectic-orthogonal-complement). This proves generation over every [field](../../../algebra.md#field).

Use the action on the points of [projective space](../../../projective-space.md), whose [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is the scalar center $Z=\{\lambda I:\lambda^2=1\}$. For $m=1$ this is the $SL_2$ case. For $m\ge2$ the action is primitive, although it is generally not two-transitive. The stabilizer of a line $L$ has two orbits on other lines: those orthogonal to $L$ and those not orthogonal to $L$. This follows by extending a [hyperbolic pair](../../../linear-algebra.md#hyperbolic-pair), or an independent isotropic pair, to a [symplectic basis](../../../linear-algebra.md#symplectic-basis). A block containing $L$ and a second line $M$ contains the entire corresponding orbit of the stabilizer of $L$. The stabilizer of $M$ then supplies a line of the other type: choose a [vector](../../../vector-space.md#vector) orthogonal to one of $L,M$ and not to the other. Nondegeneracy and independence guarantee such a [vector](../../../vector-space.md#vector), also in dimension four. Hence the block contains both orbits and is the whole set.

The [transvections](../../../vector-space.md#transvection) along $L$ form an abelian normal [subgroup](../../../group.md#subgroup) of its stabilizer; their conjugates generate the [group](../../../group.md). Thus the [Iwasawa simplicity lemma](../../../finite-group-theory.md#iwasawa-simplicity-lemma) applies as soon as perfectness is established. For $|F|>3$, every [transvection](../../../vector-space.md#transvection) lies in an embedded $SL_2(F)$ acting on a hyperbolic plane, and 4(c) proves that embedded [group](../../../group.md) perfect.

For the remaining fields, the [perfectness of finite symplectic groups](../../../finite-group-theory.md#perfectness-of-finite-symplectic-groups) has a short direct proof. Over $\mathbb F_3$ with $m\ge2$, all parameter-one [transvections](../../../vector-space.md#transvection) have the same class $t$ in the [abelianization](../../../group-theory.md#abelianization), and $3t=0$. In an isotropic plane with basis $u,v$, the four directions $u,v,u+v,u-v$ give commuting [transvections](../../../vector-space.md#transvection) whose product is $1$: their rank-one terms add to zero, since

$$
uu^{\mathsf T}+vv^{\mathsf T}+(u+v)(u+v)^{\mathsf T}+(u-v)(u-v)^{\mathsf T}=0
$$

over $\mathbb F_3$. Thus $4t=0$, giving $t=0$. Parameter-two [transvections](../../../vector-space.md#transvection) are inverses, so all generators vanish in the [abelianization](../../../group-theory.md#abelianization). Over $\mathbb F_2$ with $m\ge3$, use the seven nonzero [vectors](../../../vector-space.md#vector) of an isotropic three-space. Their commuting [transvections](../../../vector-space.md#transvection) multiply to $1$, since each diagonal coordinate of $\sum_{0\ne v}vv^{\mathsf T}$ occurs four times and each off-diagonal coordinate twice. Their common abelianized class satisfies $2t=7t=0$, and again the [group](../../../group.md) is perfect.

Consequently **the projective [symplectic group](../../../symplectic-geometry.md#symplectic-group) is simple**, with the necessary exceptions

$$
\boxed{PSp_{2m}(F)\text{ simple, except }(m,F)=(1,\mathbb F_2),(1,\mathbb F_3),(2,\mathbb F_2).}
$$

The first two are the linear exceptions; the last is $Sp_4(2)\cong S_6$, proved in 6(c). The word “projective” matters: the unquotiented [symplectic group](../../../symplectic-geometry.md#symplectic-group) may have the nontrivial scalar center $\{I,-I\}$.

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For $g\in GL_n(q)$, make $V=\mathbb F_q^n$ a [module](../../../module-theory.md#module-mathematics) over the [polynomial ring](../../../commutative-algebra.md#polynomial-ring) $R=\mathbb F_q[t]$ by $t\cdot v=gv$. The [structure theorem for finitely generated modules over a principal ideal domain](../../../module-theory.md#structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain) and [primary decomposition](../../../module-theory.md#primary-decomposition) give

$$
V\cong\bigoplus_{f\ne t}\bigoplus_{j\ge1}\bigl(R/(f^j)\bigr)^{m_j(f)}.
$$

Here $f$ ranges over [monic polynomials](../../../polynomial.md#monic-polynomial) that are [irreducible polynomials](../../../polynomial.md#irreducible-polynomial), and $t$ is excluded because $g$ is invertible. Associate the [integer partition](../../../combinatorics.md#integer-partition) $\lambda_f$ having $m_j(f)$ parts equal to $j$. It has finite support and satisfies $\sum_f\deg(f)|\lambda_f|=n$. Two matrices are conjugate exactly when their R-modules are isomorphic, so this gives a bijective parameterization of [conjugacy classes](../../../group-theory.md#conjugacy-class).

The [centralizer](../../../group-theory.md#centralizer) is the R-module [automorphism](../../../algebra.md#automorphism) [group](../../../group.md). Homomorphisms between distinct primary components vanish: coprimeness of their annihilating [polynomials](../../../polynomial.md) makes each such map zero. Fix one $f$ of degree $d$, put $Q=q^d$, and write $m_j=m_j(f)$. A map $R/(f^a)\to R/(f^b)$ is determined by an [image](../../../set-theory.md#image-of-a-function) killed by $f^a$, so its space has dimension $d\min(a,b)$ over $\mathbb F_q$. Consequently the [endomorphism](../../../algebra.md#endomorphism) algebra $E$ has

$$
|E|=Q^{\sum_{a,b}\min(a,b)m_am_b}=Q^{\sum_i(\lambda'_i)^2},
$$

where $\lambda'$ is the [conjugate partition](../../../representation-theory-of-the-symmetric-group.md#conjugate-partition).

Its semisimple quotient is $\prod_jM_{m_j}(\mathbb F_Q)$: reduce the maps between the equal-length summands modulo $f$ and discard the maps between unequal lengths. Composition through a different length acquires a factor of $f$ when it returns to the original length, so these reductions define an algebra homomorphism. It is onto, and its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is nilpotent. One can see the latter directly by expanding a sufficiently long product into paths through the finitely many possible summand lengths: repeated returns through unequal lengths or equal-length [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) factors accumulate powers of $f$, while a strictly monotone path has bounded length. Eventually every path vanishes in every summand.

An element is invertible exactly when its [image](../../../set-theory.md#image-of-a-function) in that quotient is invertible, since a nilpotent error is inverted by a finite [geometric series](../../../real-analysis.md#geometric-series). The fraction of units is therefore $\prod_j|GL_{m_j}(Q)|/Q^{m_j^2}=\prod_j\prod_{r=1}^{m_j}(1-Q^{-r})$. Multiplying the independent primary contributions gives the [primary matrix centralizer formula](../../../linear-operator-theory.md#primary-matrix-centralizer-formula):

$$
\boxed{|C_{GL_n(q)}(g)|=\prod_{f\ne t}q^{\deg(f)\sum_i(\lambda'_{f,i})^2}\prod_{j\ge1}\prod_{r=1}^{m_j(f)}(1-q^{-r\deg(f)}).}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The [generating function](../../../real-analysis.md#generating-function) for [integer partitions](../../../combinatorics.md#integer-partition) is $\sum_\lambda u^{|\lambda|}=\prod_{i\ge1}(1-u^i)^{-1}$, since independently choosing the multiplicity of each part size gives a [geometric series](../../../real-analysis.md#geometric-series). Applying the parameterization in 5(a),

$$
\sum_{n\ge0}k_n(q)t^n=\prod_{f\ne t}\prod_{i\ge1}(1-t^{i\deg(f)})^{-1}.
$$

Unique factorization of [monic polynomials](../../../polynomial.md#monic-polynomial) shows

$$
\prod_{f\ne t}(1-u^{\deg(f)})^{-1}
=1+\sum_{r\ge1}(q-1)q^{r-1}u^r
=\frac{1-u}{1-qu}.
$$

Indeed the left side counts [monic polynomials](../../../polynomial.md#monic-polynomial) with nonzero constant term; in degree $r\ge1$ there are $(q-1)q^{r-1}$ choices. Reordering the formal products is legitimate because only finitely many factors contribute to any fixed coefficient. Substituting $u=t^i$ for each $i$ gives the [conjugacy-class generating function for finite general linear groups](../../../finite-group-theory.md#conjugacy-class-generating-function-for-finite-general-linear-groups):

$$
\boxed{k_n(q)=[t^n]\prod_{i\ge1}\frac{1-t^i}{1-qt^i}.}
$$

The constant term corresponds to the trivial zero-dimensional [group](../../../group.md).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Translation $X\mapsto I+X$ is a [bijection](../../../function.md#bijection) from [nilpotent matrices](../../../linear-operator-theory.md#nilpotent-matrix) to [unipotent matrices](../../../lie-theory.md#unipotent-matrix). We can count the former without requiring a further partition identity. Let $a_n$ be their number, with $a_0=1$.

Every [linear operator](../../../vector-space.md#linear-operator) $T$ has a unique decomposition from the [Fitting lemma](../../../module-theory.md#fitting-lemma)

$$
V=\ker T^n\oplus\operatorname{im}T^n,
$$

on which it is respectively nilpotent and invertible. To justify the decomposition, kernels and images stabilize by step $n$; if $T^nv\in\ker T^n$, then $v\in\ker T^{2n}=\ker T^n$, so $T^nv=0$. The dimensions then show the sum is all of $V$, and stabilization makes $T$ invertible on the [image](../../../set-theory.md#image-of-a-function). These two summands are determined by $T$, so there is no overcounting.

For a nilpotent summand of dimension $k$, the number of ordered complementary subspaces is $|GL_n(q)|/(|GL_k(q)||GL_{n-k}(q)|)$, by transporting two fixed bases. The restrictions of $T$ have $a_k$ and $|GL_{n-k}(q)|$ choices. Summing all $q^{n^2}$ [matrices](../../../vector-space.md#matrix) gives

$$
\frac{q^{n^2}}{|GL_n(q)|}=\sum_{k=0}^n\frac{a_k}{|GL_k(q)|}.
$$

Write $\phi_n(q^{-1})=\prod_{i=1}^n(1-q^{-i})$, so $|GL_n(q)|=q^{n^2}\phi_n(q^{-1})$. Subtract the same equation for $n-1$:

$$
\frac{a_n}{|GL_n(q)|}=\frac1{\phi_n(q^{-1})}-\frac1{\phi_{n-1}(q^{-1})}
=\frac{q^{-n}}{\phi_n(q^{-1})}.
$$

Thus [counting nilpotent matrices by the Fitting decomposition](../../../linear-operator-theory.md#counting-nilpotent-matrices-by-the-fitting-decomposition) proves

$$
\boxed{\#\{\text{unipotent elements of }GL_n(q)\}=a_n=q^{n^2-n}.}
$$

The supplied product identity is consistent with the resulting mass series: taking its variables to be $s=u$, $t=q^{-1}$ gives $\sum_na_nu^n/|GL_n(q)|=\prod_{i\ge1}(1-uq^{-i})^{-1}$.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

For the fixed degree-two [irreducible polynomial](../../../polynomial.md#irreducible-polynomial) $f$, a [matrix](../../../vector-space.md#matrix) with [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) a power of $f$ has only one primary component. Its [conjugacy classes](../../../group-theory.md#conjugacy-class) correspond to [integer partitions](../../../combinatorics.md#integer-partition) $\lambda$ of $m$. By the [primary matrix centralizer formula](../../../linear-operator-theory.md#primary-matrix-centralizer-formula), its [centralizer](../../../group-theory.md#centralizer) has exactly the same order $c_\lambda(q^2)$ as the [centralizer](../../../group-theory.md#centralizer) of the corresponding [unipotent matrix](../../../lie-theory.md#unipotent-matrix) in $GL_m(q^2)$.

Sum the [conjugacy class](../../../group-theory.md#conjugacy-class) sizes:

$$
\#\{g\in GL_{2m}(q):\mu_g=f^a\text{ for some }a\ge1\}
=|GL_{2m}(q)|\sum_{\lambda\vdash m}\frac1{c_\lambda(q^2)}.
$$

The same sum times $|GL_m(q^2)|$ is the number of [unipotent matrices](../../../lie-theory.md#unipotent-matrix) of $GL_m(q^2)$, which 5(c) shows is $(q^2)^{m^2-m}$. Hence [counting matrices with a fixed primary polynomial](../../../linear-operator-theory.md#counting-matrices-with-a-fixed-primary-polynomial) gives

$$
\boxed{q^{2m^2-2m}\frac{|GL_{2m}(q)|}{|GL_m(q^2)|}.}
$$

In particular the exponent $a$ of the minimal polynomial is not fixed in advance: summing all [integer partitions](../../../combinatorics.md#integer-partition) includes every possible largest block size. The usual statement takes $m\ge1$; dimension zero can instead be included with its identity convention.

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Let $V$ have dimension $2m$ over the [finite field](../../../algebra.md#finite-field) $\mathbb F_q$, with a [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) [alternating bilinear form](../../../linear-algebra.md#alternating-bilinear-form) $B$. The [symplectic group over a finite field](../../../finite-group-theory.md#symplectic-group-over-a-finite-field) is

$$
Sp(V,B)=\{g\in GL(V):B(gx,gy)=B(x,y)\text{ for all }x,y\}.
$$

It acts simply transitively on ordered [symplectic bases](../../../linear-algebra.md#symplectic-basis): a [linear map](../../../vector-space.md#linear-map) between two such bases is uniquely specified and preserves all pairings, hence the whole [bilinear form](../../../linear-algebra.md#bilinear-form).

Count a first [hyperbolic pair](../../../linear-algebra.md#hyperbolic-pair) $(e_1,f_1)$. There are $q^{2m}-1$ choices for $e_1\ne0$. Nondegeneracy makes $B(e_1,-)$ a nonzero [linear functional](../../../linear-algebra.md#linear-functional), so there are $q^{2m-1}$ choices of $f_1$ with $B(e_1,f_1)=1$. Their span is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form), and its [symplectic orthogonal complement](../../../linear-algebra.md#symplectic-orthogonal-complement) is a [symplectic vector space](../../../linear-algebra.md#symplectic-vector-space) of dimension $2m-2$. Recursing, with $|Sp_0(q)|=1$, yields

$$
\boxed{|Sp_{2m}(q)|=\prod_{i=1}^m(q^{2i}-1)q^{2i-1}
=q^{m^2}\prod_{i=1}^m(q^{2i}-1).}
$$

The construction also proves the existence of the required [symplectic bases](../../../linear-algebra.md#symplectic-basis), in [characteristic](../../../algebra.md#characteristic-of-a-field) two as well as odd [characteristic](../../../algebra.md#characteristic-of-a-field).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Represent a subset by the coordinate [vector](../../../vector-space.md#vector) of its [indicator function](../../../measure-theory.md#indicator-function) in $\mathbb F_2^n$. [Symmetric difference](../../../set.md#symmetric-difference) then becomes coordinatewise addition, and the proposed pairing is the [dot product](../../../linear-algebra.md#dot-product)

$$
B(x,y)=\sum_{i=1}^nx_iy_i.
$$

It is a [symmetric bilinear form](../../../linear-algebra.md#symmetric-bilinear-form), and it is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) because its [Gram matrix](../../../linear-algebra.md#gram-matrix) in the singleton basis is the identity. Coordinate [permutations](../../../combinatorics.md#permutation) preserve the sum, so the natural $S_n$ action preserves the [bilinear form](../../../linear-algebra.md#bilinear-form).

Let $j=(1,\ldots,1)$, the [vector](../../../vector-space.md#vector) representing the full set. Then

$$
W=\langle j\rangle^\perp=\{x:\sum_ix_i=0\}
$$

is the even-weight subspace. For even $n$, $B(j,j)=n=0$ in $\mathbb F_2$, so $j\in W$. Moreover $B(x,x)=\sum_ix_i^2=\sum_ix_i=0$ for $x\in W$, making the restricted [bilinear form](../../../linear-algebra.md#bilinear-form) alternating. Nondegeneracy on the ambient space implies $W^\perp=\langle j\rangle$, so the radical of $B|_W$ is exactly

$$
W\cap W^\perp=\langle j\rangle.
$$

Thus it descends to an [alternating bilinear form](../../../linear-algebra.md#alternating-bilinear-form) on $W/\langle j\rangle$, independent of the representatives, and that quotient form has zero radical. **The induced form is [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form)**, and its dimension is $n-2$. This is the [symplectic quotient of the binary subset module](../../../finite-group-theory.md#symplectic-quotient-of-the-binary-subset-module); at $n=2$ it is the zero-dimensional [nondegenerate](../../../linear-algebra.md#nondegenerate-bilinear-form) space.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Take $n=6$ in 6(b). The [symplectic quotient of the binary subset module](../../../finite-group-theory.md#symplectic-quotient-of-the-binary-subset-module) has dimension four, so the action gives a [group homomorphism](../../../group-theory.md#group-homomorphism)

$$
S_6\longrightarrow Sp_4(2).
$$

It is injective. If $\sigma$ acts trivially on the quotient, every two-element subset $A$ has $\sigma A+A\in\{\varnothing,\Omega\}$. Hence $\sigma A$ equals $A$ or its complement. The latter has size four, whereas $\sigma A$ has size two; therefore $\sigma$ fixes every two-element subset. Given $i$, choose distinct $j,k\ne i$. It then fixes the intersection $\{i,j\}\cap\{i,k\}=\{i\}$, so it fixes each point and is the identity.

Finally 6(a) gives

$$
|Sp_4(2)|=2^4(2^2-1)(2^4-1)=16\cdot3\cdot15=720=|S_6|.
$$

An injective [group homomorphism](../../../group-theory.md#group-homomorphism) between these [finite groups](../../../group.md#finite-group) of the same order is surjective. Thus

$$
\boxed{Sp_4(2)\cong S_6.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
