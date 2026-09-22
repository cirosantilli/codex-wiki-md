# Paper 3

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2016/paperia_3.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2016/paperia_3.pdf)

**Table of contents**

- [1D](#1d)
  - [i](#1d/i)
    - [Solution](#1d/i/solution)
  - [ii](#1d/ii)
    - [Solution](#1d/ii/solution)
- [2D](#2d)
  - [Solution](#2d/solution)
- [3C](#3c)
  - [Solution](#3c/solution)
- [4C](#4c)
  - [Solution](#4c/solution)
- [5D](#5d)
  - [i](#5d/i)
    - [Solution](#5d/i/solution)
  - [ii](#5d/ii)
    - [Solution](#5d/ii/solution)
  - [iii](#5d/iii)
    - [Solution](#5d/iii/solution)
  - [iv](#5d/iv)
    - [Solution](#5d/iv/solution)
  - [v](#5d/v)
    - [Solution](#5d/v/solution)
- [6D](#6d)
  - [Solution](#6d/solution)
- [7D](#7d)
  - [Solution](#7d/solution)
- [8D](#8d)
  - [Solution](#8d/solution)
- [9C](#9c)
  - [a](#9c/a)
    - [Solution](#9c/a/solution)
  - [b](#9c/b)
    - [Solution](#9c/b/solution)
- [10C](#10c)
  - [Solution](#10c/solution)
- [11C](#11c)
  - [a](#11c/a)
    - [Solution](#11c/a/solution)
  - [b](#11c/b)
    - [Solution](#11c/b/solution)
  - [c](#11c/c)
    - [Solution](#11c/c/solution)
- [12C](#12c)
  - [a](#12c/a)
    - [Solution](#12c/a/solution)
  - [b](#12c/b)
    - [Solution](#12c/b/solution)
  - [c](#12c/c)
    - [Solution](#12c/c/solution)
  - [d](#12c/d)
    - [Solution](#12c/d/solution)

## 1D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="1d/i">i</h3>

↑ **Parent:** [1D](#1d)

<h4 id="1d/i/solution">Solution</h4>

↑ **Parent:** [I](#1d/i)

Suppose every [group commutator](../../../group.md#group-commutator) belongs to $H$. For $h\in H$ and $g\in G$, the particular [group commutator](../../../group.md#group-commutator) $h^{-1}g^{-1}hg$ belongs to $H$. Multiplying on the left by $h$ gives $g^{-1}hg\in H$. Thus $g^{-1}Hg\subseteq H$ for every $g$; applying the same inclusion to $g^{-1}$ gives the reverse inclusion. **Therefore $H$ is a [normal subgroup](../../../group-theory.md#normal-subgroup).**

We can now form the [quotient group](../../../group-theory.md#quotient-group). Its [group commutators](../../../group.md#group-commutator) are

$$
(aH)^{-1}(bH)^{-1}(aH)(bH)=(a^{-1}b^{-1}ab)H=H.
$$

A [group commutator](../../../group.md#group-commutator) is the [identity element](../../../group.md#identity-element) exactly when the two elements commute. Hence **$G/H$ is an [abelian group](../../../group.md#abelian-group)**. Equivalently, the hypothesis says that $H$ contains the [commutator subgroup](../../../group-theory.md#commutator-subgroup), so the quotient factors through the [abelianization](../../../group-theory.md#abelianization).

<h3 id="1d/ii">ii</h3>

↑ **Parent:** [1D](#1d)

<h4 id="1d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1d/ii)

Conversely, assume $H$ is a [normal subgroup](../../../group-theory.md#normal-subgroup) and the [quotient group](../../../group-theory.md#quotient-group) $G/H$ is an [abelian group](../../../group.md#abelian-group). Commuting the two [cosets](../../../group-theory.md#coset) $aH$ and $bH$ gives

$$
(a^{-1}b^{-1}ab)H=H,
$$

so every [group commutator](../../../group.md#group-commutator) $a^{-1}b^{-1}ab$ belongs to $H$. This proves the converse and completes the equivalence.

For the [dihedral group](../../../finite-group-theory.md#dihedral-group) of order ten, choose a rotation $r$ and a reflection $s$ with $r^5=s^2=1$ and $srs=r^{-1}$. Its rotation [subgroup](../../../group.md#subgroup) $\langle r\rangle$ is a [normal subgroup](../../../group-theory.md#normal-subgroup), and the quotient by it has order two, hence is an [abelian group](../../../group.md#abelian-group). Consequently the [commutator subgroup](../../../group-theory.md#commutator-subgroup) is contained in $\langle r\rangle$. On the other hand,

$$
[r,s]=r^{-1}s^{-1}rs=r^{-2}.
$$

Since $r^{-2}$ generates the order-five [cyclic group](../../../group.md#cyclic-group) $\langle r\rangle$, the [commutator subgroup](../../../group-theory.md#commutator-subgroup) is exactly $\langle r\rangle$. Every [abelian quotient](../../../group-theory.md#abelian-quotient) must kill this [subgroup](../../../group.md#subgroup). There are only two [subgroups](../../../group.md#subgroup) containing it, since the remaining quotient has prime order. **The complete list, including the trivial quotient, is**

$$
\boxed{D_{10}/\langle r\rangle\cong C_2,\qquad D_{10}/D_{10}\cong\{1\}.}
$$

This is the order-ten instance of the [abelianization of an odd dihedral group](../../../group-theory.md#abelianization-of-an-odd-dihedral-group).

## 2D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="2d/solution">Solution</h3>

↑ **Parent:** [2D](#2d)

[Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem) states that, for a [finite group](../../../group.md#finite-group) $G$ and a [subgroup](../../../group.md#subgroup) $H$,

$$
\boxed{|G|=[G:H]|H|.}
$$

To prove it, define an equivalence relation by $x\sim y$ when $x^{-1}y\in H$. Its classes are the left [cosets](../../../group-theory.md#coset) $xH$, which therefore partition $G$. Left multiplication by $x$ gives a [bijection](../../../function.md#bijection) $H\to xH$, so every [coset](../../../group-theory.md#coset) has $|H|$ elements. Counting this partition gives the formula; in particular $|H|$ divides $|G|$. Applying the theorem to the [cyclic subgroup](../../../group.md#cyclic-subgroup) generated by an element shows that its [order of a group element](../../../group-theory.md#order-of-a-group-element) divides $|G|$.

Write the given order-two [normal subgroup](../../../group-theory.md#normal-subgroup) as $N=\{1,z\}$. Conjugation must preserve $N$ and cannot send its nonidentity element to the identity, so $gzg^{-1}=z$ for all $g\in G$. Thus $z$ is in the [center of a group](../../../group-theory.md#center-of-a-group): a [normal subgroup of order two is central](../../../group-theory.md#normal-subgroup-of-order-two-is-central).

Choose $g\notin N$. By [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem), its [order of a group element](../../../group-theory.md#order-of-a-group-element) is $2$, $p$ or $2p$. It cannot have order two: since $z$ is central, the four distinct elements $1,z,g,zg$ would form a [subgroup](../../../group.md#subgroup) of order four, whereas $4$ does not divide $2p$ for odd $p$. If $g$ has order $2p$, it already generates $G$. Otherwise $g$ has order $p$, commutes with $z$, and $(gz)^k=1$ implies $g^k=z^{-k}\in\langle g\rangle\cap N=\{1\}$. Hence both $p$ and $2$ divide $k$, so $gz$ has order $2p$. **In either case**

$$
\boxed{G\cong C_{2p}.}
$$

## 3C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="3c/solution">Solution</h3>

↑ **Parent:** [3C](#3c)

The [chain rule](../../../calculus.md#chain-rule) along a smooth curve is

$$
\boxed{\frac{d}{dt}f(\mathbf X(t))=\sum_{i=1}^n\frac{\partial f}{\partial x_i}(\mathbf X(t))X_i'(t)=\nabla f(\mathbf X(t))\cdot\mathbf X'(t).}
$$

Differentiating the circular parametrization gives the [tangent vector](../../../differential-geometry.md#tangent-vector)

$$
\mathbf x'(t)=(-a\sin t,a\cos t)=(-y(t),x(t)).
$$

Thus the [chain rule](../../../calculus.md#chain-rule) turns the angular derivative of $u$ into $-yu_x+xu_y$. The given [partial differential equation](../../../partial-differential-equation.md) makes this equal to $u$, so along every portion of the circle inside the upper half-plane, $U(t)=u(\mathbf x(t))$ satisfies the [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) $U'=U$. Its solution is $U(t)=U(t_0)e^{t-t_0}$.

For the two specified points take $a=\sqrt2$. The initial point corresponds to $t_0=\pi/4$ and the terminal point to $t_1=3\pi/4$. The entire intervening arc lies in $y>0$, so no continuation outside the domain is used. **The requested value is**

$$
\boxed{u(-1,1)=10e^{\pi/2}.}
$$

These circular [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) also show locally that the general solution has the polar-coordinate form $u(r,\theta)=C(r)e^\theta$, with $0<\theta<\pi$; there is no requirement of angular periodicity on the upper half-plane.

## 4C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="4c/solution">Solution</h3>

↑ **Parent:** [4C](#4c)

Let $R$ be an [orthogonal matrix](../../../linear-algebra.md#orthogonal-matrix) describing a Cartesian change of coordinates, with transformed [vector](../../../vector-space.md#vector) components $v_i'=R_{ia}v_a$ and $w_j'=R_{jb}w_b$. Their [outer product](../../../vector-space.md#outer-product) transforms as

$$
T_{ij}'=v_i'w_j'=R_{ia}R_{jb}T_{ab},
$$

which is the transformation law of a second-order Cartesian [tensor](../../../linear-algebra.md#tensor). Here “rank two” counts tensor indices, not the [rank of a matrix](../../../vector-space.md#matrix-rank); a nonzero [outer product](../../../vector-space.md#outer-product) has matrix rank one.

For an [isotropic second-rank tensor](../../../linear-algebra.md#isotropic-second-rank-tensor), invariance means $RTR^T=T$ for every proper [rotation matrix](../../../linear-algebra.md#rotation-matrix). The half-turn matrices $\operatorname{diag}(1,-1,-1)$, $\operatorname{diag}(-1,1,-1)$ and $\operatorname{diag}(-1,-1,1)$ force all off-diagonal entries to vanish. Quarter-turns around coordinate axes then force the three diagonal entries to be equal. Conversely $RIR^T=I$, so **the most general second-rank [isotropic tensor](../../../linear-algebra.md#isotropic-tensor) is**

$$
\boxed{T_{ij}=\lambda\delta_{ij},\qquad\lambda\in\mathbb R.}
$$

Since $vw^T$ has matrix rank at most one, it cannot equal a nonzero scalar multiple of the three-dimensional identity. Thus its isotropy forces $vw^T=0$. If $v\ne0$, a nonzero component $v_i$ makes the entire $i$th row vanish only when $w=0$; the converse is immediate. **The required choices are exactly**

$$
\boxed{v=0\quad\text{or}\quad w=0.}
$$

For the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol), multilinearity and antisymmetry of the [determinant](../../../linear-algebra.md#determinant) give

$$
R_{ia}R_{jb}R_{kc}\epsilon_{abc}=(\det R)\epsilon_{ijk}=\epsilon_{ijk}
$$

for every $R\in SO(3)$. This proves the [rotation invariance of the Levi-Civita symbol](../../../calculus.md#rotation-invariance-of-the-levi-civita-symbol), hence its third-rank isotropy. The convention is invariance under proper rotations: under an orthogonal reflection $\det R=-1$, the sign reverses. Thus it is a [pseudotensor](../../../linear-algebra.md#pseudotensor) if transformations of both orientations are included.

## 5D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="5d/i">i</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/i/solution">Solution</h4>

↑ **Parent:** [I](#5d/i)

**No such nonabelian [group](../../../group.md) exists.** Every element, including the identity, satisfies $g^2=1$, so $g^{-1}=g$. For any $a,b$,

$$
ab=(ab)^{-1}=b^{-1}a^{-1}=ba.
$$

Therefore the [group](../../../group.md) is an [abelian group](../../../group.md#abelian-group). This proves that a [group of exponent two is abelian](../../../group.md#group-of-exponent-two-is-abelian) without any finiteness assumption.

<h3 id="5d/ii">ii</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5d/ii)

**An example is the [unitriangular group of degree three over F3](../../../finite-group-theory.md#unitriangular-group-of-degree-three-over-f3)**, consisting of

$$
M(a,b,c)=\begin{pmatrix}1&a&c\\0&1&b\\0&0&1\end{pmatrix},\qquad a,b,c\in\mathbb F_3.
$$

This is an [upper unitriangular group](../../../finite-group-theory.md#upper-unitriangular-group) of order $3^3=27$. Direct [matrix multiplication](../../../vector-space.md#matrix-multiplication) gives

$$
M(a,b,c)M(a',b',c')=M(a+a',b+b',c+c'+ab').
$$

The formula gives closure, identity $M(0,0,0)$, and inverse $M(-a,-b,ab-c)$; associativity follows from [matrix multiplication](../../../vector-space.md#matrix-multiplication). The two elements $M(1,0,0)$ and $M(0,1,0)$ do not commute: their products have respectively $c=1$ and $c=0$.

Every element has the form $I+N$ with $N^3=0$. Since the [finite field](../../../algebra.md#finite-field) $\mathbb F_3$ has characteristic three, the binomial expansion gives

$$
(I+N)^3=I+3N+3N^2+N^3=I.
$$

Hence every nonidentity element has order exactly three. **This is a nonabelian [finite group](../../../group.md#finite-group) with [exponent of a finite group](../../../group-theory.md#exponent-of-a-finite-group) equal to three.**

<h3 id="5d/iii">iii</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5d/iii)

The [order of a group element](../../../group-theory.md#order-of-a-group-element) represented by a [permutation](../../../combinatorics.md#permutation) is the [least common multiple](../../../number-theory.md#least-common-multiple) of its disjoint cycle lengths. An order divisible by nine therefore requires a [permutation cycle](../../../finite-group-theory.md#permutation-cycle) whose length is divisible by nine. In $S_9$ that must be a nine-cycle, which uses every letter and has order nine, not eighteen. **There is no element of $S_9$ of order eighteen.**

<h3 id="5d/iv">iv</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5d/iv)

Take two [disjoint permutation cycles](../../../finite-group-theory.md#disjoint-permutation-cycles) of lengths five and four:

$$
\boxed{\sigma=(1\,2\,3\,4\,5)(6\,7\,8\,9).}
$$

Disjoint [permutation cycles](../../../finite-group-theory.md#permutation-cycle) commute, and their powers act independently on their supports. Thus $\sigma^k=1$ exactly when both $5$ and $4$ divide $k$, so its [order of a group element](../../../group-theory.md#order-of-a-group-element) is $\operatorname{lcm}(5,4)=20$.

<h3 id="5d/v">v</h3>

↑ **Parent:** [5D](#5d)

<h4 id="5d/v/solution">Solution</h4>

↑ **Parent:** [V](#5d/v)

**No such [finite group](../../../group.md#finite-group) exists.** [Cayley theorem](../../../group-theory.md#cayley-s-theorem) embeds every [finite group](../../../group.md#finite-group) $G$ of order $n$ into $S_n$: the left-regular [group action](../../../group-theory.md#group-action) sends $g$ to the [permutation](../../../combinatorics.md#permutation) $x\mapsto gx$, and this is faithful because the image of the identity element is $g$.

To make every image permutation even, let $t=(n+1\ n+2)$, with support disjoint from the first $n$ letters. For $\sigma\in S_n$, let $e(\sigma)=0$ for an [even permutation](../../../finite-group-theory.md#even-permutation) and $e(\sigma)=1$ for an [odd permutation](../../../finite-group-theory.md#odd-permutation), and set

$$
\iota(\sigma)=\sigma t^{e(\sigma)}.
$$

The [sign homomorphism](../../../finite-group-theory.md#sign-homomorphism) gives $e(\sigma\tau)\equiv e(\sigma)+e(\tau)\pmod2$, and $t$ commutes with all permutations of the first $n$ letters. Thus $\iota$ is a [group homomorphism](../../../group-theory.md#group-homomorphism). It is injective by restriction to those letters, and its sign is $(-1)^{e(\sigma)}(-1)^{e(\sigma)}=1$. Consequently

$$
\boxed{G\hookrightarrow S_n\hookrightarrow A_{n+2}.}
$$

This is the [alternating-group embedding of a finite group](../../../group-theory.md#alternating-group-embedding-of-a-finite-group).

## 6D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="6d/solution">Solution</h3>

↑ **Parent:** [6D](#6d)

Every [permutation](../../../combinatorics.md#permutation) is a product of [transpositions](../../../combinatorics.md#transposition-permutation), since a cycle can be written

$$
(a_1\,a_2\,\ldots\,a_k)=(a_1\,a_k)\cdots(a_1\,a_2)
$$

with rightmost factors acting first. Define the [sign of a permutation](../../../finite-group-theory.md#sign-of-a-permutation) to be $(-1)^r$ for a product of $r$ [transpositions](../../../combinatorics.md#transposition-permutation). To prove that it is well defined without assuming parity, let $P_\sigma$ be the [permutation matrix](../../../vector-space.md#permutation-matrix) specified by $P_\sigma e_i=e_{\sigma(i)}$. Then $P_{\sigma\tau}=P_\sigma P_\tau$, and a [transposition](../../../combinatorics.md#transposition-permutation) exchanges two columns of the identity, so its [determinant](../../../linear-algebra.md#determinant) is $-1$. Any decomposition into $r$ [transpositions](../../../combinatorics.md#transposition-permutation) therefore has

$$
\det P_\sigma=(-1)^r.
$$

The left-hand side depends only on $\sigma$, proving well-definedness. Multiplicativity of the [determinant](../../../linear-algebra.md#determinant) now gives the [sign homomorphism](../../../finite-group-theory.md#sign-homomorphism):

$$
\boxed{\operatorname{sgn}(\sigma\tau)=\operatorname{sgn}(\sigma)\operatorname{sgn}(\tau).}
$$

For the first requested [group embedding](../../../group-theory.md#group-embedding), use the [faithful four-point action of GL2 over F2](../../../finite-group-theory.md#faithful-four-point-action-of-gl2-over-f2): label the four [vectors](../../../vector-space.md#vector) in $\mathbb F_2^2$ and let an invertible $2\times2$ [matrix](../../../vector-space.md#matrix) act on them by multiplication. Composition of these actions gives a [group homomorphism](../../../group-theory.md#group-homomorphism) $\psi:GL_2(\mathbb F_2)\to S_4$. If a matrix fixes every vector, it fixes both standard basis vectors and is the identity, so the action is faithful. The matrix

$$
B=\begin{pmatrix}0&1\\1&0\end{pmatrix}
$$

fixes $(0,0)$ and $(1,1)$ and exchanges $(1,0)$ with $(0,1)$. Its image is a single [transposition](../../../combinatorics.md#transposition-permutation), hence $\operatorname{sgn}(\psi(B))=-1$. **The composite sign map is nontrivial.**

For the second [group embedding](../../../group-theory.md#group-embedding), simply take

$$
\boxed{\phi(\sigma)=P_\sigma\in GL_n(\mathbb R),\qquad\det\phi(\sigma)=\operatorname{sgn}(\sigma).}
$$

The preceding multiplication formula proves the [group homomorphism](../../../group-theory.md#group-homomorphism) property, and $P_\sigma=I$ forces $\sigma(i)=i$ for every $i$, proving injectivity.

## 7D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="7d/solution">Solution</h3>

↑ **Parent:** [7D](#7d)

For a [group action](../../../group-theory.md#group-action) of a [finite group](../../../group.md#finite-group) $G$ on a set and a point $x$, the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) is

$$
\boxed{|Gx|=[G:G_x],\qquad |G|=|G_x||Gx|,}
$$

where $G_x=\{g:gx=x\}$ is the [stabilizer subgroup](../../../group-theory.md#stabilizer-subgroup). The map $gG_x\mapsto gx$ is well defined because elements of the same [coset](../../../group-theory.md#coset) act identically on $x$. If $gx=hx$, then $h^{-1}g\in G_x$, so their [cosets](../../../group-theory.md#coset) agree; every orbit point has the form $gx$, giving surjectivity. This is a [bijection](../../../function.md#bijection). [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem), $|G|=[G:H]|H|$ for any [subgroup](../../../group.md#subgroup) $H$, yields the counting formula.

Apply the [conjugation action](../../../group-theory.md#conjugation-action) of the [finite p-group](../../../finite-group-theory.md#finite-p-group) $G$ to its nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) $N$. Normality ensures the action stays inside $N$. The singleton [orbits of a group action](../../../group-theory.md#orbit-of-a-group-action) are exactly the elements of $N\cap Z(G)$. Every larger [orbit of a group action](../../../group-theory.md#orbit-of-a-group-action) has size a positive power of $p$, by the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) and [Lagrange's theorem](../../../group-theory.md#lagrange-s-theorem). Therefore

$$
|N|\equiv |N\cap Z(G)|\pmod p.
$$

Since $N$ is nontrivial, its order is divisible by $p$. The intersection contains the identity and has cardinality a positive multiple of $p$, so it contains a nonidentity element. This proves the [central intersection property of normal subgroups of finite p-groups](../../../finite-group-theory.md#central-intersection-property-of-normal-subgroups-of-finite-p-groups).

For the proper [subgroup](../../../group.md#subgroup) $H$, let $H$ act by left multiplication on the left [cosets](../../../group-theory.md#coset) $G/H$. A [coset](../../../group-theory.md#coset) $gH$ is fixed by every $h\in H$ exactly when $g^{-1}Hg\subseteq H$. Both groups have the same finite size, so this inclusion is equality; the fixed [cosets](../../../group-theory.md#coset) are precisely those with $g\in N_G(H)$. Hence their number is $[N_G(H):H]$. All non-singleton [orbits of a group action](../../../group-theory.md#orbit-of-a-group-action) have size divisible by $p$, so

$$
[G:H]\equiv[N_G(H):H]\pmod p.
$$

Since $H$ is proper, $[G:H]$ is a positive power of $p$ greater than one. The fixed-coset count is nonzero, because $H$ itself is fixed, and is divisible by $p$. Therefore **the [normalizer](../../../group-theory.md#normalizer) strictly contains $H$**:

$$
\boxed{[N_G(H):H]\geq p,\qquad\exists g\in G\setminus H:\ g^{-1}Hg=H.}
$$

This is the [normalizer condition for finite p-groups](../../../finite-group-theory.md#normalizer-condition-for-finite-p-groups). The proof also covers $H=\{1\}$, whose action fixes all [cosets](../../../group-theory.md#coset).

## 8D

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="8d/solution">Solution</h3>

↑ **Parent:** [8D](#8d)

The [Möbius group](../../../group-theory.md#mobius-group) consists of all [Möbius transformations](../../../group-theory.md#mobius-transformation) of the [Riemann sphere](../../../complex-analysis.md#riemann-sphere) $\mathbb C_\infty=\mathbb C\cup\{\infty\}$, with operation [function composition](../../../algebra.md#function-composition). A nonzero-determinant [matrix](../../../vector-space.md#matrix) $M=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ represents the map $z\mapsto(az+b)/(cz+d)$. If $c\ne0$, its pole $-d/c$ maps to $\infty$ and $\infty$ maps to $a/c$; if $c=0$, the map is affine and fixes $\infty$. Nonzero scalar multiples of $M$ represent the same transformation.

Define $\phi(M)$ by this action for $M\in SL_2(\mathbb C)$. Substitution of fractional-linear expressions shows $\phi(MN)=\phi(M)\circ\phi(N)$, so $\phi$ is a [group homomorphism](../../../group-theory.md#group-homomorphism). Any invertible matrix can be rescaled into the [special linear group](../../../group-theory.md#special-linear-group): choose $\lambda\in\mathbb C^\times$ with $\lambda^2\det M=1$, which is possible because every nonzero complex number has a square root. This does not change the transformation, proving surjectivity. A transformation represented by $M$ is the identity only if fixing $0$, $\infty$ and $1$ forces $b=c=0$ and $a=d$. The determinant-one condition then gives $a^2=1$. **Thus**

$$
\boxed{\ker\phi=\{I,-I\},\qquad\mathcal M\cong SL_2(\mathbb C)/\{\pm I\}.}
$$

For the fixed-point claim, a nonidentity [Möbius transformation](../../../group-theory.md#mobius-transformation) has at least one [fixed point of a Möbius transformation](../../../group-theory.md#fixed-point-of-a-mobius-transformation): when $c\ne0$ the finite fixed points solve a quadratic, and when $c=0$ infinity is fixed. A quadratic shows there can be no more than two distinct fixed points unless the transformation is the identity. Suppose there is exactly one. Conjugate it to infinity by a [Möbius transformation](../../../group-theory.md#mobius-transformation). The resulting map has form $z\mapsto az+b$, since it fixes infinity. If $a\ne1$ it also has the finite fixed point $b/(1-a)$, a contradiction. Hence it is $z\mapsto z+b$ with $b\ne0$. Its $m$th power is $z\mapsto z+mb$, never the identity for $m>0$. Conjugation preserves order, so **a nonidentity finite-order [Möbius transformation](../../../group-theory.md#mobius-transformation) has exactly two fixed points**.

Now let $K$ be a [finite abelian subgroup of the Möbius group](../../../group-theory.md#finite-abelian-subgroup-of-the-mobius-group). First suppose it contains an element $g$ of order greater than two. Conjugate the two fixed points of $g$ to $0$ and $\infty$, so $g(z)=\zeta z$, with $\zeta$ a [root of unity](../../../algebra.md#root-of-unity) of order greater than two. Every element $h$ commuting with $g$ permutes its fixed-point set, because $g(h(p))=h(g(p))=h(p)$. A [Möbius transformation](../../../group-theory.md#mobius-transformation) preserving each of $0,\infty$ is $h(z)=az$; one exchanging them is $h(z)=a/z$. In the second case $hg(z)=a/(\zeta z)$ and $gh(z)=\zeta a/z$, so commuting would force $\zeta^2=1$, impossible. Thus all elements of $K$ are scalings. A [finite subgroup of a field multiplicative group is cyclic](../../../group-theory.md#finite-subgroup-of-a-field-multiplicative-group-is-cyclic); here one can see this directly by choosing the least common multiple $m$ of all element orders and observing that the scalars lie among the $m$th roots of unity, a [cyclic group](../../../group.md#cyclic-group). Hence $K$ is cyclic.

Otherwise every nonidentity element of $K$ has order two. If $K$ is nontrivial, choose $g$ and conjugate it to $z\mapsto-z$. The action of $K$ on $\{0,\infty\}$ has image of order at most two. Its kernel consists of scalings $z\mapsto az$, and the order-two condition forces $a^2=1$, so the kernel has at most two elements. Hence $|K|\leq4$. Orders one and two give cyclic groups; order four with all nonidentity elements involutions gives $C_2\times C_2$, generated by any two distinct nonidentity elements. Both possibilities occur: scalings by roots of unity give every finite cyclic group, and $\{z,-z,1/z,-1/z\}$ gives the Klein four group. **The classification is**

$$
\boxed{K\text{ is cyclic, or }K\cong C_2\times C_2.}
$$

## 9C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="9c/a">a</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/a/solution">Solution</h4>

↑ **Parent:** [A](#9c/a)

A [conservative vector field](../../../calculus.md#conservative-vector-field) on $\mathbb R^n$ is a [vector field](../../../calculus.md#vector-field) $\mathbf V=\nabla F$ for a globally defined smooth [potential of a conservative vector field](../../../calculus.md#potential-of-a-conservative-vector-field) $F$. The [chain rule](../../../calculus.md#chain-rule) gives

$$
\int_C\mathbf V\cdot d\mathbf x=F(\text{endpoint})-F(\text{startpoint}),
$$

so its [line integral](../../../calculus.md#line-integral) is [path independent](../../../calculus.md#path-independence).

[Green theorem](../../../calculus.md#green-theorem) states that, for a bounded planar region $D$ with piecewise smooth boundary and continuously differentiable $P,Q$ on a neighbourhood of its closure,

$$
\boxed{\oint_{\partial D}(P\,dx+Q\,dy)=\iint_D(Q_x-P_y)\,dx\,dy.}
$$

The boundary is positively oriented: the region lies on the left while it is traversed, so outer components run counterclockwise and hole boundaries clockwise.

For the proposed [potential of a conservative vector field](../../../calculus.md#potential-of-a-conservative-vector-field), the [fundamental theorem of calculus](../../../calculus.md#fundamental-theorem-of-calculus) and [differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) give

$$
F_y(x,y)=Q(x,y),\qquad F_x(x,y)=P(x,0)+\int_0^yQ_x(x,s)\,ds.
$$

Since $Q_x=P_y$, the last integral equals $P(x,y)-P(x,0)$, including negative $y$ with the usual signed-integral convention. Hence **the proposed potential is global and**

$$
\boxed{\nabla F=(P,Q)=\mathbf V.}
$$

The fact that the [vector field](../../../calculus.md#vector-field) is defined on all of $\mathbb R^2$ ensures both straight integration segments stay inside its domain; a hole in the domain could obstruct a global potential.

<h3 id="9c/b">b</h3>

↑ **Parent:** [9C](#9c)

<h4 id="9c/b/solution">Solution</h4>

↑ **Parent:** [B](#9c/b)

Integrating the oscillatory term together with the constant components gives a [potential of a conservative vector field](../../../calculus.md#potential-of-a-conservative-vector-field)

$$
\boxed{F(x,y)=x+2y+\frac{\sin(2\pi(x+y))}{2\pi}.}
$$

Direct [partial derivatives](../../../calculus.md#partial-derivative) recover both components of $\mathbf V$, proving it is a [conservative vector field](../../../calculus.md#conservative-vector-field). Its [line integral](../../../calculus.md#line-integral) is therefore [path independent](../../../calculus.md#path-independence). At an integer endpoint $(m,n)$, the sine term vanishes, so **for any of the specified paths**

$$
\boxed{\int_C\mathbf V\cdot d\mathbf x=m+2n.}
$$

Any other potential has the same [gradient](../../../calculus.md#gradient), so differs from $F$ by a constant on the connected plane. In particular every potential changes by $1$ under $x\mapsto x+1$ and by $2$ under $y\mapsto y+1$. Equivalently the integral from $(0,0)$ to $(1,0)$ is $1$, whereas a unit-periodic potential would make that difference zero. **There is no potential periodic with period one in both coordinate directions.** This is an example of how [periods obstruct a periodic potential](../../../calculus.md#periods-obstruct-a-periodic-potential): a periodic [vector field](../../../calculus.md#vector-field) need not have a periodic potential.

## 10C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="10c/solution">Solution</h3>

↑ **Parent:** [10C](#10c)

For a smooth map $\mathbf u$, the [Jacobian determinant](../../../calculus.md#jacobian-determinant) is the determinant of its [Jacobian matrix](../../../calculus.md#jacobian-matrix) $A_{ai}=\partial_i u_a$. In [Einstein summation convention](../../../linear-algebra.md#einstein-notation),

$$
J[\mathbf u]=\det A=\frac16\epsilon_{ijk}\epsilon_{abc}(\partial_i u_a)(\partial_j u_b)(\partial_k u_c).
$$

Differentiate the supplied expression for $V_i$ by the [product rule](../../../calculus.md#product-rule). The term differentiating $\partial_j u_a$ vanishes because $\partial_i\partial_j u_a$ is symmetric in $i,j$, while $\epsilon_{ijk}$ is antisymmetric; the term differentiating $\partial_k u_b$ vanishes similarly. Only differentiation of $u_c$ remains:

$$
\partial_iV_i=\frac16\epsilon_{ijk}\epsilon_{abc}(\partial_j u_a)(\partial_k u_b)(\partial_i u_c)=J[\mathbf u].
$$

The last equality follows by the cyclic relabelling $(i,j,k)\mapsto(j,k,i)$, which has positive sign. This proves the [Jacobian determinant as a divergence](../../../calculus.md#jacobian-determinant-as-a-divergence) identity.

For a composition $\mathbf w=\mathbf u\circ\mathbf v$, the [chain rule](../../../calculus.md#chain-rule) gives

$$
\partial_iw_a(\mathbf x)=(\partial_bu_a)(\mathbf v(\mathbf x))\,\partial_iv_b(\mathbf x),\qquad D\mathbf w(\mathbf x)=D\mathbf u(\mathbf v(\mathbf x))D\mathbf v(\mathbf x).
$$

Taking [determinants](../../../linear-algebra.md#determinant) yields

$$
\boxed{J[\mathbf w](\mathbf x)=J[\mathbf u](\mathbf v(\mathbf x))J[\mathbf v](\mathbf x).}
$$

For the first-order perturbation, use [spatial derivative control in perturbations of the identity map](../../../calculus.md#spatial-derivative-control-in-perturbations-of-the-identity-map): the usual smooth-family interpretation gives $D\mathbf u_t=I+tD\mathbf F+o(t)$ locally. Multilinearity of the [determinant](../../../linear-algebra.md#determinant) shows that its linear term comes from choosing one column of $tD\mathbf F$ and all other columns from $I$. This gives the [trace](../../../linear-algebra.md#matrix-trace):

$$
\boxed{J[\mathbf u_t]=1+t\operatorname{tr}(D\mathbf F)+o(t)=1+t\nabla\cdot\mathbf F+o(t),\qquad Q=\nabla\cdot\mathbf F.}
$$

The regularity qualification matters: a pointwise $o(t)$ remainder for maps does not by itself give an $o(t)$ remainder for spatial derivatives. For instance $(x+t^2\sin(x/t^2),y,z)$ has a uniform $o(t)$ displacement and $\mathbf F=0$, but its [Jacobian determinant](../../../calculus.md#jacobian-determinant) at $x=0$ is $2$ for $t\ne0$. Thus the first expansion needs the remainder in $C^1$ locally, or an equivalent smoothness assumption on the family.

Under the subsequent group law, $\mathbf u_0$ is the identity and $\mathbf u_{-t}$ is the inverse of $\mathbf u_t$. Write $j(t,\mathbf x)=J[\mathbf u_t](\mathbf x)$. Applying the composition formula to $\mathbf u_{t+h}=\mathbf u_h\circ\mathbf u_t$ and the short-time expansion gives the [Jacobian evolution of a smooth flow](../../../dynamical-systems.md#jacobian-evolution-of-a-smooth-flow):

$$
\partial_tj(t,\mathbf x)=(\nabla\cdot\mathbf F)(\mathbf u_t(\mathbf x))j(t,\mathbf x),\qquad j(0,\mathbf x)=1.
$$

Hence

$$
j(t,\mathbf x)=\exp\left(\int_0^t(\nabla\cdot\mathbf F)(\mathbf u_s(\mathbf x))\,ds\right).
$$

If only the pointwise generator expansion is assumed initially, the group law still gives $\partial_t\mathbf u_t(\mathbf x)=\mathbf F(\mathbf u_t(\mathbf x))$. Uniqueness and smooth dependence for this smooth [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation) make it a smooth [flow map](../../../dynamical-systems.md#flow-map), thereby justifying the differentiated expansion used above. Thus **a divergence-free generator has**

$$
\boxed{J[\mathbf u_t]=1\quad\text{for every }t.}
$$

By the [change of variables formula](../../../calculus.md#change-of-variables-formula), these maps preserve ordinary Euclidean volume and orientation. This is the Euclidean instance of a [volume-preserving vector field](../../../differential-form.md#volume-preserving-vector-field).

## 11C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="11c/a">a</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/a/solution">Solution</h4>

↑ **Parent:** [A](#11c/a)

The [product rule](../../../calculus.md#product-rule) for the [divergence](../../../calculus.md#divergence) gives

$$
\nabla\cdot(u\nabla v)=\nabla u\cdot\nabla v+u\nabla^2v,\qquad\nabla\cdot(v\nabla u)=\nabla v\cdot\nabla u+v\nabla^2u.
$$

Subtracting cancels the two [gradient](../../../calculus.md#gradient) products. **Therefore**

$$
\boxed{\nabla\cdot(u\nabla v-v\nabla u)=u\nabla^2v-v\nabla^2u.}
$$

To obtain the requested order of terms, apply this identity with $u,v$ interchanged and use the [divergence theorem](../../../calculus.md#divergence-theorem) on the spherical shell. On the outer sphere the shell's outward [unit normal](../../../differential-geometry.md#unit-normal) is $\widehat{\mathbf r}$; on the inner sphere it is $-\widehat{\mathbf r}$. Write $\partial_r=\widehat{\mathbf r}\cdot\nabla$ on both spheres. Then the resulting [Green second identity](../../../partial-differential-equation.md#green-second-identity) is

$$
\boxed{\int_{\rho\leq|\mathbf x|\leq r}(v\nabla^2u-u\nabla^2v)\,dV=\int_{|\mathbf x|=r}(v\partial_ru-u\partial_rv)\,dS-\int_{|\mathbf x|=\rho}(v\partial_ru-u\partial_rv)\,dS.}
$$

The minus sign records the inward radial direction of the shell's normal on its inner boundary. Thus the normal derivatives in the displayed difference are outward from each individual ball; using shell-outward normals instead would put a plus sign between the two boundary integrals.

<h3 id="11c/b">b</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/b/solution">Solution</h4>

↑ **Parent:** [B](#11c/b)

In [Einstein summation convention](../../../linear-algebra.md#einstein-notation), the [curl](../../../calculus.md#curl) is

$$
(\nabla\times\mathbf V)_i=\epsilon_{ijk}\partial_jV_k.
$$

Apply another [curl](../../../calculus.md#curl) and use the [contraction of two Levi-Civita symbols](../../../calculus.md#contraction-of-two-levi-civita-symbols):

$$
\begin{aligned}(\nabla\times(\nabla\times\mathbf V))_i&=\epsilon_{ijk}\epsilon_{klm}\partial_j\partial_lV_m\\&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})\partial_j\partial_lV_m\\&=\partial_i(\partial_jV_j)-\partial_j\partial_jV_i.\end{aligned}
$$

Smoothness allows the [partial derivatives](../../../calculus.md#partial-derivative) to commute. **This proves the [curl of the curl identity](../../../calculus.md#curl-of-the-curl-identity):**

$$
\boxed{\nabla\times(\nabla\times\mathbf V)=\nabla(\nabla\cdot\mathbf V)-\nabla^2\mathbf V.}
$$

<h3 id="11c/c">c</h3>

↑ **Parent:** [11C](#11c)

<h4 id="11c/c/solution">Solution</h4>

↑ **Parent:** [C](#11c/c)

The identity [divergence of a curl is zero](../../../calculus.md#divergence-of-a-curl-is-zero) follows by the symmetry of second [partial derivatives](../../../calculus.md#partial-derivative) and antisymmetry of the [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol). Therefore

$$
\boxed{\nabla\cdot\mathbf J=\nabla\cdot(\nabla\times\mathbf B)=0.}
$$

If $\mathbf B=\nabla\times\mathbf A$ and $\mathbf A$ is in [Coulomb gauge](../../../electromagnetism.md#coulomb-gauge), the [curl of the curl identity](../../../calculus.md#curl-of-the-curl-identity) gives $\mathbf J=-\nabla^2\mathbf A$. Apply the supplied scalar [Poisson equation](../../../partial-differential-equation.md#poisson-equation) representation to each component of the decaying [vector potential](../../../calculus.md#vector-potential). In the units of this problem the [Coulomb-gauge vector potential of a localized steady current](../../../electromagnetism.md#coulomb-gauge-vector-potential-of-a-localized-steady-current) is

$$
\boxed{\mathbf A(\mathbf x)=\int_{\mathbb R^3}\frac{\mathbf J(\mathbf y)}{4\pi|\mathbf x-\mathbf y|}\,d^3y.}
$$

Here one needs $\mathbf A=O(|\mathbf x|^{-1})$, $\nabla\mathbf A=O(|\mathbf x|^{-2})$ and enough localization of $\mathbf J$ for the stated representation and differentiations. A smooth compactly supported [current density](../../../electromagnetism.md#current-density) is a sufficient convenient case. The local differential equations and gauge alone do not impose these conditions: $\mathbf A=(-y,x,0)$, $\mathbf B=(0,0,2)$, $\mathbf J=0$ satisfy them but do not satisfy the displayed integral formula. The formula selects the decaying solution, excluding nondecaying homogeneous [harmonic functions](../../../partial-differential-equation.md#harmonic-function).

With $\mathbf r=\mathbf x-\mathbf y$, the [gradient](../../../calculus.md#gradient) of the kernel is $\nabla_x(1/|\mathbf r|)=-\mathbf r/|\mathbf r|^3$. Since $\mathbf J(\mathbf y)$ is independent of $\mathbf x$,

$$
\nabla_x\times\left(\frac{\mathbf J(\mathbf y)}{4\pi|\mathbf r|}\right)=\frac{\mathbf J(\mathbf y)\times\mathbf r}{4\pi|\mathbf r|^3}.
$$

Thus **taking the [curl](../../../calculus.md#curl) gives the [Biot-Savart law](../../../electromagnetism.md#biot-savart-law) in the problem's normalization**:

$$
\boxed{\mathbf B(\mathbf x)=\int_{\mathbb R^3}\frac{\mathbf J(\mathbf y)\times(\mathbf x-\mathbf y)}{4\pi|\mathbf x-\mathbf y|^3}\,d^3y.}
$$

Finally, change variables $\mathbf z=\mathbf x-\mathbf y$ in the integral for $\mathbf A$. This keeps the singular kernel independent of the differentiation variable:

$$
\mathbf A(\mathbf x)=\int_{\mathbb R^3}\frac{\mathbf J(\mathbf x-\mathbf z)}{4\pi|\mathbf z|}\,d^3z,\qquad\nabla\cdot\mathbf A(\mathbf x)=\int_{\mathbb R^3}\frac{(\nabla\cdot\mathbf J)(\mathbf x-\mathbf z)}{4\pi|\mathbf z|}\,d^3z=0.
$$

For smooth localized $\mathbf J$, [differentiation under the integral sign](../../../analysis.md#differentiation-under-the-integral-sign) is legitimate: $1/|\mathbf z|$ is locally integrable in three dimensions, and on a bounded neighbourhood of $\mathbf x$ the translated sources and their derivatives have common compact support. **The integral indeed satisfies [Coulomb gauge](../../../electromagnetism.md#coulomb-gauge).**

## 12C

↑ **Parent:** [Paper 3](paper-3.md)

<h3 id="12c/a">a</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/a/solution">Solution</h4>

↑ **Parent:** [A](#12c/a)

The [curl](../../../calculus.md#curl) is constant:

$$
\nabla\times\mathbf F=(\partial_yF_z-\partial_zF_y,\partial_zF_x-\partial_xF_z,\partial_xF_y-\partial_yF_x)=(1,1,1).
$$

Orient the spanning planar disk by the [unit normal](../../../differential-geometry.md#unit-normal) $\mathbf n=(a,b,c)$ and orient its boundary by the right-hand rule, equivalently counterclockwise when viewed from the side towards which $\mathbf n$ points. [Stokes theorem](../../../calculus.md#stokes-theorem) converts the [line integral](../../../calculus.md#line-integral) to a constant [flux integral](../../../calculus.md#flux-integral) through a disk of area $\pi R^2$. **With this orientation**

$$
\boxed{\oint_C\mathbf F\cdot d\mathbf x=\pi R^2(a+b+c).}
$$

Reversing the orientation changes the sign. The centre of the circle does not enter because the [curl](../../../calculus.md#curl) is constant.

<h3 id="12c/b">b</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/b/solution">Solution</h4>

↑ **Parent:** [B](#12c/b)

Symmetry of the derivative matrix means $\partial_iF_j=\partial_jF_i$. Contracting this symmetric pair with the antisymmetric [Levi-Civita symbol](../../../calculus.md#levi-civita-symbol) gives

$$
(\nabla\times\mathbf F)_k=\epsilon_{kij}\partial_iF_j=0.
$$

Every circle bounds its planar disk, and the [vector field](../../../calculus.md#vector-field) is smooth on all of $\mathbb R^3$, including that disk. [Stokes theorem](../../../calculus.md#stokes-theorem) therefore gives **for either orientation**

$$
\boxed{\oint_C\mathbf F\cdot d\mathbf x=\int_D(\nabla\times\mathbf F)\cdot\mathbf n\,dS=0.}
$$

The global domain is essential to this argument; the same local symmetry condition on a domain with a hole need not make every closed-curve [line integral](../../../calculus.md#line-integral) vanish.

<h3 id="12c/c">c</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/c/solution">Solution</h4>

↑ **Parent:** [C](#12c/c)

Away from the origin, the given [vector field](../../../calculus.md#vector-field) is the [gradient](../../../calculus.md#gradient) of the globally single-valued radius:

$$
\mathbf F=\nabla r,\qquad r=\sqrt{x^2+y^2+z^2}.
$$

The sphere has centre $(5,3,2)$, at distance $\sqrt{38}$ from the origin, and radius one. Its intersection circle is therefore wholly away from the origin, since every point on the sphere has distance at least $\sqrt{38}-1>0$. Along the closed curve the [chain rule](../../../calculus.md#chain-rule) gives $\mathbf F\cdot d\mathbf x=dr$. **Consequently, independently of orientation,**

$$
\boxed{\oint_C\mathbf F\cdot d\mathbf x=0.}
$$

The intersection is nondegenerate: the centre's distance from the plane is $4/\sqrt{35}<1$. No parametrization of the resulting circle is needed because $r$ is a [potential of a conservative vector field](../../../calculus.md#potential-of-a-conservative-vector-field) throughout the punctured space.

<h3 id="12c/d">d</h3>

↑ **Parent:** [12C](#12c)

<h4 id="12c/d/solution">Solution</h4>

↑ **Parent:** [D](#12c/d)

Set $s=x^2+y^2>0$. The first two components of the [curl](../../../calculus.md#curl) vanish since the horizontal components are independent of $z$ and the last component depends only on $z$. For the third,

$$
\partial_x\left(\frac{x}{s}\right)=\frac{y^2-x^2}{s^2},\qquad\partial_y\left(\frac{-y}{s}\right)=\frac{y^2-x^2}{s^2},
$$

so **this is a [curl-free vector field](../../../calculus.md#irrotational-vector-field) everywhere in its domain**:

$$
\boxed{\nabla\times\mathbf F=0.}
$$

Choose the orientation in which the projection onto the $xy$-plane runs counterclockwise, and parametrize

$$
\mathbf x(t)=(\cos t,\sin t,200+\cos t),\qquad0\leq t\leq2\pi.
$$

On this curve the horizontal contribution is $(-\sin t,\cos t)\cdot(-\sin t,\cos t)\,dt=dt$, while the vertical contribution is $z\,dz=d(z^2/2)$. Its integral over a closed curve is zero. **Therefore**

$$
\boxed{\oint_C\mathbf F\cdot d\mathbf x=2\pi,}
$$

with $-2\pi$ for the opposite orientation. This does not contradict [Stokes theorem](../../../calculus.md#stokes-theorem): the planar disk spanning this curve meets the excluded $z$-axis at $(0,0,200)$, where the [vector field](../../../calculus.md#vector-field) is undefined. The horizontal one-form is the angular differential and records one winding about that axis; thus this [curl-free vector field](../../../calculus.md#irrotational-vector-field) has no single-valued global [potential of a conservative vector field](../../../calculus.md#potential-of-a-conservative-vector-field) on its domain.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
