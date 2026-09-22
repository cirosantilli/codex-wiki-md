# Paper 1

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper1.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper1.pdf)

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

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Work with finite [groups](../../../group.md), as required for these [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) counts. Let $P$ act by [conjugation](../../../group-theory.md#conjugation) on the set of Sylow $p$-subgroups. The [stabilizer](../../../group-theory.md#stabilizer-subgroup) of $Q$ is $P\cap N_G(Q)$. Since $Q$ is the normal [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) of its own [normalizer](../../../group-theory.md#normalizer), every $p$-subgroup of that [normalizer](../../../group-theory.md#normalizer) lies in $Q$. Consequently the [stabilizer](../../../group-theory.md#stabilizer-subgroup) is exactly $P\cap Q$, and the [orbit-stabilizer theorem](../../../group-theory.md#orbit-stabilizer-theorem) gives orbit size $[P:P\cap Q]$. The orbit of $P$ has size one. Every other orbit size is a power of $p$ at least $p^a$, hence is divisible by $p^a$. Adding orbit sizes proves the [strengthened Sylow congruence from intersections](../../../finite-group-theory.md#strengthened-sylow-congruence-from-intersections):

$$
\boxed{n_p\equiv1\pmod{p^a}.}
$$

Now suppose $G$ is simple of order $2^e\cdot15$. If $e=0$, its Sylow $5$-subgroup is normal because its number divides three and is one modulo five. If $e=1$, an involution in the regular [permutation action](../../../group-theory.md#group-action) of $G$ swaps fifteen pairs, so its sign is negative. The [sign of a permutation](../../../finite-group-theory.md#sign-of-a-permutation) would give a nontrivial [group homomorphism](../../../group-theory.md#group-homomorphism) $G\to C_2$ with a proper nontrivial normal kernel. Both cases contradict simplicity. Thus $e\ge2$.

The [Sylow theorems](../../../finite-group-theory.md#sylow-theorems) make $n_2$ a divisor of fifteen. It is not one, since a nontrivial [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) would then be normal. It is not three, since the [conjugation action](../../../group-theory.md#conjugation-action) on three [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) would give a faithful [group homomorphism](../../../group-theory.md#group-homomorphism) $G\hookrightarrow S_3$, impossible by order. If $n_2=5$, take a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) $P$ itself: its [normalizer](../../../group-theory.md#normalizer) has [subgroup index](../../../group.md#index-of-a-subgroup) five. If $n_2=15$, not all distinct [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) can intersect $P$ in [subgroup index](../../../group.md#index-of-a-subgroup) at least four, since that would give $15\equiv1\pmod4$. Choose $Q\ne P$ with $[P:P\cap Q]=2$. Put $R=P\cap Q$, of order $2^{e-1}$. It has [subgroup index](../../../group.md#index-of-a-subgroup) two in both $P,Q$, so is normal in each. Hence $N_G(R)$ contains both distinct [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) and has order greater than $2^e$. It is proper: otherwise $R$ would be a nontrivial proper [normal subgroup](../../../group-theory.md#normal-subgroup) of $G$. Its order is therefore $2^e\cdot3$ or $2^e\cdot5$. The latter would give an index-three subgroup and again an impossible faithful action on three [cosets](../../../group-theory.md#coset). Thus $[G:N_G(R)]=5$.

In either case we have the requested subgroup of order $2^e$ or $2^{e-1}$ with index-five [normalizer](../../../group-theory.md#normalizer). The action on the five [cosets](../../../group-theory.md#coset) of that [normalizer](../../../group-theory.md#normalizer) is nontrivial and faithful by simplicity. Its image lies in $A_5$, since composing with sign cannot give a nontrivial map from this [simple group](../../../finite-group-theory.md#simple-group) of order greater than two to $C_2$. Thus $2^e\cdot15$ divides $60$, forcing $e=2$ and equality of orders. This proves the [simple groups with order a power of two times fifteen](../../../finite-group-theory.md#simple-groups-with-order-a-power-of-two-times-fifteen) conclusion:

$$
\boxed{G\cong A_5.}
$$

For $SL_2(5)$, choose the first column: there are $5^2-1=24$ nonzero choices. For each, determinant one is a nonzero linear equation in the second column and has five solutions. Therefore $|SL_2(5)|=120$. A central [matrix](../../../vector-space.md#matrix) commuting with $\left(\begin{smallmatrix}1&1\\0&1\end{smallmatrix}\right)$ has zero lower-left entry and equal diagonal entries; commuting also with $\left(\begin{smallmatrix}1&0\\1&1\end{smallmatrix}\right)$ makes the upper-right entry zero. It is scalar. Determinant one then gives

$$
\boxed{|SL_2(5)|=120,\qquad Z=\{I,-I\},\quad |Z|=2.}
$$

To establish the [projective special linear group over the field with five elements](../../../finite-group-theory.md#projective-special-linear-group-over-the-field-with-five-elements) isomorphism without assuming its simplicity, compute its classes. For determinant-one matrices, the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) is $X^2-tX+1$ with trace $t$. The possibilities over $\mathbb F_5$ exhaust the group:

$$
\begin{array}{c|c|c}
\text{type in }SL_2(5)&\text{centralizer order}&\text{class sizes in }SL_2(5)\\\hline
\pm I&120&1,1\\
t=0&4&30\\
t=1,-1&6&20,20\\
t=2,-2,\ \text{noncentral}&10&12,12,12,12
\end{array}
$$

For trace zero the [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $2,3$, so the determinant-one [centralizer](../../../group-theory.md#centralizer) is the split diagonal torus of order four. For traces $\pm1$, the discriminant is the nonsquare $2$: the [centralizer](../../../group-theory.md#centralizer) is the norm-one subgroup of $\mathbb F_{25}^{\times}$, of order six. In both semisimple cases the determinant map on the full linear [centralizer](../../../group-theory.md#centralizer) is surjective onto $\mathbb F_5^{\times}$; consequently each trace type is a single special-linear class. For the noncentral traces $\pm2$, a [Jordan block](../../../linear-operator-theory.md#jordan-block) has full linear [centralizer](../../../group-theory.md#centralizer) $\left\{\left(\begin{smallmatrix}a&b\\0&a\end{smallmatrix}\right):a\ne0\right\}$ with determinant $a^2$. The [determinant](../../../linear-algebra.md#determinant) image consists of the two squares, so each general-linear class splits into two special-linear classes; the determinant-one [centralizer](../../../group-theory.md#centralizer) has order $2\cdot5=10$. These sizes sum to $120$.

Quotienting by $Z$ identifies a matrix with its negative. The trace-zero class gives one projective class of size fifteen; the two traces $\pm1$ give one class of size twenty; the four noncentral unipotent classes give two classes of size twelve. Their respective projective orders are $2,3,5,5$, by the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial)s. A [normal subgroup](../../../group-theory.md#normal-subgroup) is a union of classes containing the identity. The nontrivial proper possible union sizes are $13,16,21,25,28,33,36,40,45,48$, none of which divides $60$. Thus the quotient is simple. Applying the order-$60$ result above gives

$$
\boxed{PSL_2(5)\cong A_5.}
$$

Finally, if $A^2=I$ over an odd-characteristic field, its [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) divides the square-free polynomial $(X-1)(X+1)$, so it is diagonalizable with [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\pm1$. In dimension two, determinant one requires both eigenvalues equal. Hence $A=I$ or $A=-I$. This proves the [unique involution in SL2 over an odd field](../../../finite-group-theory.md#unique-involution-in-sl2-over-an-odd-field) assertion: **the only element of order two in $SL_2(5)$ is $-I$**. If an index-two subgroup $H$ existed, it would be normal and have order sixty. By [Cauchy theorem](../../../complex-analysis.md#cauchy-s-integral-theorem) it would contain an involution, hence contain $Z$. Then $H/Z$ would be a [normal subgroup](../../../group-theory.md#normal-subgroup) of order thirty in the simple quotient $PSL_2(5)$, a contradiction. Thus **$SL_2(5)$ has no index-two subgroup**.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

First prove [Simplicity of alternating groups](../../../finite-group-theory.md#simplicity-of-alternating-groups). The $3$-cycles generate $A_n$: express an even permutation as an even number of [transpositions](../../../combinatorics.md#transposition-permutation) and pair them. A pair sharing a point is a $3$-cycle, an identical pair cancels, and a disjoint pair can be written $(ab)(cd)=(acb)(acd)$. All $3$-cycles are conjugate in $A_n$ when $n\ge5$: a conjugator in $S_n$ can have its parity corrected by a [transposition](../../../combinatorics.md#transposition-permutation) on two points outside the target triple, without changing its effect on that triple.

Let $1\ne N\triangleleft A_n$ and choose $1\ne\sigma\in N$. Some $3$-cycle $\tau$ does not commute with $\sigma$. Indeed, commuting with every $3$-cycle would preserve every triple setwise; intersecting all triples containing a given point forces that point to be fixed, so would make $\sigma=1$. The nonidentity [group commutator](../../../group.md#group-commutator) $\sigma\tau\sigma^{-1}\tau^{-1}\in N$ is supported on at most six points. Its possible nontrivial even cycle types are a $3$-cycle, a double [transposition](../../../combinatorics.md#transposition-permutation), a $5$-cycle, two disjoint $3$-cycles, or a $4$-cycle times a [transposition](../../../combinatorics.md#transposition-permutation). Each yields a $3$-cycle in $N$ by explicit [group commutators](../../../group.md#group-commutator):

For $(ab)(cd)$, use $\tau=(cde)$ with a fifth point $e$; [conjugation](../../../group-theory.md#conjugation) reverses $\tau$, so the [group commutator](../../../group.md#group-commutator) is $\tau^{-2}=\tau$. For $(abcde)$, use $(abc)$: the [group commutator](../../../group.md#group-commutator) is $(bcd)(abc)^{-1}=(adb)$. The same calculation works for $(abcd)(ef)$. For $(abc)(def)$, use $(abd)$; its conjugate is $(bce)$, and the product $(bce)(abd)^{-1}$ is a $5$-cycle, reducing to the preceding case. Thus $N$ contains a $3$-cycle, hence the whole [conjugacy class](../../../group-theory.md#conjugacy-class) of $3$-cycles, and hence all of $A_n$. Therefore

$$
\boxed{A_n\text{ is simple for }n\ge5.}
$$

For the exceptional [automorphism](../../../algebra.md#automorphism), a [duad](../../../combinatorics.md#duad) is an unordered pair of six points, a [syntheme](../../../combinatorics.md#syntheme) is a partition into three duads, and a [pentad](../../../combinatorics.md#total-of-synthemes) is a set of five synthemes covering every duad once. There are fifteen synthemes. To count pentads, fix $12|34|56$, where bars separate duads. A syntheme disjoint from it in duads is one of eight; the union of the two matchings is a six-cycle, so the [stabilizer](../../../group-theory.md#stabilizer-subgroup) of the fixed syntheme is transitive on these eight choices. For the choice $13|25|46$, the remaining compatible synthemes are $14|26|35$, $15|24|36$, $16|23|45$ and $16|24|35$. The last shares a duad with each of the first three and cannot belong to a completion; the first three form the unique completion. Thus each of the eight choices has a unique completion through the fixed syntheme. Each completion contains four of them, so exactly two pentads contain a fixed syntheme, and there are $15\cdot2/5=6$ pentads in total.

Here is the complete list, which also defines concrete labels for the induced action:

$$
\begin{array}{c|l}
1&12|34|56,\ 13|25|46,\ 14|26|35,\ 15|24|36,\ 16|23|45\\
2&12|34|56,\ 13|26|45,\ 14|25|36,\ 15|23|46,\ 16|24|35\\
3&12|35|46,\ 13|24|56,\ 14|25|36,\ 15|26|34,\ 16|23|45\\
4&12|35|46,\ 13|26|45,\ 14|23|56,\ 15|24|36,\ 16|25|34\\
5&12|36|45,\ 13|24|56,\ 14|26|35,\ 15|23|46,\ 16|25|34\\
6&12|36|45,\ 13|25|46,\ 14|23|56,\ 15|26|34,\ 16|24|35
\end{array}
$$

Relabelling points gives a [group homomorphism](../../../group-theory.md#group-homomorphism) $\Phi:S_6\to S_6$ on these pentads. Direct substitution in the table gives

$$
\Phi((12))=(12)(34)(56),\qquad
\Phi((123))=(145)(263).
$$

The restriction to $A_6$ is nontrivial, hence faithful by the simplicity just proved. Therefore the full kernel has order at most two. An order-two [normal subgroup](../../../group-theory.md#normal-subgroup) would be central, whereas $S_6$ has trivial centre: an element centralizing every [transposition](../../../combinatorics.md#transposition-permutation) fixes every unordered pair and consequently every point. The kernel is trivial, and equal orders make $\Phi$ an [automorphism](../../../algebra.md#automorphism). It preserves $A_6$, because that is the unique index-two subgroup of $S_6$: any nontrivial [group homomorphism](../../../group-theory.md#group-homomorphism) to $C_2$ sends every conjugate [transposition](../../../combinatorics.md#transposition-permutation) to the nonidentity element, and is therefore the sign map. Its restriction is the [pentad construction of the exceptional alternating-group automorphism](../../../combinatorics.md#pentad-construction-of-the-exceptional-alternating-group-automorphism). It maps a $3$-cycle to two disjoint $3$-cycles, while [conjugation](../../../group-theory.md#conjugation) in $S_6$ preserves [cycle type](../../../finite-group-theory.md#cycle-type). Hence **this [automorphism](../../../algebra.md#automorphism) of $A_6$ is not induced by any element of $S_6$**.

For the other degrees, recover the points from $3$-cycles. An element of order three has type $3^k1^{n-3k}$. Its [centralizer](../../../group-theory.md#centralizer) in $S_n$ has order $3^k k!(n-3k)!$. That [centralizer](../../../group-theory.md#centralizer) contains an odd permutation: either swap two fixed points, or, when $k\ge2$, swap two three-cycles by three [transpositions](../../../combinatorics.md#transposition-permutation). Thus

$$
|C_{A_n}(x)|=\frac{3^k k!(n-3k)!}{2}.
$$

For $n=5$, only $k=1$ is possible. For $n\ge7$, the $k=1$ value is strictly largest. For $k=2$ equality first occurs at $n=6$, and the ratio increases strictly with $n$. For $k\ge3$, already at $n=3k$ one has $(3k-3)!>3^{k-1}k!$: it holds at $k=3$, and the inductive ratio is $(3k)(3k-1)(3k-2)>3(k+1)$. Increasing $n$ again increases the ratio. Consequently every [automorphism](../../../algebra.md#automorphism) preserves the set of $3$-cycles when $n\ne6$.

Each [cyclic subgroup](../../../group.md#cyclic-subgroup) generated by a $3$-cycle corresponds to its three-point support. Two distinct such subgroups commute exactly when the supports are disjoint. If they meet in one point, products of their nonidentity generators have order five. If they meet in two points, those products have order two or three. These intrinsic tests recover adjacency in the [Johnson graph](../../../graph-theory.md#johnson-graph) $J(n,3)$, so the [automorphism](../../../algebra.md#automorphism) acts on its vertices.

We can reconstruct the underlying points without an additional group-theoretic bound. The [maximal cliques of a Johnson graph](../../../graph-theory.md#maximal-cliques-of-a-johnson-graph) in $J(n,3)$ are the $n-2$ triples containing a fixed pair, and the four triples contained in a fixed four-set. To verify the classification, take adjacent triples $D\cup\{a\}$ and $D\cup\{b\}$ with $|D|=2$. Any common adjacent triple either contains $D$ or lies in $D\cup\{a,b\}$. A triple of the first kind outside that four-set is not adjacent to a triple of the second kind omitting a point of $D$, so a clique cannot mix the two alternatives. Extending a clique therefore gives exactly one of the two listed families.

For $n\ge5$, $n\ne6$, their sizes distinguish the pair-containing cliques. Their intersections reconstruct the pair graph $J(n,2)$: two such cliques intersect precisely when their defining pairs meet in one point. In this graph the maximal cliques are stars of $n-1$ pairs through a point and triangles of three pairs within a triple. These sizes are different for $n\ge5$, so its [automorphisms](../../../algebra.md#automorphism) permute the stars and hence the points. Every pair is the intersection of its two point stars, and every triple is determined by its three pairs. Thus the original graph action comes from some $\pi\in S_n$.

Undo [conjugation](../../../group-theory.md#conjugation) by $\pi$. The remaining [group automorphism](../../../algebra.md#group-automorphism) $\beta$ fixes each cyclic $3$-subgroup, so it fixes or inverts each generator. For adjacent supports, inverting exactly one generator changes the order of their product between two and three; inverting both preserves that order. Hence the two inversion choices must agree. The triple-support graph is connected, since one can replace differing points one at a time, so the choice is uniform. Inverting every $3$-cycle is impossible: take $c=(123)$, $d=(142)$, whose product is the $3$-cycle $(143)$. Then $\beta(cd)=(cd)^{-1}=d^{-1}c^{-1}$, whereas the [group homomorphism](../../../group-theory.md#group-homomorphism) property would give $c^{-1}d^{-1}$; these are unequal because $c,d$ do not commute. Therefore $\beta$ fixes every $3$-cycle and is the identity. Conversely, [conjugation](../../../group-theory.md#conjugation) by $S_n$ acts faithfully on $A_n$, since centralizing all $3$-cycles fixes every triple and every point. The [automorphisms of alternating groups from triple supports](../../../finite-group-theory.md#automorphisms-of-alternating-groups-from-triple-supports) are exactly

$$
\boxed{\operatorname{Aut}(A_n)\cong S_n\qquad(n\ge5,\ n\ne6).}
$$

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Choose a minimal nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) $L$ of $K$ itself. Every conjugate $L^g$ for $g\in G$ is also a [minimal normal subgroup](../../../group-theory.md#minimal-normal-subgroup) of $K$, since $K$ is normal in $G$. Distinct such subgroups intersect trivially: their intersection is normal in $K$ and minimality forces either equality or trivial intersection. Moreover $[L_i,L_j]\subseteq L_i\cap L_j=1$, so distinct ones commute.

Choose a maximal family of these conjugates whose product $M=L_1\times\cdots\times L_r$ is direct. For any further conjugate $L^g$, its intersection with $M$ is normal in $K$ and is either all of $L^g$ or trivial. In the latter case it commutes with all the existing factors and could be adjoined to the [direct product of groups](../../../group-theory.md#direct-product-of-groups), contrary to maximality. Thus every conjugate is contained in $M$. The product of all conjugates is consequently $M$, which is nontrivial and normal in $G$. Minimality of $K$ as a $G$-normal subgroup gives $M=K$.

Any [normal subgroup](../../../group-theory.md#normal-subgroup) of a factor $L_i$ is normal in $K$: the other direct factors commute with it, and $L_i$ normalizes it. Minimality of $L_i$ as a $K$-normal subgroup makes it simple. All factors are isomorphic because they are conjugate to $L$. This proves the [direct-product structure of a finite minimal normal subgroup](../../../group-theory.md#direct-product-structure-of-a-finite-minimal-normal-subgroup):

$$
\boxed{K\cong S^r\quad\text{for a finite simple group }S.}
$$

An abelian [simple group](../../../finite-group-theory.md#simple-group) is cyclic of prime order, so the abelian case is elementary abelian. Now let $H$ be a maximal proper subgroup of a nonabelian [simple group](../../../finite-group-theory.md#simple-group) $X$. It is nontrivial, since $X$ has nontrivial proper [cyclic subgroups](../../../group.md#cyclic-subgroup). Choose a [minimal normal subgroup](../../../group-theory.md#minimal-normal-subgroup) $K$ of $H$. Then $H\le N_X(K)$. This [normalizer](../../../group-theory.md#normalizer) cannot be $X$, since that would make $1<K\le H<X$ normal in $X$. Maximality gives

$$
\boxed{H=N_X(K),\qquad K\cong S^r.}
$$

For each of the two groups in this question, the allowed absence of proper nonabelian simple subgroups makes the factors of such a $K$ cyclic of prime order. Hence it suffices to examine [normalizers](../../../group-theory.md#normalizer) of nontrivial elementary abelian subgroups.

In $A_5$, the possible primes are two, three and five. The [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) for the last two primes are cyclic of orders three and five. Every involution is a double [transposition](../../../combinatorics.md#transposition-permutation); for $(12)(34)$ the [centralizer](../../../group-theory.md#centralizer) in $A_5$ is

$$
\{1,(12)(34),(13)(24),(14)(23)\},
$$

the [Klein four-group](../../../finite-group-theory.md#klein-four-group) fixing point five. Thus an elementary abelian $2$-subgroup is cyclic of order two or a [Klein four-group](../../../finite-group-theory.md#klein-four-group). The [normalizer](../../../group-theory.md#normalizer) of a cyclic order-two subgroup equals its [centralizer](../../../group-theory.md#centralizer) and has order four, so is contained in a point [stabilizer](../../../group-theory.md#stabilizer-subgroup) of order twelve. A [Klein four-group](../../../finite-group-theory.md#klein-four-group)'s common fixed point is intrinsic, and the full point [stabilizer](../../../group-theory.md#stabilizer-subgroup) $A_4$ normalizes it; its [normalizer](../../../group-theory.md#normalizer) is therefore exactly that [stabilizer](../../../group-theory.md#stabilizer-subgroup).

An order-three subgroup has support a triple. Its [normalizer](../../../group-theory.md#normalizer) preserves the triple and the remaining pair, and is $(S_3\times S_2)\cap A_5$, of order six. An order-five subgroup acts regularly on all five points. Label the points by $\mathbb F_5$, with the subgroup acting by translations. Its [normalizer](../../../group-theory.md#normalizer) in $S_5$ is the twenty affine maps $x\mapsto ax+b$. The translations are even, whereas multiplication by a generator of $\mathbb F_5^{\times}$ is a four-cycle and is odd. Exactly half these maps are even, so the [normalizer](../../../group-theory.md#normalizer) in $A_5$ has order ten.

The only candidates for [maximal subgroups](../../../group.md#maximal-subgroup) are thus the [normalizers](../../../group-theory.md#normalizer) of orders twelve, ten and six. They are all maximal: none can lie in a larger candidate, except potentially an order-six subgroup in an order-twelve $A_4$. But an index-two subgroup of $A_4$ would contain every order-three element; there are eight such elements, plus the identity, already more than six. Hence that containment is impossible. Point [stabilizers](../../../group-theory.md#stabilizer-subgroup) are conjugate; order-three and order-five subgroup [normalizers](../../../group-theory.md#normalizer) each form one class by the [Sylow theorems](../../../finite-group-theory.md#sylow-theorems). Therefore the [maximal subgroups of A5](../../../finite-group-theory.md#maximal-subgroups-of-a5) form precisely

$$
\boxed{\text{three conjugacy classes, of orders }12,10,6.}
$$

Their numbers are five, six and ten respectively, since these proper [maximal subgroups](../../../group.md#maximal-subgroup) are self-normalizing in the [simple group](../../../finite-group-theory.md#simple-group).

For $X=GL_3(2)$, choosing independent columns gives $|X|=(8-1)(8-2)(8-4)=168$. If $t$ is an involution, write $t=I+N$. [Field characteristic](../../../algebra.md#characteristic-of-a-field) two gives $N^2=0$, and $\operatorname{im}N\subseteq\ker N$ in dimension three forces its nonzero rank to be one. Thus $t=I+vf$, with nonzero vector $v$, nonzero [linear functional](../../../linear-algebra.md#linear-functional) $f$ and $f(v)=0$. This [transvection](../../../vector-space.md#transvection) fixes the plane $\ker f$ and has image line $\langle v\rangle$. Every flag consisting of an incident line and plane occurs, giving $7\cdot3=21$ involutions, all conjugate. Its [centralizer](../../../group-theory.md#centralizer), and hence the [normalizer](../../../group-theory.md#normalizer) of its [cyclic subgroup](../../../group.md#cyclic-subgroup), is the flag [stabilizer](../../../group-theory.md#stabilizer-subgroup) of order $168/21=8$. It lies in both the line and plane [stabilizers](../../../group-theory.md#stabilizer-subgroup) of order $24$, so cannot be maximal.

For the [elementary abelian subgroups in GL3 over F2](../../../finite-group-theory.md#elementary-abelian-subgroups-in-gl3-over-f2), consider commuting [transvections](../../../vector-space.md#transvection) $I+vf$, $I+wh$. Their rank-one parts satisfy

$$
v f(w)h=w h(v)f.
$$

If $v,w$ are independent, equality forces both sides zero; thus $f,h$ vanish on $\langle v,w\rangle$ and are the same nonzero functional. If $v=w$, they have a common image line. Consequently the two types of order-four elementary abelian subgroup are

$$
K_L=\{I+vf:f(v)=0\},\qquad
K_W=\{I+wf:w\in W=\ker f\}.
$$

No extra [transvection](../../../vector-space.md#transvection) can commute with all elements of $K_L$: if its image were different, its functional would have to equal each of the two independent functionals occurring in $K_L$. Dually, the same holds for $K_W$. Thus these exhaust the elementary abelian $2$-subgroups of rank at least two. The [normalizer](../../../group-theory.md#normalizer) of $K_L$ is the line [stabilizer](../../../group-theory.md#stabilizer-subgroup) and the [normalizer](../../../group-theory.md#normalizer) of $K_W$ is the plane [stabilizer](../../../group-theory.md#stabilizer-subgroup), each of order $168/7=24$. They give different [conjugacy classes](../../../group-theory.md#conjugacy-class) because their common fixed spaces have dimensions one and two. All line [stabilizers](../../../group-theory.md#stabilizer-subgroup) are conjugate, as are all plane [stabilizers](../../../group-theory.md#stabilizer-subgroup).

For an order-three element, its [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) is $(X-1)(X^2+X+1)$: it has a fixed line and an invariant complementary irreducible plane. Its [normalizer](../../../group-theory.md#normalizer) preserves both and is the full $GL_2(2)$ on that plane, of order six, since the order-three subgroup is normal in $GL_2(2)$. This [normalizer](../../../group-theory.md#normalizer) lies in the corresponding line and plane [stabilizers](../../../group-theory.md#stabilizer-subgroup), so is not maximal.

An order-seven element is irreducible. Over the [finite field](../../../algebra.md#finite-field) $\mathbb F_2$ one has $X^7-1=(X-1)(X^3+X+1)(X^3+X^2+1)$, and both cubic factors are irreducible because neither has a root in $\mathbb F_2$. Its [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial) divides this square-free product and cannot be just $X-1$, since the element is not the identity. It therefore contains a cubic factor; the three-dimensional space forces that irreducible cubic to be the whole [minimal polynomial](../../../linear-operator-theory.md#minimal-polynomial). Identify the space with $\mathbb F_8$ and the element with multiplication by a generator $\alpha$ of $\mathbb F_8^{\times}$. Its [centralizer](../../../group-theory.md#centralizer) consists of the seven nonzero multiplication maps. A [normalizer](../../../group-theory.md#normalizer) induces an $\mathbb F_2$-automorphism of this field, so it sends $\alpha$ to $\alpha$, $\alpha^2$ or $\alpha^4$. All three possibilities occur via the field [automorphisms](../../../algebra.md#automorphism) $x\mapsto x^{2^j}$. Therefore the [normalizer](../../../group-theory.md#normalizer) of the [Singer cycle](../../../finite-group-theory.md#singer-cycle) has order $7\cdot3=21$, and all such [normalizers](../../../group-theory.md#normalizer) are conjugate by the [Sylow theorems](../../../finite-group-theory.md#sylow-theorems).

The maximal-normalizer reduction leaves exactly the two order-twenty-four [stabilizer](../../../group-theory.md#stabilizer-subgroup) types and the order-twenty-one type. Each is maximal because it cannot be contained in any larger remaining candidate; equal-order subgroups cannot properly contain one another and $21$ does not divide $24$. Thus

$$
\boxed{GL_3(2)\text{ has exactly three maximal-subgroup classes, of orders }24,24,21.}
$$

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For $H\le G$ of finite [subgroup index](../../../group.md#index-of-a-subgroup), let $H'= [H,H]$ and choose a right-coset transversal $T$ for the [cosets](../../../group-theory.md#coset) $Ht$. For each $g\in G$ write

$$
tg=h(t,g)t_g,\qquad h(t,g)\in H,\quad t_g\in T.
$$

The [transfer homomorphism](../../../group-theory.md#transfer-group-theory) is

$$
\boxed{V_{G,H}(g)=\prod_{t\in T}h(t,g)\pmod{H'}\ \in H/H'.}
$$

The product is taken in the [abelianization](../../../group-theory.md#abelianization), so its order is irrelevant. If another transversal has representative $a_tt$ for $Ht$, with $a_t\in H$, its factor is $a_t h(t,g)a_{t_g}^{-1}$. The map $t\mapsto t_g$ permutes $T$, so the extra factors cancel in $H/H'$. This proves independence of the transversal. Also

$$
h(t,g_1g_2)=h(t,g_1)h(t_{g_1},g_2).
$$

Multiplying over $t$ and again permuting the second indices proves $V(g_1g_2)=V(g_1)V(g_2)$. Thus it is indeed a [group homomorphism](../../../group-theory.md#group-homomorphism).

The [Burnside transfer theorem](../../../group-theory.md#burnside-transfer-theorem) states that if a Sylow $p$-subgroup $P$ of a [finite group](../../../group.md#finite-group) satisfies $P\subseteq Z(N_G(P))$, then $G$ has a normal $p$-complement: a [normal subgroup](../../../group-theory.md#normal-subgroup) of order $|G|/|P|$. The hypothesis first makes $P$ abelian. It also makes fusion inside $P$ trivial. To prove this, suppose $u,v\in P$ and $u^g=v$, using $u^g=g^{-1}ug$. Both $P$ and $P^g$ lie in $C_G(v)$: the former because $P$ is abelian, and the latter because $v\in P^g$. They are [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) of that [centralizer](../../../group-theory.md#centralizer). Choose $c\in C_G(v)$ with $(P^g)^c=P$. Then $gc\in N_G(P)$ and $u^{gc}=v^c=v$, while the central-normalizer hypothesis gives $u^{gc}=u$. Thus $u=v$.

Evaluate transfer to the [abelian group](../../../group.md#abelian-group) $P$ on $u\in P$. In the action of $u$ on right [cosets](../../../group-theory.md#coset), a cycle of length $r$ contributes

$$
\prod_{j=0}^{r-1}t_jut_{j+1}^{-1}=t_0u^rt_0^{-1}\in P,
$$

with $t_r=t_0$. This is a conjugate of $u^r$ inside $P$ and hence equals $u^r$ by the fusion argument. Summing the cycle lengths therefore gives

$$
V_{G,P}(u)=u^{[G:P]}.
$$

The exponent is coprime to $p$, so this power map is an [automorphism](../../../algebra.md#automorphism) of the finite abelian $p$-group $P$. Transfer is consequently onto $P$, and its kernel is normal of [subgroup index](../../../group.md#index-of-a-subgroup) $|P|$ and of order prime to $p$. This proves the theorem. Notice also that a normal $p$-complement consists exactly of the elements of prime-to-$p$ order: they map trivially to the $p$-group quotient, while all elements of the complement have such order. It is therefore unique and a [characteristic subgroup](../../../algebra.md#characteristic-subgroup).

Now let $G\le A_p$ be primitive of degree $p=2q+1$, with $q$ prime. Every nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) of a faithful [primitive group action](../../../group-theory.md#primitive-group-action) is transitive: its orbits form a $G$-invariant block partition, and singleton orbits would make it trivial. Such a subgroup has order divisible by $p$. A Sylow $p$-subgroup $P$ has order $p$, since $p!$ contains only one factor $p$. The [normalizer](../../../group-theory.md#normalizer) of a regular $p$-cycle in $S_p$ is the affine group $x\mapsto ax+b$ on $\mathbb F_p$, of order $p(p-1)$. Translations are even, whereas a generating multiplier gives a $(p-1)$-cycle and is odd. Its [normalizer](../../../group-theory.md#normalizer) in $A_p$ therefore has order $p(p-1)/2=pq$.

Suppose $G$ is not simple and choose $1<N\triangleleft G$ proper. It is transitive, so we can choose $P\le N$. The [Frattini argument](../../../finite-group-theory.md#frattini-argument) gives $G=NN_G(P)$: for each $g$, the subgroup $P^g$ is a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) of $N$ and can be conjugated back to $P$ within $N$. Since $N_G(P)$ contains $P$ and lies in the order-$pq$ [normalizer](../../../group-theory.md#normalizer), it has order $p$ or $pq$. If its order were $p$, the Burnside theorem applied to $G$ would give a normal $p$-complement. A nontrivial such complement cannot be transitive because its order is prime to $p$, contradicting primitivity. It must be trivial, giving $G=P$, contrary to the choice of $N$. Thus $|N_G(P)|=pq$.

The intersection $N_N(P)$ again has order $p$ or $pq$. If it had order $pq$, the whole [normalizer](../../../group-theory.md#normalizer) would lie in $N$ and the Frattini equality would give $G=N$. Hence $N_N(P)=P$. Applying Burnside transfer within $N$ gives its normal $p$-complement $K$. By the uniqueness argument, $K$ is a [characteristic subgroup](../../../algebra.md#characteristic-subgroup) of $N$, and so normal in $G$. Primitivity again forces this prime-to-$p$ subgroup to be trivial. Thus $N=P$ is normal in $G$, and $G=N_G(P)$ has order $pq$. The [even primitive groups of safe-prime degree](../../../group-theory.md#even-primitive-groups-of-safe-prime-degree) conclusion is

$$
\boxed{G\text{ is simple, or }|G|=pq.}
$$

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

A [subnormal series](../../../group-theory.md#subnormal-series) of a [finite group](../../../group.md#finite-group) is a chain $1=G_0\triangleleft G_1\triangleleft\cdots\triangleleft G_r=G$. A [normal series of a group](../../../group-theory.md#normal-series-of-a-group) requires every $G_i$ normal in the whole group. This distinction matters: a [composition series](../../../finite-group-theory.md#composition-series) is a [subnormal series](../../../group-theory.md#subnormal-series) with nontrivial simple factors, whereas a [chief series](../../../group-theory.md#chief-series) is a strict, unrefinable [normal series of a group](../../../group-theory.md#normal-series-of-a-group), whose factors are [minimal normal subgroups](../../../group-theory.md#minimal-normal-subgroup) of the appropriate ambient quotients. Both exist in a [finite group](../../../group.md#finite-group), by successively choosing maximal proper [normal subgroups](../../../group-theory.md#normal-subgroup) or a maximal chain of ambient-normal subgroups. The direct-product result proved above shows that [chief factors](../../../group-theory.md#chief-factor) are powers of isomorphic [simple groups](../../../finite-group-theory.md#simple-group), rather than necessarily simple themselves.

The [Jordan–Hölder theorem](../../../finite-group-theory.md#jordan-holder-theorem) says that any two [composition series](../../../finite-group-theory.md#composition-series) have the same multiset of simple factors, up to isomorphism and order. Here is an induction proof. The assertion is trivial for the identity group. Let $A,B$ be the penultimate terms of two series for $G$; they are maximal proper [normal subgroups](../../../group-theory.md#normal-subgroup). If $A=B$, apply induction there. Otherwise $AB=G$, since its image is a nontrivial [normal subgroup](../../../group-theory.md#normal-subgroup) in each simple quotient. Put $C=A\cap B$. The maps to the quotients give

$$
A/C\cong G/B,\qquad B/C\cong G/A.
$$

For example, $a\mapsto aB$ has kernel $C$ and is onto because $AB=G$. Take a [composition series](../../../finite-group-theory.md#composition-series) of $C$ and append $A$, obtaining a [composition series](../../../finite-group-theory.md#composition-series) of $A$ because $A/C$ is simple; do the same with $B$. Induction inside these smaller groups shows that the factors in the two original series are, in both cases, the factors of $C$ together with $G/A$ and $G/B$. This proves the theorem and justifies the phrase [Jordan–Hölder factors](../../../finite-group-theory.md#jordan-holder-factor) independently of a chosen series.

The [derived series](../../../group-theory.md#derived-series) is $G^{(0)}=G$, $G^{(i+1)}=[G^{(i)},G^{(i)}]$. Its terms are [characteristic subgroups](../../../algebra.md#characteristic-subgroup), hence normal. A group is soluble if this series reaches the identity. Equivalently it admits a [subnormal series](../../../group-theory.md#subnormal-series) with abelian factors. One direction uses the [derived series](../../../group-theory.md#derived-series) itself. For the other, note the extension principle: if $N\triangleleft G$ has derived length $a$ and $G/N$ has derived length $b$, then $G^{(b)}\le N$, so $G^{(a+b)}=1$. Applying this principle along an abelian-factor series proves solubility.

Subgroups and quotients of a [soluble group](../../../group-theory.md#solvable-group) are soluble: $H^{(i)}\le G^{(i)}$ for a subgroup, and the [commutator subgroup](../../../group-theory.md#commutator-subgroup) of a quotient is the image of the [commutator subgroup](../../../group-theory.md#commutator-subgroup). A finite soluble [simple group](../../../finite-group-theory.md#simple-group) is abelian, since its [commutator subgroup](../../../group-theory.md#commutator-subgroup) is normal and cannot equal the whole group if the [derived series](../../../group-theory.md#derived-series) terminates. An abelian simple [finite group](../../../group.md#finite-group) is cyclic of prime order. Therefore **a [finite group](../../../group.md#finite-group) is soluble exactly when all its [Jordan–Hölder factors](../../../finite-group-theory.md#jordan-holder-factor) are cyclic of prime order**: necessity follows from the subgroup/quotient property, and sufficiency follows from the extension principle. Its [chief factors](../../../group-theory.md#chief-factor) are elementary abelian, by the minimal-normal-subgroup result.

For nilpotence, the [lower central series](../../../group-theory.md#lower-central-series) is $\gamma_1(G)=G$, $\gamma_{i+1}(G)=[\gamma_i(G),G]$. A group is nilpotent if $\gamma_{c+1}=1$ for some $c$. An ascending [central series](../../../group-theory.md#central-series) $1=N_0\le\cdots\le N_c=G$ satisfies $[N_{i+1},G]\le N_i$. Reversing a terminating [lower central series](../../../group-theory.md#lower-central-series) gives such a [central series](../../../group-theory.md#central-series). Conversely, induction gives $\gamma_i(G)\le N_{c-i+1}$, so any such [central series](../../../group-theory.md#central-series) forces $\gamma_{c+1}=1$. The [upper central series](../../../group-theory.md#upper-central-series) $Z_0=1$, $Z_{i+1}/Z_i=Z(G/Z_i)$ contains every ascending [central series](../../../group-theory.md#central-series) term by term, and thus reaches $G$ exactly in the nilpotent case. Because $[\gamma_i,\gamma_i]\le[\gamma_i,G]=\gamma_{i+1}$, induction gives $G^{(i)}\le\gamma_{i+1}$: **[nilpotent groups](../../../group-theory.md#nilpotent-group) are soluble**.

For [finite groups](../../../group.md#finite-group) there is the stronger structural characterization: **a [finite group](../../../group.md#finite-group) is nilpotent exactly when it is the [direct product of groups](../../../group-theory.md#direct-product-of-groups) formed from its [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup)**. To prove the forward direction, the [upper central series](../../../group-theory.md#upper-central-series) gives the [normalizer](../../../group-theory.md#normalizer) condition. If $H<G$, choose its first term $Z_i$ not contained in $H$, with $Z_{i-1}\le H$. An element of $Z_i\setminus H$ has all [group commutators](../../../group.md#group-commutator) with $H$ in $Z_{i-1}$, so normalizes $H$. Hence $H<N_G(H)$.

For a [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) $P$, its [normalizer](../../../group-theory.md#normalizer) is self-normalizing. Indeed, if $x$ normalizes $N_G(P)$, the two [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) $P^x,P$ of that [normalizer](../../../group-theory.md#normalizer) are conjugate there; adjusting $x$ by an element of $N_G(P)$ puts it in $N_G(P)$ already. Applying the strict [normalizer](../../../group-theory.md#normalizer) condition to $N_G(P)$ shows that it cannot be proper, so $P$ is normal. Normal [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) of distinct primes commute, since their [group commutators](../../../group.md#group-commutator) lie in their trivial intersection. Their product has [cardinality](../../../set-theory.md#cardinality) $|G|$ and is direct.

Conversely, a nontrivial finite $p$-group has nontrivial centre: in the class equation every noncentral [conjugacy class](../../../group-theory.md#conjugacy-class) has size divisible by $p$, so $p$ divides the centre's order. Induct on its order through the quotient by its centre to obtain an [upper central series](../../../group-theory.md#upper-central-series). Thus every finite $p$-group is nilpotent, and a finite [direct product of groups](../../../group-theory.md#direct-product-of-groups) of them is nilpotent because its [upper central series](../../../group-theory.md#upper-central-series) is obtained componentwise.

A finite [supersolvable group](../../../group-theory.md#supersolvable-group) has a [normal series of a group](../../../group-theory.md#normal-series-of-a-group) with cyclic prime-order factors. It is soluble, but the ambient-normal condition is stronger than the condition on a [composition series](../../../finite-group-theory.md#composition-series). Finite [nilpotent groups](../../../group-theory.md#nilpotent-group) are supersolvable: a $p$-group has a central subgroup of order $p$, and induction in its quotient builds an ambient-normal prime-factor series; [direct products of groups](../../../group-theory.md#direct-product-of-groups) of the Sylow factors combine these series. The converses fail. The group $S_3$ is supersolvable via $1<C_3<S_3$, but is not nilpotent because its Sylow $2$-subgroups are not normal. The group $A_4$ is soluble via $1<V_4<A_4$, but is not supersolvable: no subgroup of order two is normal, since the three involutions are conjugate, and no subgroup of order three is normal, since there are four such subgroups. In this example $1<C_2<V_4<A_4$ is a [composition series](../../../finite-group-theory.md#composition-series) whose first $C_2$ is not normal in $A_4$, while $1<V_4<A_4$ is a [chief series](../../../group-theory.md#chief-series) with a nonsimple [chief factor](../../../group-theory.md#chief-factor) $V_4$.

Finally, a [perfect group](../../../group-theory.md#perfect-group) satisfies $G'=G$. In any [finite group](../../../group.md#finite-group), the [derived series](../../../group-theory.md#derived-series) eventually stabilizes at a perfect [characteristic subgroup](../../../algebra.md#characteristic-subgroup), because a descending sequence of finite subgroup orders eventually stops decreasing. It is trivial exactly when the group is soluble. A nonabelian [simple group](../../../finite-group-theory.md#simple-group) is perfect: its nontrivial [commutator subgroup](../../../group-theory.md#commutator-subgroup) is normal and must be the whole group. Thus series distinguish successively stronger notions, summarize the building blocks through [Jordan–Hölder factors](../../../finite-group-theory.md#jordan-holder-factor), and separate soluble behaviour from a persistent perfect part.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

For a set of primes $\pi$, a Hall $\pi$-subgroup $H$ of a [finite group](../../../group.md#finite-group) is a subgroup whose order uses only primes in $\pi$ and whose [subgroup index](../../../group.md#index-of-a-subgroup) uses only primes outside $\pi$. Equivalently, $|H|$ is the full $\pi$-part of $|G|$. A [Hall subgroup](../../../group.md#hall-subgroup) is a Hall $\pi$-subgroup for some $\pi$. The theorem of P. Hall for finite [soluble groups](../../../group-theory.md#solvable-group) states: Hall $\pi$-subgroups exist for every $\pi$, any two are conjugate, and every $\pi$-subgroup is contained in a Hall $\pi$-subgroup.

For the existence proof, first give the explicit coprime splitting calculation needed in the induction. Let $N$ be elementary abelian of [field characteristic](../../../algebra.md#characteristic-of-a-field) $r$, normal in $E$, with $r\nmid|E/N|$. Write $Q=E/N$ and use additive notation on $N$. A normalized section $s:Q\to E$ gives an action $x\cdot n=s(x)ns(x)^{-1}$ independent of its choice, since $N$ is abelian. Write $s(x)s(y)=f(x,y)s(xy)$. Associativity gives

$$
f(x,y)+f(xy,z)=x\cdot f(y,z)+f(x,yz).
$$

Sum over $z\in Q$, put $S(x)=\sum_z f(x,z)$, and divide by $|Q|$ in the [vector space](../../../vector-space.md) $N$. This is legitimate because $r\nmid|Q|$. With $b(x)=|Q|^{-1}S(x)$ one obtains

$$
f(x,y)=b(x)+x\cdot b(y)-b(xy).
$$

The new section $s'(x)=(-b(x))s(x)$ therefore has zero multiplication defect and is a [group homomorphism](../../../group-theory.md#group-homomorphism). Its image is a complement to $N$.

We will also need a single [conjugation](../../../group-theory.md#conjugation) carrying one complement to the other. If two homomorphic sections differ by $d(x)$, their difference satisfies $d(xy)=d(x)+x\cdot d(y)$. Summing over $y$ gives $d(x)=c-x\cdot c$, where $c=|Q|^{-1}\sum_y d(y)$. Thus the second section is $c\,s(x)c^{-1}$. This proves, by explicit averaging, both [coprime splitting over an elementary abelian normal subgroup](../../../group-theory.md#coprime-splitting-over-an-elementary-abelian-normal-subgroup) and the existence of such a [conjugation](../../../group-theory.md#conjugation) by an element of $N$.

Now induct on $|G|$ for [Hall subgroup existence in soluble groups](../../../group.md#hall-subgroup-existence-in-soluble-groups). A [minimal normal subgroup](../../../group-theory.md#minimal-normal-subgroup) $N$ of a finite [soluble group](../../../group-theory.md#solvable-group) is elementary abelian of some [field characteristic](../../../algebra.md#characteristic-of-a-field) $r$. Indeed, $N'$ is a [characteristic subgroup](../../../algebra.md#characteristic-subgroup) of $N$ and normal in $G$; it cannot equal $N$ because $N$ is soluble, so it is trivial. In this [abelian group](../../../group.md#abelian-group), a nontrivial primary component is a [characteristic subgroup](../../../algebra.md#characteristic-subgroup), forcing a single prime, and the [characteristic subgroup](../../../algebra.md#characteristic-subgroup) annihilated by that prime forces exponent $r$.

By induction $G/N$ has a Hall $\pi$-subgroup $\overline H$, with preimage $M$. If $M<G$, induction in $M$ supplies a Hall $\pi$-subgroup of $M$, which is also Hall in $G$ because $[G:M]$ is prime to all primes in $\pi$. If $M=G$, the quotient is a $\pi$-group. When $r\in\pi$, $G$ itself is a $\pi$-group. When $r\notin\pi$, the averaging construction splits off $N$, and its complement has order $|G/N|$ and is the required Hall $\pi$-subgroup. This completes the existence proof, including the identity group and empty prime set.

A [Sylow basis](../../../finite-group-theory.md#sylow-basis) is a family $\{P_p:p\mid|G|\}$ containing one [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) for each prime, with $P_pP_q=P_qP_p$ for each pair. This is permutability of subgroups, not commutation of all their elements. The product of any subfamily is a subgroup: commuting the factors as sets proves closure and closure under inversion. Inductively its order is the product of the prime-power orders, since the newly adjoined factor has trivial intersection with the earlier product. It is thus the corresponding [Hall subgroup](../../../group.md#hall-subgroup).

Prove existence of a [Sylow basis](../../../finite-group-theory.md#sylow-basis) by induction on $|G|$, again using elementary abelian $N$ of [field characteristic](../../../algebra.md#characteristic-of-a-field) $r$. Choose a basis $\{\overline P_p\}$ of $G/N$, taking $\overline P_r=1$ if $r$ does not divide that quotient's order. The product $\overline H=\prod_{p\ne r}\overline P_p$ is its Hall $r'$-subgroup. In its full preimage $T$, the averaging lemma supplies a complement $H$ to $N$, mapping isomorphically to $\overline H$. For $p\ne r$, let $P_p$ be the inverse image of $\overline P_p$ under this isomorphism within $H$. Let $P_r$ be the full preimage of $\overline P_r$ in $G$. These are [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) of $G$. The other-prime pairs permute because they do so in $\overline H$. For $P_r$ and $P_p$, their product is contained in the full preimage of the subgroup $\overline P_r\overline P_p$ and has exactly that preimage's order $|N|\,|\overline P_r|\,|\overline P_p|$. Equality follows, so the product is a subgroup and these two factors permute as well. This constructs a basis.

To obtain a simultaneous [conjugation](../../../group-theory.md#conjugation) of two bases, take two bases. Their images in $G/N$ are bases: $N$ lies in every Sylow $r$-subgroup, and the other-prime [Sylow subgroups](../../../finite-group-theory.md#sylow-subgroup) project injectively. By induction, conjugate one basis so that all corresponding images agree. The products of their non-$r$ factors are then two complements to $N$ in the same preimage $T$ of their common Hall $r'$-subgroup. The averaging lemma for complements supplies a single element of $N$ conjugating these complements. In the resulting common complement each corresponding [Sylow subgroup](../../../finite-group-theory.md#sylow-subgroup) is the unique lift of its agreed quotient subgroup, so all non-$r$ factors agree. The $r$-factors already equal the full preimage of their common quotient factor and are preserved by [conjugation](../../../group-theory.md#conjugation) from $N$. Thus **all [Sylow bases](../../../finite-group-theory.md#sylow-basis) of a finite [soluble group](../../../group-theory.md#solvable-group) are conjugate**.

In $S_4$ there are three Sylow $2$-subgroups of order eight: the action on the three pair-partitions of four points has kernel $V_4$, and these subgroups are the preimages of the three order-two subgroups of $S_3$. There are four Sylow $3$-subgroups, one for each three-point support. Every choice $P_2,P_3$ has trivial intersection and product of cardinality $8\cdot3=24$, so $P_2P_3=S_4=P_3P_2$. Therefore

$$
\boxed{b(S_4)=3\cdot4=12.}
$$

For $E=V\rtimes S_4$, $V=\mathbb F_5^4$, the Sylow $5$-subgroup is uniquely $V$. In a [Sylow basis](../../../finite-group-theory.md#sylow-basis) the product $P_2P_3$ is a Hall $5'$-subgroup, hence a complement to $V$. Conversely, a basis of any complement together with $V$ is a basis of $E$, because $V$ is normal. The averaging lemma makes all complements conjugate by $V$. The [stabilizer](../../../group-theory.md#stabilizer-subgroup) of the standard complement $S_4$ under this [conjugation](../../../group-theory.md#conjugation) is $C_V(S_4)$: if a vector normalizes it, its [group commutator](../../../group.md#group-commutator) with each complement element lies in both $V$ and that complement, hence is trivial. The fixed vectors under the natural coordinate [permutation action](../../../group-theory.md#group-action) are exactly $(a,a,a,a)$, so $|C_V(S_4)|=5$. There are consequently $5^4/5=125$ complements, and each has twelve bases. The complement is uniquely recovered from its basis as $P_2P_3$, so no basis is counted twice. The [counting Sylow bases in a coprime elementary abelian extension](../../../finite-group-theory.md#counting-sylow-bases-in-a-coprime-elementary-abelian-extension) formula yields

$$
\boxed{b(5^4\rtimes S_4)=125\cdot12=1500.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
