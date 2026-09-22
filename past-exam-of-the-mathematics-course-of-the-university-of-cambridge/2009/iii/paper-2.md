# Paper 2

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper2.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper2.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)

## 1

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [composition series](../../../finite-group-theory.md#composition-series) is a subnormal chain whose nontrivial successive quotients are simple. The [Jordan–Hölder theorem](../../../finite-group-theory.md#jordan-holder-theorem) asserts that any two [composition series](../../../finite-group-theory.md#composition-series) of a [finite group](../../../group.md#finite-group) have the same length and the same multiset of simple factors, up to [isomorphism](../../../algebra.md#isomorphism). Existence follows by successively choosing maximal proper [normal subgroups](../../../group-theory.md#normal-subgroup) until the identity is reached.

For uniqueness, induct on the [group](../../../group.md) order. Let $A,B$ be the penultimate terms of two series. If $A=B$, apply induction to that [subgroup](../../../group.md#subgroup) and add the common top factor. If $A\ne B$, their normality and maximality give $AB=G$. Put $C=A\cap B$. The [isomorphism](../../../algebra.md#isomorphism) theorems give

$$
A/C\cong G/B,\qquad B/C\cong G/A.
$$

Both are simple. Take any [composition series](../../../finite-group-theory.md#composition-series) of $C$. Appending $A$ to it gives a series for $A$, so induction identifies the factors of the original series inside $A$ with the factors of $C$ together with $G/B$. Similarly the factors inside $B$ are those of $C$ together with $G/A$. Adding the respective top factors produces the same multiset in both cases. This proves uniqueness, including multiplicities and length.

A [normal subgroup](../../../group-theory.md#normal-subgroup) $K$ of order two is central because its [automorphism group](../../../group-theory.md#automorphism-group) is trivial. By Jordan–Hölder, a [composition series](../../../finite-group-theory.md#composition-series) through $K$ leaves the simple quotient $G/K\cong A_5$. The image of $Z(G)$ in this quotient is central and hence trivial, since $A_5$ is nonabelian simple. Thus

$$
\boxed{Z(G)=K.}
$$

The [symmetric group](../../../finite-group-theory.md#symmetric-group) $S_5$ has trivial [group center](../../../group-theory.md#center-of-a-group): [conjugation](../../../group-theory.md#conjugation) of each [transposition](../../../combinatorics.md#transposition-permutation) by a central [permutation](../../../combinatorics.md#permutation) must preserve its two-element support, forcing the [permutation](../../../combinatorics.md#permutation) to fix every point. Since its [Jordan–Hölder factors](../../../finite-group-theory.md#jordan-holder-factor) are $A_5$ and $C_2$, a [normal subgroup](../../../group-theory.md#normal-subgroup) of order two would equal that trivial [group center](../../../group-theory.md#center-of-a-group), a contradiction.

Identify $C_2=\{1,-1\}$ and put $D=1\times A_5$ in $C_2\times S_5$. Its three maximal [normal subgroups](../../../group-theory.md#normal-subgroup) are

$$
M_1=C_2\times A_5,\quad M_2=1\times S_5,\quad
M_3=\{(\operatorname{sgn}\sigma,\sigma):\sigma\in S_5\}.
$$

They are the three [kernels](../../../linear-algebra.md#kernel-of-a-linear-map) of nonzero maps from the [abelianization](../../../group-theory.md#abelianization) $C_2^2$ to $C_2$. There is no quotient $A_5$: a central $C_2$ must map trivially, while $S_5$ has no quotient $A_5$. The latter follows from its [normal subgroups](../../../group-theory.md#normal-subgroup) $1,A_5,S_5$, which can themselves be obtained by intersecting with the simple [subgroup](../../../group.md#subgroup) $A_5$ and using its trivial [centralizer](../../../group-theory.md#centralizer). The complete list of [composition series](../../../finite-group-theory.md#composition-series) is

$$
\boxed{\begin{aligned}
1&<C_2\times1<M_1<C_2\times S_5,\\
1&<D<M_1<C_2\times S_5,\\
1&<D<M_2<C_2\times S_5,\\
1&<D<M_3<C_2\times S_5.
\end{aligned}}
$$

Within $M_1$ the two direct factors are the only maximal [normal subgroups](../../../group-theory.md#normal-subgroup); within each of $M_2,M_3\cong S_5$ the only such [subgroup](../../../group.md#subgroup) is its copy of $A_5$. Hence **there are exactly four series**.

For $S_5\times S_5$, put $D=A_5\times A_5$, $X=A_5\times1$, $Y=1\times A_5$ and

$$
M_L=A_5\times S_5,\quad M_R=S_5\times A_5,\quad
M_D=\{(\sigma,\rho):\operatorname{sgn}\sigma=\operatorname{sgn}\rho\}.
$$

Again these are exactly the maximal [normal subgroups](../../../group-theory.md#normal-subgroup): they are the three cyclic quotient [kernels](../../../linear-algebra.md#kernel-of-a-linear-map), and there is no simple quotient $A_5$ of the whole product. All series are

$$
\boxed{1<T<D<M<S_5\times S_5\quad(T=X\text{ or }Y,\ M=M_L,M_R,M_D),}
$$

together with

$$
\boxed{1<Y<1\times S_5<M_L<S_5\times S_5,\qquad
1<X<S_5\times1<M_R<S_5\times S_5.}
$$

To verify exhaustiveness, $M_L$ has maximal [normal subgroups](../../../group-theory.md#normal-subgroup) $D$ and $1\times S_5$, and $M_R$ has $D$ and $S_5\times1$. A quotient $A_5$ of a direct product can receive a nontrivial image from only one simple factor, since the images commute and $A_5$ has trivial [group center](../../../group-theory.md#center-of-a-group). The remaining maximal-normal possibility is $M_D$. Its derived [subgroup](../../../group.md#subgroup) is $D$, because both alternating factors are perfect. A hypothetical quotient $A_5$ would project one alternating factor isomorphically and kill the other, but [conjugation](../../../group-theory.md#conjugation) by an odd diagonal element induces an [outer automorphism](../../../group-theory.md#outer-automorphism-of-a-group) on that surviving factor, impossible inside $A_5$. Odd [conjugation](../../../group-theory.md#conjugation) is outer because otherwise an odd [permutation](../../../combinatorics.md#permutation) times an even one would centralize $A_5$; a [permutation](../../../combinatorics.md#permutation) commuting with every [three-cycle](../../../finite-group-theory.md#three-cycle) fixes every three-element support and is the identity. Thus $D$ is the only maximal [normal subgroup](../../../group-theory.md#normal-subgroup) of $M_D$. Finally the only maximal [normal subgroups](../../../group-theory.md#normal-subgroup) of $D$ are $X,Y$: [normal subgroups](../../../group-theory.md#normal-subgroup) of a product of two centerless [simple groups](../../../finite-group-theory.md#simple-group) are products of the factors, as follows by commutating with each factor. This proves **exactly eight series** and the classification of [composition chains in products with S5](../../../finite-group-theory.md#composition-chains-in-products-with-s5).

For $SL_2(5)$, commuting with both elementary upper and lower [transvections](../../../vector-space.md#transvection) forces a central [matrix](../../../vector-space.md#matrix) to be scalar. A scalar $\lambda I$ has [determinant](../../../linear-algebra.md#determinant) $\lambda^2$, so

$$
\boxed{Z(SL_2(5))=\{I,-I\}.}
$$

If $g^2=I$, characteristic five makes $g$ diagonalizable with eigenvalues in $\{1,-1\}$. [Determinant](../../../linear-algebra.md#determinant) one rules out one of each, so the unique nonidentity [involution](../../../group-theory.md#involution) is $-I$. An index-two [subgroup](../../../group.md#subgroup) would have order $60$ and, by the [Cauchy theorem for groups](../../../finite-group-theory.md#cauchy-theorem-for-groups), contain that [involution](../../../group-theory.md#involution) and hence the [group center](../../../group-theory.md#center-of-a-group). Its image in $PSL_2(5)$ would have index two. The simplicity and identification $PSL_2(5)\cong A_5$ are established by the independent [matrix](../../../vector-space.md#matrix) argument in Solution 4; a [simple group](../../../finite-group-theory.md#simple-group) has no proper index-two [subgroup](../../../group.md#subgroup). Therefore **$SL_2(5)$ has no [subgroup](../../../group.md#subgroup) of index two**.

## 2

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Hall theorem for soluble groups](../../../group.md#hall-conjugacy-and-embedding-in-finite-soluble-groups) says that for every prime set $\pi$, a finite [soluble group](../../../group-theory.md#solvable-group) has Hall $\pi$-subgroups; they are all conjugate, and every $\pi$-subgroup is contained in one. A Hall $\pi$-subgroup has only primes in $\pi$ in its order and no primes in $\pi$ in its index.

For a proof outline, induct on the [group](../../../group.md) order and choose a [minimal normal subgroup](../../../group-theory.md#minimal-normal-subgroup) $N$. In a finite [soluble group](../../../group-theory.md#solvable-group) this is elementary abelian of some characteristic $p$: its derived [subgroup](../../../group.md#subgroup) is characteristic and solvability forces it to be trivial; primary components and the [subgroup](../../../group.md#subgroup) of elements of order dividing $p$ are then characteristic, so minimality gives an [elementary abelian p-group](../../../group.md#elementary-abelian-group). Choose a Hall $\pi$-subgroup of $G/N$ and let $U$ be its preimage. If $p\in\pi$, $U$ is itself a Hall $\pi$-subgroup. If $p\notin\pi$, $U/N$ has order prime to $p$ and [coprime splitting over an elementary abelian normal subgroup](../../../group-theory.md#coprime-splitting-over-an-elementary-abelian-normal-subgroup) supplies a complement to $N$ in $U$, of the required Hall order.

Here the complement fact has a short averaging proof. Choose a section of $U/N=H$ and write its multiplication defect as $f(h,k)\in N$, in additive notation. Associativity gives

$$
f(h,k)+f(hk,t)=h f(k,t)+f(h,kt).
$$

Since $|H|$ is invertible on $N$, averaging over $t$ expresses the defect as $f(h,k)=b(h)+h b(k)-b(hk)$; adjusting the section by $-b$ gives a homomorphic section. Two such complements differ by $d(hk)=d(h)+h d(k)$. Averaging this identity gives $d(h)=b-hb$, so they are conjugate by $b\in N$. Inductive conjugacy in the quotient followed by this complement conjugacy proves Hall conjugacy. To embed an arbitrary $\pi$-subgroup $Q$, first put its quotient inside the chosen quotient [Hall subgroup](../../../group.md#hall-subgroup). In the coprime case $Q$ and the corresponding [subgroup](../../../group.md#subgroup) of a complement are both complements to $N$ inside $NQ$, hence are $N$-conjugate. In the other case $Q\le U$ directly. This proves [Hall conjugacy and embedding in finite soluble groups](../../../group.md#hall-conjugacy-and-embedding-in-finite-soluble-groups) as well as existence.

Now prove the assertion about [maximal subgroups](../../../group.md#maximal-subgroup) by induction on $|G|$. Suppose a nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) $K$ is contained in $A$. If $K\not\le B$, maximality gives $KB=G$, and since $K\le A$ this gives $AB=G$. If $K\le B$, both $A/K$ and $B/K$ are maximal in $G/K$; induction yields either their product equal to $G/K$ or their conjugacy, lifting respectively to $AB=G$ or to conjugacy of $A,B$. The same applies with their roles reversed.

It remains to suppose that no nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) of $G$ lies in either maximum. Let $K$ be minimal normal, an [elementary abelian p-group](../../../group.md#elementary-abelian-group). Since $K$ lies in neither maximum, $KA=KB=G$. The intersection $K\cap A$ is normalized by $A$ and by the [abelian group](../../../group.md#abelian-group) $K$, hence by $G$; it is therefore trivial. Likewise $K\cap B=1$. Thus both $A$ and $B$ complement $K$. Their action on $K$ is irreducible, since an [invariant subspace](../../../representation-theory.md#invariant-subspace) would be a proper nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) of $G$. It is also faithful: $C_A(K)$ is normalized by $A$ and centralized by $K$, so is a [normal subgroup](../../../group-theory.md#normal-subgroup) of $G$ contained in $A$ and must be trivial.

If $G/K=1$, these assumptions force $A=B=1$ and $G$ to have prime order. Otherwise choose $L>K$ normal in $G$ with $L/K$ minimal normal in $G/K$. It is an elementary abelian r-group. Under $A\cong G/K$, its copy $R=A\cap L$ is a nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) of $A$. The prime $r$ differs from $p$: a [p-group](../../../finite-group-theory.md#p-group) acting on the characteristic-p [vector space](../../../vector-space.md) $K$ has nonzero fixed points, by counting its orbits on $K$ modulo $p$. Its fixed subspace would be $A$-invariant, hence all of $K$ by irreducibility, contrary to faithfulness of $R$.

Therefore $A\cap L$ and $B\cap L$ are Sylow r-subgroups of $L=K(A\cap L)=K(B\cap L)$. They are conjugate in $L$. Conjugate $B$ so that these intersections coincide as $R$. Since $R\lhd A$, $N_G(R)\ge A$. It cannot equal $G$, since $R$ would then be a nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) contained in $A$. Maximality gives $N_G(R)=A$, and the same argument gives $N_G(R)=B$. The conjugated maxima are equal. Hence

$$
\boxed{G=AB\quad\text{or}\quad A\text{ and }B\text{ are conjugate in }G.}
$$

This is the factorization-or-conjugacy property of [maximal subgroups of a finite soluble group](../../../group.md#maximal-subgroups-of-a-finite-soluble-group).

## 3

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For $|G|=p^a m$ with $p\nmid m$, [Sylow theorems](../../../finite-group-theory.md#sylow-theorems) assert existence of a [subgroup](../../../group.md#subgroup) of order $p^a$, containment of every p-subgroup in one, conjugacy of all these [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup), and

$$
n_p\equiv1\pmod p,\qquad n_p\mid m,\qquad n_p=[G:N_G(P)].
$$

A [group](../../../group.md) of order $20$ has $n_5\mid4$ and $n_5\equiv1\pmod5$, so its Sylow 5-subgroup $P$ is unique. In $S_6$ it is generated by a five-cycle and has one fixed point. Its [normalizer](../../../group-theory.md#normalizer) preserves that point and, on the other five points identified with $\mathbb F_5$, is the affine [group](../../../group.md) $x\mapsto ax+b$. Every automorphism of the cyclic translation [group](../../../group.md) is realized by a multiplier. Thus $|N_{S_6}(P)|=5\cdot4=20$, forcing

$$
\boxed{N=N_{S_6}(P)\cong C_5\rtimes C_4,\qquad N\le H\cong S_5.}
$$

Inside $S_5$ there are $120/20=6$ Sylow 5-subgroups. [Conjugation](../../../group-theory.md#conjugation) gives a transitive action on them and a homomorphism into $S_6$. Its [group homomorphism kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) is a [normal subgroup](../../../group-theory.md#normal-subgroup) of $S_5$, whose only possibilities are $1,A_5,S_5$. The latter two would leave an image of order at most two, incompatible with transitivity on six points. Hence it is faithful. Denote the resulting transitive copy of $S_5$ by $J\le S_6$.

The action of $S_6$ on the six cosets of $J$ is also faithful: its [group homomorphism kernel](../../../group-theory.md#kernel-of-a-group-homomorphism) cannot contain the simple [subgroup](../../../group.md#subgroup) $A_6$, since an image of order at most two is not transitive of degree six, and a [normal subgroup](../../../group-theory.md#normal-subgroup) disjoint from $A_6$ centralizes $A_6$ and is trivial. It therefore gives an automorphism $\tau:S_6\to S_6$ carrying $J$ to a natural [point stabilizer](../../../group-theory.md#stabilizer-subgroup). This automorphism is outer, because [conjugation](../../../group-theory.md#conjugation) cannot carry a transitive [subgroup](../../../group.md#subgroup) to an intransitive one.

There are precisely two classes of copies of $S_5$ in $S_6$. A faithful intransitive copy must have an orbit of length five: all partitions of six into smaller orbits embed it in [groups](../../../group.md) of order below $120$. Thus it is a natural [point stabilizer](../../../group-theory.md#stabilizer-subgroup). A transitive copy is a degree-six coset action of an abstract $S_5$, with an order-$20$ stabilizer. Every order-$20$ [subgroup](../../../group.md#subgroup) of $S_5$ is a Sylow-five [normalizer](../../../group-theory.md#normalizer), so these stabilizers are conjugate and the degree-six actions are permutation-equivalent. Hence all transitive copies form one class. The [outer automorphism](../../../group-theory.md#outer-automorphism-of-a-group) constructed above swaps these two classes; it cannot preserve the point-stabilizer class, since any automorphism preserving that class induces a relabeling of its six members, and equivariance of their faithful [conjugation](../../../group-theory.md#conjugation) action then makes the automorphism inner.

Identify $S_6$ with its [inner automorphism](../../../group-theory.md#inner-automorphism) [group](../../../group.md) inside $\overline G$. Every Sylow 5-subgroup of $\overline G$ is contained in $S_6$, since that [normal subgroup](../../../group-theory.md#normal-subgroup) has index two. There are $720/20=36$ of them. Consequently

$$
\boxed{|\overline N|=1440/36=40,\qquad\overline N\cap S_6=N.}
$$

To prove maximality, first classify the proper overgroups of $N$ in $S_6$. The affine multiplier in $N$ of order four is a four-cycle and is odd. Within $H\cong S_5$, a proper overgroup larger than $N$ could only have order $60$, but the index-two [subgroup](../../../group.md#subgroup) is $A_5$ and cannot contain that odd element. Thus $N$ is maximal in $H$. A nontransitive overgroup of $N$ must fix its unique fixed point, so is $H$ if it is larger than $N$. A transitive overgroup $M$ has $M\cap H\ge N$; this [point stabilizer](../../../group-theory.md#stabilizer-subgroup) is either $N$ or $H$. In the latter case $M=S_6$, and in the former $|M|=6\cdot20=120$, making it a transitive copy of $S_5$.

There is exactly one such transitive copy containing $N$. There are six conjugates of $J$: applying the preceding overgroup argument to its own Sylow-five [normalizer](../../../group-theory.md#normalizer) shows that $J$ is maximal, and $J$ is not normal. Each contains six Sylow 5-subgroups. Counting pairs of a conjugate copy and a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) gives $6\cdot6=36$, with the same number through every one of the 36 [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) of $S_6$. Thus each [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup), and hence its [normalizer](../../../group-theory.md#normalizer) $N$, is contained in exactly one transitive copy. In particular the only proper strict overgroups of $N$ are its natural $H$ and this $J$.

The [subgroup](../../../group.md#subgroup) $\overline N$ has an outer element, because it has twice the order of $N$. Such an element normalizes $P$ and swaps the unique overgroups $H,J$. If $\overline N\le U\le\overline G$, then $U\cap S_6$ is normalized by $\overline N$, so it cannot be just $H$ or just $J$. It is therefore $N$ or $S_6$. In the latter case $U=\overline G$. In the former $U$ normalizes $N$ and hence its unique Sylow 5-subgroup $P$, giving $U\le\overline N$. Therefore

$$
\boxed{\overline N\text{ is a maximal subgroup of }\operatorname{Aut}(S_6).}
$$

## 4

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [special linear group over a finite field](../../../finite-group-theory.md#special-linear-group-over-a-finite-field) $SL_n(q)$ consists of the determinant-one invertible matrices over $\mathbb F_q$. Counting an ordered [basis](../../../vector-space.md#basis) gives

$$
|GL_n(q)|=\prod_{i=0}^{n-1}(q^n-q^i)
=q^{n(n-1)/2}\prod_{j=1}^n(q^j-1).
$$

The [determinant](../../../linear-algebra.md#determinant) map is onto $\mathbb F_q^*$, so

$$
\boxed{|SL_n(q)|=q^{n(n-1)/2}\prod_{j=2}^n(q^j-1).}
$$

A [transvection](../../../vector-space.md#transvection) has the form $I+vf$, where $v\ne0$, the [linear functional](../../../linear-algebra.md#linear-functional) $f$ is nonzero and $f(v)=0$. It has [determinant](../../../linear-algebra.md#determinant) one, fixes the [hyperplane](../../../vector-space.md#hyperplane) $\ker f$ pointwise, and its displacement has image the line $\langle v\rangle$. In particular $E_{ij}(t)=I+te_{ij}$ for $i\ne j$ is an elementary [transvection](../../../vector-space.md#transvection) when $t\ne0$.

Row addition is multiplication by such a [matrix](../../../vector-space.md#matrix). [Gaussian elimination](../../../numerical-analysis.md#gaussian-elimination) reduces a determinant-one [matrix](../../../vector-space.md#matrix) to diagonal form using row additions and determinant-one pivot exchanges. The latter, and all remaining diagonal factors, are themselves products of [transvections](../../../vector-space.md#transvection): within two coordinates,

$$
w(t)=E_{12}(t)E_{21}(-t^{-1})E_{12}(t)=\begin{pmatrix}0&t\\-t^{-1}&0\end{pmatrix},\qquad
w(t)w(-1)=\operatorname{diag}(t,t^{-1}).
$$

A diagonal [matrix](../../../vector-space.md#matrix) with product of entries one is a product of these two-coordinate diagonal matrices. Thus **[transvections](../../../vector-space.md#transvection) generate $SL_n(q)$**. This generation statement actually holds for every $n\ge2$ and every [finite field](../../../algebra.md#finite-field); the exclusions in the question are needed for the subsequent simplicity assertion.

Commuting with all elementary matrices forces the [group center](../../../group-theory.md#center-of-a-group) to consist of scalar matrices $\lambda I$ with $\lambda^n=1$, so its order is $d=\gcd(n,q-1)$. The projective quotient acts faithfully on the one-dimensional subspaces. Its action is two-transitive: send an ordered pair of independent representative vectors to any other pair and adjust the [determinant](../../../linear-algebra.md#determinant) by rescaling a representative without changing its line. Therefore it is primitive.

The [Iwasawa simplicity lemma](../../../finite-group-theory.md#iwasawa-simplicity-lemma) says that in a faithful primitive action, if a [point stabilizer](../../../group-theory.md#stabilizer-subgroup) has an abelian [normal subgroup](../../../group-theory.md#normal-subgroup) whose conjugates generate the [group](../../../group.md), every nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) contains the derived [subgroup](../../../group.md#subgroup). In particular a nontrivial [perfect group](../../../group-theory.md#perfect-group) satisfying these conditions is simple. No proof of the lemma is required here.

For the point $\ell=\langle v\rangle$, the [subgroup](../../../group.md#subgroup)

$$
U_\ell=\{I+vf:f(v)=0\}
$$

is abelian, is normal in the line stabilizer, and its conjugates contain all [transvections](../../../vector-space.md#transvection). Its image in the projective quotient has the same properties. Perfectness follows explicitly from elementary [commutators](../../../lie-algebra.md#commutator). If $n\ge3$, choose a third index $r$ to obtain

$$
[E_{ir}(a),E_{rj}(b)]=E_{ij}(ab).
$$

If $n=2,q>3$, choose $t$ with $t^2\ne1$ and set $h(t)=\operatorname{diag}(t,t^{-1})$. Then

$$
[h(t),E_{12}(c)]=E_{12}((t^2-1)c).
$$

Every upper [transvection](../../../vector-space.md#transvection) is a [commutator](../../../lie-algebra.md#commutator), and [conjugation](../../../group-theory.md#conjugation) gives the lower ones. The [group](../../../group.md) and its projective quotient are perfect. [Iwasawa's simplicity lemma](../../../finite-group-theory.md#iwasawa-simplicity-lemma) now proves

$$
\boxed{PSL_n(q)\text{ is simple for }n\ge3\text{ or }n=2,\ q>3.}
$$

The order of $PSL_2(4)$ is $4(4^2-1)=60$. Its faithful projective-line action has degree five, so its image is an index-two [subgroup](../../../group.md#subgroup) of $S_5$, necessarily $A_5$. Thus $PSL_2(4)\cong A_5$.

For $PSL_2(5)$ the order is $5(5^2-1)/2=60$. We construct a faithful degree-five action. In $SL_2(5)$ take

$$
i=\begin{pmatrix}2&0\\0&3\end{pmatrix},\qquad
j=\begin{pmatrix}0&1\\4&0\end{pmatrix}.
$$

They satisfy $i^2=j^2=-I$ and $ij=-ji$. Their quaternion [subgroup](../../../group.md#subgroup) projects to a Sylow 2-subgroup $V\cong C_2^2$. Its projective [centralizer](../../../group-theory.md#centralizer) is $V$: a lift of a centralizing element conjugates each of $i,j$ to itself or its negative. In the [matrix](../../../vector-space.md#matrix) [basis](../../../vector-space.md#basis) $I,i,j,ij$, those four sign choices each leave a one-dimensional space, and [determinant](../../../linear-algebra.md#determinant) one leaves just its two quaternion representatives. The [matrix](../../../vector-space.md#matrix)

$$
r=\frac{-I+i+j+ij}{2}=\begin{pmatrix}3&4\\3&1\end{pmatrix}
$$

has order three and cyclically permutes the three nonidentity elements of $V$. The [normalizer](../../../group-theory.md#normalizer) quotient embeds in $S_3$ and has order dividing both $6$ and $60/4=15$, so it has order exactly three. Hence $|N(V)|=12$ and there are five Sylow 2-subgroups. Their [conjugation](../../../group-theory.md#conjugation) action is nontrivial and transitive, and simplicity makes it faithful. Its image again has order $60$ in $S_5$, proving

$$
\boxed{PSL_2(4)\cong PSL_2(5)\cong A_5.}
$$

Finally,

$$
|PSL_3(4)|=\frac{4^3(4^2-1)(4^3-1)}3=20160,qquad
|PSL_4(2)|=2^6(2^2-1)(2^3-1)(2^4-1)=20160.
$$

In [characteristic two](../../../algebra.md#characteristic-two) an involutory [matrix](../../../vector-space.md#matrix) has form $I+N$ with $N^2=0$. Its Jordan blocks have size at most two. A projective [involution](../../../group-theory.md#involution) in $PSL_3(4)$ has a unique involutory lift to $SL_3(4)$: its square is central, and squaring is an automorphism of the scalar center of order three, allowing a unique scalar adjustment. The nonidentity Jordan form in [dimension](../../../vector-space.md#dimension-vector-space) three is only $(2,1)$. This GL-class remains a single SL-class, since the [centralizer](../../../group-theory.md#centralizer) contains $\operatorname{diag}(I_2,c)$ of every [determinant](../../../linear-algebra.md#determinant) $c\in\mathbb F_4^*$. Thus $PSL_3(4)$ has one [involution](../../../group-theory.md#involution) class.

In $PSL_4(2)=SL_4(2)=GL_4(2)$ there are two forms, $(2,1,1)$ and $(2,2)$, so there are two [involution](../../../group-theory.md#involution) classes. More concretely, the first [group](../../../group.md)'s single class has $21\cdot5\cdot3=315$ elements, counting image line, [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) plane through it and nonzero map between the quotient and image. The rank-one class in [dimension](../../../vector-space.md#dimension-vector-space) four over $\mathbb F_2$ has $15\cdot7=105$ elements; the rank-two class has $35\cdot|GL_2(2)|=210$. [Isomorphisms](../../../algebra.md#isomorphism) preserve conjugacy classes, so

$$
\boxed{PSL_3(4)\not\cong PSL_4(2),\quad\text{despite their common order }20160.}
$$

## 5

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Let $V$ have [dimension](../../../vector-space.md#dimension-vector-space) $2m$ over $\mathbb F_q$, with a nondegenerate [alternating bilinear form](../../../linear-algebra.md#alternating-bilinear-form) $B$. The symplectic [group](../../../group.md) is

$$
Sp_{2m}(q)=\{g\in GL(V):B(gv,gw)=B(v,w)\}.
$$

It acts freely and transitively on ordered symplectic bases. Choose the first vector $e_1\ne0$ in $q^{2m}-1$ ways, then choose $f_1$ with $B(e_1,f_1)=1$ in $q^{2m-1}$ ways. Their span is nondegenerate, so choose the remaining [symplectic basis](../../../linear-algebra.md#symplectic-basis) in its [orthogonal complement](../../../hilbert-space.md#orthogonal-complement). This gives the recurrence

$$
|Sp_{2m}(q)|=(q^{2m}-1)q^{2m-1}|Sp_{2m-2}(q)|,
$$

and therefore

$$
\boxed{|Sp_{2m}(q)|=q^{m^2}\prod_{j=1}^m(q^{2j}-1),\qquad |Sp_4(2)|=2^4(2^2-1)(2^4-1)=720.}
$$

For the [permutation](../../../combinatorics.md#permutation) module $\mathbb F_2^r$ with $r$ even, put $\mathbf t=(1,\ldots,1)$ and

$$
W=\left\{x:\sum_i x_i=0\right\}=\mathbf t^\perp.
$$

It is invariant under coordinate [permutations](../../../combinatorics.md#permutation) and has codimension one. The [dot product](../../../linear-algebra.md#dot-product) restricted to $W$ is alternating because $B(x,x)=\sum_i x_i^2=\sum_i x_i=0$. Since the ambient [dot product](../../../linear-algebra.md#dot-product) is nondegenerate, $W^\perp=\langle\mathbf t\rangle$. Evenness of $r$ ensures $\mathbf t\in W$, so

$$
\boxed{\operatorname{rad}(B|_W)=\langle\mathbf t\rangle.}
$$

Here the word symplectic must be understood as an alternating form before quotienting: a form with a nonzero radical is degenerate. The nondegenerate [symplectic form](../../../symplectic-geometry.md#symplectic-form) is induced on $\overline W=W/\langle\mathbf t\rangle$, of [dimension](../../../vector-space.md#dimension-vector-space) $r-2$.

Now put $r=2m+2$. Coordinate [permutations](../../../combinatorics.md#permutation) preserve the induced form and give a homomorphism $S_r\to Sp_{r-2}(2)$. To see it is faithful for $r\ge6$, suppose a [permutation](../../../combinatorics.md#permutation) $\sigma$ acts trivially on $\overline W$. For every pair of distinct indices,

$$
e_{\sigma(i)}+e_{\sigma(j)}\equiv e_i+e_j\pmod{\langle\mathbf t\rangle}.
$$

The two weight-two vectors could differ by $\mathbf t$ only if the complement of a two-element set also had size two. For $r\ge6$ that is impossible. Thus $\sigma$ preserves every two-element set, and hence fixes every index: intersect two such sets with one common element. Therefore

$$
\boxed{S_{2m+2}\hookrightarrow Sp_{2m}(2)\quad(m\ge2).}
$$

For $m=2$, both [groups](../../../group.md) have order $720$, and the injection is onto. This proves

$$
\boxed{S_6\cong Sp_4(2).}
$$

The lower bound matters: for $r=4$ the action on the quotient has the [Klein four-group](../../../finite-group-theory.md#klein-four-group) as [group homomorphism kernel](../../../group-theory.md#kernel-of-a-group-homomorphism). The construction is the [deleted permutation module in characteristic two](../../../representation-theory.md#deleted-permutation-module-in-characteristic-two).

## 6

↑ **Parent:** [Paper 2](paper-2.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A transitive [permutation](../../../combinatorics.md#permutation) [group](../../../group.md) is primitive when it preserves no nontrivial partition into blocks. A [point stabilizer](../../../group-theory.md#stabilizer-subgroup) is maximal precisely when the action is primitive. The orbits of any [normal subgroup](../../../group-theory.md#normal-subgroup) form a [block system](../../../group-theory.md#block-system), so every nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) of a faithful primitive [group](../../../group.md) is transitive. This turns the classification of primitive [groups](../../../group.md) into a study of their [minimal normal subgroups](../../../group-theory.md#minimal-normal-subgroup) and their [group socle](../../../group-theory.md#socle-of-a-finite-group).

The [socle of a finite group](../../../group-theory.md#socle-of-a-finite-group) is generated by its minimal nontrivial [normal subgroups](../../../group-theory.md#normal-subgroup). A [minimal normal subgroup](../../../group-theory.md#minimal-normal-subgroup) is characteristically simple, hence a direct power of a [simple group](../../../finite-group-theory.md#simple-group). Distinct [minimal normal subgroups](../../../group-theory.md#minimal-normal-subgroup) commute. If a transitive [normal subgroup](../../../group-theory.md#normal-subgroup) is abelian it is regular: its [point stabilizer](../../../group-theory.md#stabilizer-subgroup), being the same at all points, lies in the [group homomorphism kernel](../../../group-theory.md#kernel-of-a-group-homomorphism). In that case it is elementary abelian, and the ambient [group](../../../group.md) is affine. If two [minimal normal subgroups](../../../group-theory.md#minimal-normal-subgroup) occur, each centralizes the other; the [centralizer](../../../group-theory.md#centralizer) of a transitive [permutation](../../../combinatorics.md#permutation) [group](../../../group.md) is semiregular, so both are regular and the two regular [groups](../../../group.md) are mutual left/right partners. These observations are central to the [O'Nan–Scott theorem](../../../group-theory.md#o-nan-scott-theorem).

The theorem organizes finite primitive [groups](../../../group.md) into the following socle/action types. In the affine type HA, the [group socle](../../../group-theory.md#socle-of-a-finite-group) is $C_p^d$, degree $p^d$, and $G=C_p^d\rtimes H$ with $H\le GL_d(p)$ irreducible. In almost-simple type AS the [group socle](../../../group-theory.md#socle-of-a-finite-group) is one nonabelian [simple group](../../../finite-group-theory.md#simple-group) $T$ and $T\le G\le\operatorname{Aut}(T)$; a [maximal subgroup](../../../group.md#maximal-subgroup) not containing $T$ specifies the primitive coset action.

In simple-diagonal type SD the [group socle](../../../group-theory.md#socle-of-a-finite-group) is $T^r$, $r\ge2$, and its intersection with a [point stabilizer](../../../group-theory.md#stabilizer-subgroup) is a full diagonal copy of $T$. The degree is $|T|^{r-1}$, and the action includes the appropriate [permutation](../../../combinatorics.md#permutation) of the simple factors. Compound-diagonal type CD replaces this one diagonal by a product of diagonals in disjoint collections of factors; it is a product version of diagonal type. In product-action type PA one embeds in a [wreath product](../../../group-theory.md#wreath-product) with a primitive nonregular almost-simple base, acting on a Cartesian power $\Delta^r$, so the degree is $|\Delta|^r$ and the [group socle](../../../group-theory.md#socle-of-a-finite-group) is a corresponding power of $T$.

Types HS and HC have two regular [minimal normal subgroups](../../../group-theory.md#minimal-normal-subgroup), each isomorphic respectively to $T$ or to $T^r$ with $r>1$. Their socle consists of the left and right regular [groups](../../../group.md); the degrees are $|T|$ and $|T|^r$. Finally TW, twisted-wreath type, has a unique regular nonabelian [minimal normal subgroup](../../../group-theory.md#minimal-normal-subgroup) $T^r$ and a [point stabilizer](../../../group-theory.md#stabilizer-subgroup) acting through a twisted [permutation](../../../combinatorics.md#permutation) of its factors. This has degree $|T|^r$; primitivity imposes restrictive conditions, in particular $r\ge6$. These eight modern labels refine the older affine/almost-simple/diagonal/product description. The theorem reduces the problem to [simple groups](../../../finite-group-theory.md#simple-group), their [maximal subgroups](../../../group.md#maximal-subgroup), irreducible linear actions and the specified product constructions; it does not make every primitive [group](../../../group.md) maximal in a [symmetric group](../../../finite-group-theory.md#symmetric-group).

For [maximal subgroups](../../../group.md#maximal-subgroup) of $S_n$ there are first two elementary families. An intransitive [maximal subgroup](../../../group.md#maximal-subgroup) is the stabilizer $S_a\times S_{n-a}$ of an unordered distinguished subset, with $1\le a<n/2$; replacing the subset by its complement gives the same class. When $a=n/2$, this [subgroup](../../../group.md#subgroup) sits properly inside the stabilizer of the two equal blocks. A transitive imprimitive [maximal subgroup](../../../group.md#maximal-subgroup) is a full block-system stabilizer $S_a\wr S_b$, with $ab=n$, $a,b>1$, in its imprimitive action.

The [alternating group](../../../finite-group-theory.md#alternating-group) $A_n$ is itself maximal. A remaining primitive maximum must contain odd [permutations](../../../combinatorics.md#permutation). The primitive part of O'Nan–Scott places it among full affine, diagonal, product-action, or almost-simple overgroups. Full affine [groups](../../../group.md) have degree $p^d$; full diagonal [groups](../../../group.md) have degree $|T|^{r-1}$ and socle $T^r$; full product-action wreath [groups](../../../group.md) have degree $d^r$. Almost-simple cases require the actual simple-group [permutation](../../../combinatorics.md#permutation) degree and its full [permutation](../../../combinatorics.md#permutation) [normalizer](../../../group-theory.md#normalizer). Regular nonabelian types are contained in the corresponding holomorph/diagonal or product overgroups, so do not supply extra maximal families. Parity and exceptional containments must be checked before calling any of these candidates maximal.

In degree sixteen the complete list, up to $S_{16}$-conjugacy, is

$$
\boxed{A_{16};\quad S_a\times S_{16-a}\ (1\le a\le7);\quad S_2\wr S_8,\ S_4\wr S_4,\ S_8\wr S_2.}
$$

The three [wreath products](../../../group-theory.md#wreath-product) here act on blocks, not Cartesian coordinates. The other proper primitive [groups](../../../group.md) of this degree are affine and lie in $AGL_4(2)$. A nonzero translation of its sixteen points is eight [transpositions](../../../combinatorics.md#transposition-permutation), and a generating linear [transvection](../../../vector-space.md#transvection) is four [transpositions](../../../combinatorics.md#transposition-permutation), so the full affine [group](../../../group.md) lies in $A_{16}$. Even the tempting product-action $S_4\wr S_2$ on $4^2$ points is contained in this affine [group](../../../group.md): identify each four-point coordinate with $\mathbb F_2^2$. Alternatively, each base [transposition](../../../combinatorics.md#transposition-permutation) repeats four times and coordinate exchange makes six [transpositions](../../../combinatorics.md#transposition-permutation), both even. Thus none is an additional maximum of $S_{16}$. There are **eleven conjugacy classes** in the displayed list.

In degree sixty the complete list is

$$
\boxed{\begin{gathered}
A_{60};\qquad S_a\times S_{60-a}\quad(1\le a\le29);\\
S_a\wr S_{60/a}\quad(a=2,3,4,5,6,10,12,15,20,30);\\
PGL_2(59)\text{ on }\mathbb P^1(\mathbb F_{59});\qquad D(A_5,2)\text{ on }A_5.
\end{gathered}}
$$

The notation $D(A_5,2)$ denotes the full diagonal [normalizer](../../../group-theory.md#normalizer), not just $A_5\times A_5$. It is generated on the set $A_5$ by $x\mapsto axb^{-1}$, an [outer automorphism](../../../group-theory.md#outer-automorphism-of-a-group) induced by odd [conjugation](../../../group-theory.md#conjugation) in $S_5$, and $x\mapsto x^{-1}$. Its order is

$$
|D(A_5,2)|=60^2\cdot2\cdot2=14400.
$$

Its two alternating factors form the [group socle](../../../group-theory.md#socle-of-a-finite-group). The [point stabilizer](../../../group-theory.md#stabilizer-subgroup) intersects them in the diagonal $A_5$, of index sixty. Odd [conjugation](../../../group-theory.md#conjugation) by a [transposition](../../../combinatorics.md#transposition-permutation) of $S_5$ fixes its six commuting elements in $A_5$, hence makes $(60-6)/2=27$ [transpositions](../../../combinatorics.md#transposition-permutation) and is odd. Inversion fixes the identity and the fifteen [involutions](../../../group-theory.md#involution), so makes twenty-two [transpositions](../../../combinatorics.md#transposition-permutation) and is even. This verifies that the full diagonal [group](../../../group.md) is not lost inside $A_{60}$.

The almost-simple maximum $PGL_2(59)$ has order $59(59^2-1)=205320$ and its usual two-transitive projective-line action. Multiplication by a primitive element of $\mathbb F_{59}^*$ makes one 58-cycle and fixes zero and infinity, so it too contains odd [permutations](../../../combinatorics.md#permutation). The simple [subgroup](../../../group.md#subgroup) $PSL_2(59)$ alone is not maximal. Degree sixty is neither a prime power nor a proper power, excluding affine and product/compound types; its diagonal possibility is $T=A_5,r=2$. The almost-simple primitive possibilities, besides the natural alternating/[symmetric groups](../../../finite-group-theory.md#symmetric-group), have socle $PSL_2(59)$. Their full [normalizer](../../../group-theory.md#normalizer) is the displayed $PGL_2(59)$. These degree-specific classification facts supply the exhaustive primitive part of the list. Altogether there are **forty-two conjugacy classes of [maximal subgroups](../../../group.md#maximal-subgroup) of $S_{60}$**: twenty-nine intransitive, ten imprimitive, the [alternating group](../../../finite-group-theory.md#alternating-group), and two further primitive classes.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
