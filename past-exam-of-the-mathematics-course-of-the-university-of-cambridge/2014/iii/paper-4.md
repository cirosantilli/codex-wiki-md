# Paper 4

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_4.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_4.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
- [5](#5)
  - [Solution](#5/solution)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
  - [iv](#5/iv)
    - [Solution](#5/iv/solution)

## 1

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Construct the [free product](../../../algebraic-topology.md#free-product) from the empty word and all finite alternating words $g_1\cdots g_k$, whose [syllables in a free product](../../../algebraic-topology.md#syllable-in-a-free-product) are nonidentity elements of tagged copies of $G_1,G_2$, with adjacent syllables from different factors. Multiply by concatenating, multiplying adjacent elements in the same factor, and deleting identities until the word is reduced. The [normal form theorem for a free product](../../../algebraic-topology.md#normal-form-theorem-for-a-free-product) gives a unique result; reducing three concatenated words gives the same result under either parenthesization, so multiplication is associative. The empty word is the identity, and the inverse reverses the word and inverts each syllable. Each factor embeds as words of length one.

The [universal property of a free product](../../../algebraic-topology.md#universal-property-of-a-free-product) says that for every [group](../../../group.md) $K$ and [group homomorphisms](../../../group-theory.md#group-homomorphism) $f_i:G_i\to K$ there is a unique [group homomorphism](../../../group-theory.md#group-homomorphism) $f:G_1*G_2\to K$ extending both. Explicitly, send a reduced word to the product of its syllable images; reduction preserves this product. This gives existence, while generation by the two factors gives uniqueness.

A standard form of [Klein's combination theorem](../../../geometric-group-theory.md#ping-pong-lemma), or the [ping-pong lemma](../../../geometric-group-theory.md#ping-pong-lemma), is the following. Let nontrivial [subgroups](../../../group.md#subgroup) $G_1,G_2$ of the [homeomorphisms](../../../topology.md#homeomorphism) of a [topological space](../../../topology.md#topological-space) $X$ have disjoint nonempty [subsets](../../../set.md#subset) $X_1,X_2$ with

$$
g(X_2)\subseteq X_1\quad(1\ne g\in G_1),\qquad h(X_1)\subseteq X_2\quad(1\ne h\in G_2).
$$

Assume also that at least one factor has at least three elements. Then **the generated [subgroup](../../../group.md#subgroup) is $\boxed{\langle G_1,G_2\rangle\cong G_1*G_2}$**. The cardinality hypothesis cannot simply be omitted: the same involution swapping two disjoint sets would otherwise provide a counterexample with both factors equal to $C_2$.

Here is the [ping-pong lemma](../../../geometric-group-theory.md#ping-pong-lemma) proof. A reduced word of odd length begins and ends in the same factor, so repeated application of the displayed inclusions sends the other factor's domain into that factor's domain. Disjointness shows that the word is not the identity. For an even reduced word, relabel the factors so that $|G_1|\geq3$, and invert the word if necessary to make it begin with $g\in G_1$ and end in $G_2$. Choose $s\in G_1\setminus\{1,g^{-1}\}$. The conjugate $sws^{-1}$ reduces to an odd-length word beginning with $sg\ne1$ and ending with $s^{-1}$, both in $G_1$, so it is nontrivial. Thus no nonempty reduced word lies in the kernel of the natural [group homomorphism](../../../group-theory.md#group-homomorphism) $G_1*G_2\to\langle G_1,G_2\rangle$, proving the theorem.

For an explicit example, let $X=\mathbb R\cup\{\infty\}$ be the one-dimensional [Real projective space](../../../algebraic-topology.md#real-projective-space), and take the [Möbius transformations](../../../group-theory.md#mobius-transformation)

$$
A(t)=t+2,\qquad B(t)=\frac{t}{2t+1},\qquad X_1=\{t:|t|>1\}\cup\{\infty\},\quad X_2=\{t:|t|<1\}.
$$

For every nonzero [integer](../../../number-theory.md#integer) $n$, $A^n(t)=t+2n$ sends $X_2$ into $X_1$, while $B^n(t)=t/(2nt+1)$ sends $X_1$ into $X_2$. Indeed $|2nt+1|>|t|$ when $|t|>1$, and $B^n(\infty)=1/(2n)$. Both transformations have infinite order. Hence the [ping-pong lemma](../../../geometric-group-theory.md#ping-pong-lemma) gives **$\boxed{\langle A,B\rangle\cong\mathbb Z*\mathbb Z=F_2}$**, a [free product](../../../algebraic-topology.md#free-product) of two nontrivial [finitely presented groups](../../../geometric-group-theory.md#finitely-presented-group).

A [finitely presented group](../../../geometric-group-theory.md#finitely-presented-group) admits a [group presentation](../../../geometric-group-theory.md#group-presentation) $\langle S\mid R\rangle$ with both $S$ and $R$ finite; it is the quotient of the [free group](../../../geometric-group-theory.md#free-group) on $S$ by the [normal closure](../../../group-theory.md#normal-closure) of $R$. If

$$
G=\langle S\mid R\rangle,\qquad H=\langle T\mid U\rangle
$$

with disjoint generator sets, then

$$
\boxed{G*H=\langle S\sqcup T\mid R\sqcup U\rangle.}
$$

Maps from this [group presentation](../../../geometric-group-theory.md#group-presentation) to any [group](../../../group.md) are exactly pairs of maps from $G$ and $H$, so the [universal property of a free product](../../../algebraic-topology.md#universal-property-of-a-free-product) proves the formula.

For a [group homomorphism](../../../group-theory.md#group-homomorphism) $\phi:H\to\operatorname{Aut}(G)$, choose a word $w_{t,s}(S)$ representing $\phi(t)(s)$ for each $t\in T,s\in S$. The [presentation of a semidirect product](../../../group-theory.md#presentation-of-a-semidirect-product) is

$$
\boxed{G\rtimes_\phi H=\langle S\sqcup T\mid R,U,\ t s t^{-1}=w_{t,s}\ (t\in T,s\in S)\rangle.}
$$

The presentation maps onto the specified [semidirect product](../../../group-theory.md#semidirect-product). Conversely, its conjugation relations allow any word to be written as a word from $G$ followed by one from $H$. The natural maps from the two factors to the presented group satisfy the full action relation, because conjugation agrees with $\phi$ first on generators and hence on all elements. They define the reverse [group homomorphism](../../../group-theory.md#group-homomorphism) $(g,h)\mapsto gh$. The two maps are inverse on every generator, proving the [group isomorphism](../../../algebra.md#group-isomorphism). There are finitely many cross-relations, so the result is again a [finitely presented group](../../../geometric-group-theory.md#finitely-presented-group).

Apply this to the specified permutation action. The presentation is

$$
\langle x,y,z,c\mid c^3=1,\ cxc^{-1}=y,\ cyc^{-1}=z,\ czc^{-1}=x\rangle.
$$

Eliminate $y=cxc^{-1}$ and $z=c^2xc^{-2}$. The last cross-relation becomes $c^3xc^{-3}=x$, already implied by $c^3=1$. Thus

$$
\boxed{F_3\rtimes_\phi C_3\cong\langle x,c\mid c^3=1\rangle\cong\mathbb Z*C_3.}
$$

Both factors are nontrivial [finitely presented groups](../../../geometric-group-theory.md#finitely-presented-group), as required.

## 2

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

A [soluble group](../../../group-theory.md#solvable-group), also called a [solvable group](../../../group-theory.md#solvable-group), has a terminating [derived series](../../../group-theory.md#derived-series):

$$
G^{(0)}=G,\qquad G^{(j+1)}=[G^{(j)},G^{(j)}],\qquad G^{(r)}=1\text{ for some }r\geq0.
$$

For a [subgroup](../../../group.md#subgroup) $S\leq G$, induction gives $S^{(j)}\leq G^{(j)}$, so subgroups of [soluble groups](../../../group-theory.md#solvable-group) are soluble. For a surjective [group homomorphism](../../../group-theory.md#group-homomorphism) $q:G\to Q$, $q(G^{(j)})=Q^{(j)}$, so quotients of [soluble groups](../../../group-theory.md#solvable-group) are soluble. Finally, in a [group extension](../../../group-theory.md#group-extension) $1\to K\to E\to Q\to1$, suppose $K^{(r)}=1$ and $Q^{(s)}=1$. Then $E^{(s)}\leq K$ and $E^{(s+r)}=1$. **[Soluble groups](../../../group-theory.md#solvable-group) are closed under [subgroups](../../../group.md#subgroup), quotients and [group extensions](../../../group-theory.md#group-extension).**

A [virtually soluble group](../../../group-theory.md#virtually-solvable-group) contains a [soluble group](../../../group-theory.md#solvable-group) as a [finite-index subgroup](../../../group.md#finite-index-subgroup). The finite-index facts proved in parts (i)–(iii) imply closure under [subgroups](../../../group.md#subgroup) and quotients: intersect a finite-index soluble subgroup with the chosen subgroup, or take its image under the quotient map.

For [group extensions](../../../group-theory.md#group-extension), no finite-generation hypothesis may be inserted. We first establish the [finite-index characteristic soluble subgroup](../../../group-theory.md#finite-index-characteristic-soluble-subgroup) lemma. If $K$ is a [virtually soluble group](../../../group-theory.md#virtually-solvable-group), the kernel of its action on the cosets of a finite-index soluble subgroup is a soluble [normal subgroup](../../../group-theory.md#normal-subgroup) $K_0$ of finite index. Among soluble [normal subgroups](../../../group-theory.md#normal-subgroup) containing $K_0$, choose $R$ with maximal $|R/K_0|$, possible because $K/K_0$ is finite. If $S$ is any soluble [normal subgroup](../../../group-theory.md#normal-subgroup) of $K$, then $RS$ is soluble: it is an extension of $R$ by $S/(R\cap S)$. Maximality forces $S\leq R$. Thus $R$ is the unique largest soluble [normal subgroup](../../../group-theory.md#normal-subgroup) of $K$, making it a [characteristic subgroup](../../../algebra.md#characteristic-subgroup), and it has finite index.

Now suppose $1\to K\to G\overset{\pi}{\to}Q\to1$ has both $K$ and $Q$ virtually soluble. Replace $G$ by the preimage $G_0$ of a finite-index soluble subgroup of $Q$. The subgroup $R$ just constructed is characteristic in $K$ and therefore normal in $G_0$. In $E=G_0/R$, the subgroup $A=K/R$ is a finite [normal subgroup](../../../group-theory.md#normal-subgroup), and $E/A$ is a [soluble group](../../../group-theory.md#solvable-group). The [centralizer](../../../group-theory.md#centralizer) $C_E(A)$ has finite index in $E$, since conjugation gives a map $E\to\operatorname{Aut}(A)$ with finite image. Its intersection with $A$ is the [center of a group](../../../group-theory.md#center-of-a-group) $Z(A)$, an [abelian group](../../../group.md#abelian-group), while its quotient by $Z(A)$ embeds in the soluble group $E/A$. Thus $C_E(A)$ is a [soluble group](../../../group-theory.md#solvable-group). Its preimage in $G_0$ is an extension by $R$, so it too is soluble and has finite index in $G$. **[Virtually soluble groups](../../../group-theory.md#virtually-solvable-group) are closed under [group extensions](../../../group-theory.md#group-extension).**

For the final example take the [restricted direct sum of groups](../../../group-theory.md#restricted-direct-sum-of-groups)

$$
\boxed{D=\bigoplus_{j\geq1}A_5,}
$$

where $A_5$ is the nonabelian [simple group](../../../finite-group-theory.md#simple-group) of even permutations on five letters. Every finite collection of elements lies in a product of finitely many finite factors, so $D$ is a [locally finite group](../../../group-theory.md#locally-finite-group) and hence a [torsion group](../../../group-theory.md#torsion-group). It cannot contain a nonabelian [free group](../../../geometric-group-theory.md#free-group), which is a [torsion-free group](../../../group.md#torsion-free-group).

To show that $D$ is not a [virtually soluble group](../../../group-theory.md#virtually-solvable-group), let $H$ be any [finite-index subgroup](../../../group.md#finite-index-subgroup) and let $N\leq H$ be the kernel of the finite coset action. Each coordinate $A_5$ maps either injectively or trivially into the finite quotient $D/N$, by [Simplicity of the alternating group A5](../../../finite-group-theory.md#simplicity-of-the-alternating-group-a5). The nontrivial images of distinct factors commute, and each has trivial centre, so any $k$ of them generate a [direct product of groups](../../../group-theory.md#direct-product-of-groups) of order $60^k$. Only finitely many such images can occur in a finite quotient. Therefore $N$, and hence $H$, contains a whole coordinate copy of $A_5$, which is not soluble: its nontrivial [commutator subgroup](../../../group-theory.md#commutator-subgroup) is normal and therefore equals $A_5$. **No finite-index subgroup of $D$ is soluble.**

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The map between left-coset [sets](../../../set.md)

$$
S/(S\cap H)\longrightarrow G/H,\qquad s(S\cap H)\longmapsto sH
$$

is well defined and [injective](../../../algebra.md#injective-function): equality of the images is equivalent to $s_2^{-1}s_1\in H$, and this element already lies in $S$. These are coset sets, not asserted quotient groups, since $H$ need not be normal. Thus the [index of a subgroup](../../../group.md#index-of-a-subgroup) satisfies

$$
\boxed{[S:S\cap H]\leq[G:H]<\infty.}
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Apply part (i) with $S=L$ and use multiplicativity of the [index of a subgroup](../../../group.md#index-of-a-subgroup) along a subgroup chain:

$$
\boxed{[G:H\cap L]=[G:L]\,[L:H\cap L]\leq[G:L]\,[G:H]<\infty.}
$$

Thus the intersection of two [finite-index subgroups](../../../group.md#finite-index-subgroup) again has finite index.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The map of coset [sets](../../../set.md)

$$
G/H\longrightarrow R/\theta(H),\qquad gH\longmapsto\theta(g)\theta(H)
$$

is well defined and [surjective](../../../algebra.md#surjective-function), because the [group homomorphism](../../../group-theory.md#group-homomorphism) $\theta$ is surjective. Therefore

$$
\boxed{[R:\theta(H)]\leq[G:H]<\infty.}
$$

No normality assumption on $H$ is required.

## 3

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $n=[G:H]<\infty$. The [group action](../../../group-theory.md#group-action) by left multiplication on $G/H$ gives a [group homomorphism](../../../group-theory.md#group-homomorphism) $G\to S_n$. Its kernel is the [normal core of a subgroup](../../../group-theory.md#core-group-theory),

$$
\boxed{N=\bigcap_{g\in G}gHg^{-1}\trianglelefteq G,\qquad N\leq H,\qquad[G:N]\leq n!.}
$$

The containment follows by looking at the stabilizer of the coset $H$, and finite index follows from the finite image in $S_n$.

The [Higman group](../../../geometric-group-theory.md#higman-group) is

$$
J=\langle a,b,c,d\mid aba^{-1}=b^2,\ bcb^{-1}=c^2,\ cdc^{-1}=d^2,\ dad^{-1}=a^2\rangle.
$$

It is visibly a [finitely presented group](../../../geometric-group-theory.md#finitely-presented-group). To prove infinitude, first form

$$
K=\langle a,b,c\mid aba^{-1}=b^2,\ bcb^{-1}=c^2\rangle.
$$

It is the [amalgamated free product](../../../algebraic-topology.md#amalgamated-free-product) of $\langle a,b\mid aba^{-1}=b^2\rangle$ and $\langle b,c\mid bcb^{-1}=c^2\rangle$, identifying their infinite cyclic subgroups generated by $b$. Each factor is an [HNN extension](../../../geometric-group-theory.md#hnn-extension) of an [infinite cyclic group](../../../group.md#infinite-cyclic-group), so its base and stable letter both have infinite order. No nonzero power of $a$ belongs to $\langle b\rangle$ in the first factor, by the map to $\mathbb Z$ sending $a$ to one and $b$ to zero. In the second factor, no nonzero power of $c$ belongs to $\langle b\rangle$: the stable-letter map forces a hypothetical equality $c^k=b^l$ to have $l=0$, and the base $c$ has infinite order. The [normal form theorem for an amalgamated free product](../../../geometric-group-theory.md#normal-form-theorem-for-an-amalgamated-free-product) therefore shows that $\langle a,c\rangle\leq K$ is a rank-two [free group](../../../geometric-group-theory.md#free-group).

Similarly,

$$
L=\langle c,d,a\mid cdc^{-1}=d^2,\ dad^{-1}=a^2\rangle
$$

contains $\langle c,a\rangle$ as a rank-two [free group](../../../geometric-group-theory.md#free-group). Identifying these two free subgroups yields

$$
J=K*_{\langle a,c\rangle}L.
$$

The [normal form theorem for an amalgamated free product](../../../geometric-group-theory.md#normal-form-theorem-for-an-amalgamated-free-product) embeds $K$ in $J$. In particular, $J$ contains a [free group](../../../geometric-group-theory.md#free-group) of rank two and is **infinite**.

The [finite quotients of cyclic squaring presentations](../../../geometric-group-theory.md#finite-quotients-of-cyclic-squaring-presentations) argument now rules out every nontrivial finite quotient of $J$. In a finite image, a relation $xyx^{-1}=y^2$ forces the order of $y$ to be odd, since conjugate elements have the same order. If any generator has nontrivial image, let $p$ be the least [prime number](../../../number-theory.md#prime-number) dividing the order of any of the four generator images, and choose $y$ whose order is divisible by $p$. Its predecessor $x$ conjugates it to its square. If $r$ is the order of $x$, iterating conjugation gives $2^r\equiv1\pmod p$. Hence the [multiplicative order](../../../number-theory.md#multiplicative-order) of $2$ modulo $p$ divides $r$. It is greater than one and divides $p-1$, so it has a [prime factor](../../../number-theory.md#prime-factor) smaller than $p$, which also divides $r$. This contradicts the minimal choice of $p$. Thus all four generator images are trivial. **$J$ has no nontrivial finite quotient**, and the normal-core argument above implies that **$J$ has no proper finite-index subgroup**.

For the final argument, [Conjugation](../../../group-theory.md#conjugation) preserves the order of an element. Thus if one nonidentity element has finite order $n$, every nonidentity element has that same order, and $n\geq2$. Moreover $n$ is prime: if a [prime factor](../../../number-theory.md#prime-factor) $p$ properly divides $n$, then $g^p$ is nonidentity but has the smaller order $n/p$.

When $n\geq3$, the element $g^2$ is nonidentity, so choose $x$ with $xgx^{-1}=g^2$. The conjugator is not the identity, since $g^2\ne g$, and therefore $x^n=1$. Induction gives $x^kgx^{-k}=g^{2^k}$, and at $k=n$ this yields

$$
g=g^{2^n},\qquad n\mid2^n-1.
$$

But [Fermat's little theorem](../../../number-theory.md#fermat-little-theorem), with the odd prime $n$, gives $2^n\equiv2\pmod n$, contradicting that divisibility.

For $n=2$, $g^2=1$ is not in the nonidentity [conjugacy class](../../../group-theory.md#conjugacy-class), so the required conjugator cannot be chosen. Instead, a group in which every element has square one is an [abelian group](../../../group.md#abelian-group): $(ab)^{-1}=ab$ also equals $b^{-1}a^{-1}=ba$. In an [abelian group](../../../group.md#abelian-group) every [conjugacy class](../../../group-theory.md#conjugacy-class) is a singleton, so one nonidentity class permits only one nonidentity element, giving a group of order two. This contradicts infinitude. **Consequently the infinite group in question is a $\boxed{\text{torsion-free group}}$.**

This establishes the [torsion-freeness from one nonidentity conjugacy class](../../../group-theory.md#torsion-freeness-from-one-nonidentity-conjugacy-class) criterion.

## 4

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [residually finite group](../../../group-theory.md#residually-finite-group) $G$ has the property that every $1\ne g\in G$ survives under a [group homomorphism](../../../group-theory.md#group-homomorphism) to some [finite group](../../../group.md#finite-group). Equivalently, the intersection of its finite-index [normal subgroups](../../../group-theory.md#normal-subgroup) is trivial. A [Hopfian group](../../../group-theory.md#hopfian-group) is a [group](../../../group.md) for which every surjective [endomorphism](../../../algebra.md#endomorphism) is an [automorphism](../../../algebra.md#automorphism).

Suppose $G$ is generated by $d$ elements. A [group homomorphism](../../../group-theory.md#group-homomorphism) $G\to S_n$ is determined by the images of these generators, so there are at most $(n!)^d$ such maps. Every subgroup of index $n$ gives a transitive coset [group action](../../../group-theory.md#group-action) on an $n$-element [set](../../../set.md), and the subgroup is the stabilizer of a point in that action. There are at most $n$ point stabilizers per action. The [finite-index subgroup count for a finitely generated group](../../../group.md#finite-index-subgroup-count-for-a-finitely-generated-group) therefore gives

$$
\boxed{\#\{H\leq G:[G:H]=n\}\leq n(n!)^d<\infty.}
$$

Now let $\psi:G\to G$ be a surjective [endomorphism](../../../algebra.md#endomorphism). For any fixed $n$, inverse image under $\psi$ preserves the index of a [normal subgroup](../../../group-theory.md#normal-subgroup). It is also an [injective function](../../../algebra.md#injective-function) on the finite [set](../../../set.md) of normal subgroups of index $n$: if $\psi^{-1}(M)=\psi^{-1}(N)$, surjectivity gives $M=N$. It is therefore a [permutation](../../../combinatorics.md#permutation) of that finite [set](../../../set.md). Given any finite-index [normal subgroup](../../../group-theory.md#normal-subgroup) $N$, there is another such subgroup $M$ with $N=\psi^{-1}(M)$, so $\ker\psi\leq N$. If $G$ is a [residually finite group](../../../group-theory.md#residually-finite-group), intersecting all these $N$ gives $\ker\psi=1$. Hence $\psi$ is an [automorphism](../../../algebra.md#automorphism). **Every [finitely generated group](../../../group.md#finitely-generated-group) that is a [residually finite group](../../../group-theory.md#residually-finite-group) is a [Hopfian group](../../../group-theory.md#hopfian-group).**

A useful [residual finiteness of semidirect products](../../../group-theory.md#residual-finiteness-of-semidirect-products) theorem is: if $K$ is a [finitely generated group](../../../group.md#finitely-generated-group), then

$$
\boxed{K\rtimes H\text{ is residually finite}\iff K\text{ and }H\text{ are residually finite}.}
$$

More generally, the forward construction only requires that $K$ have a separating family of finite-index [normal subgroups](../../../group-theory.md#normal-subgroup) invariant under the $H$ action, and that $H$ be a [residually finite group](../../../group-theory.md#residually-finite-group). Necessity follows by restricting finite separating maps to the embedded [subgroups](../../../group.md#subgroup) $K$ and $H$.

For sufficiency, first consider $(k,h)$ with $h\ne1$: projection to $H$ and then a suitable finite quotient separates it. If $h=1$ and $k\ne1$, choose a finite-index [normal subgroup](../../../group-theory.md#normal-subgroup) $U\trianglelefteq K$ with $k\notin U$. Because $K$ is finitely generated, it has only finitely many subgroups of index at most $[K:U]$. Their intersection $C$ is a finite-index [characteristic subgroup](../../../algebra.md#characteristic-subgroup) of $K$, is contained in $U$, and is invariant under every automorphism in the $H$ action. The quotient $K/C$ is finite. Let $\rho:H\to\operatorname{Aut}(K/C)$ be the induced action. The map

$$
K\rtimes H\longrightarrow (K/C)\rtimes\rho(H),\qquad (x,y)\longmapsto(xC,\rho(y))
$$

is a [group homomorphism](../../../group-theory.md#group-homomorphism) to a [finite group](../../../group.md#finite-group) and separates $(k,1)$. This proves the theorem and the more general invariant-subgroup criterion. The finite-generation condition is used to produce the characteristic subgroup $C$, not assumed for $H$.

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The first [Baumslag-Solitar group](../../../geometric-group-theory.md#baumslag-solitar-group) is

$$
\langle a,b\mid bab^{-1}=a^{-1}\rangle\cong\mathbb Z\rtimes\mathbb Z,
$$

where the second [infinite cyclic group](../../../group.md#infinite-cyclic-group) acts on the first by inversion. The [presentation of a semidirect product](../../../group-theory.md#presentation-of-a-semidirect-product) proves this identification; both copies of $\mathbb Z$ are [residually finite groups](../../../group-theory.md#residually-finite-group), since reduction modulo a suitable positive integer separates any nonzero integer. The normal factor is finitely generated, so the [residual finiteness of semidirect products](../../../group-theory.md#residual-finiteness-of-semidirect-products) theorem applies. **$\boxed{BS(1,-1)\text{ is residually finite}.}$**

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

**$\boxed{BS(3,4)\text{ is not residually finite}.}$** We exhibit a nonidentity element killed by every finite quotient.

In any finite image, let $r$ be the order of the image of $a$. The relation conjugating $a^3$ to $a^4$ gives

$$
\frac r{\gcd(r,3)}=\frac r{\gcd(r,4)}.
$$

Thus $\gcd(r,3)=\gcd(r,4)=1$. Since $3$ is invertible modulo $r$, the relation implies that the image of $bab^{-1}$ is a power of the image of $a$. Therefore every finite image kills the [group commutator](../../../group.md#group-commutator)

$$
w=[a,bab^{-1}]=a^{-1}b a^{-1}b^{-1}a b a b^{-1},
$$

using $[s,t]=s^{-1}t^{-1}st$.

View $BS(3,4)$ as an [HNN extension](../../../geometric-group-theory.md#hnn-extension) of $\langle a\rangle\cong\mathbb Z$, with associated subgroups $\langle a^3\rangle$ and $\langle a^4\rangle$. A [pinch in an HNN extension](../../../geometric-group-theory.md#pinch-in-an-hnn-extension) would be $ba^{3j}b^{-1}$ or $b^{-1}a^{4j}b$. The word $w$ has none: its intervening exponents are $-1,1,1$, incompatible with the required divisibilities $3,4,3$. By [Britton's lemma](../../../geometric-group-theory.md#britton-s-lemma), $w\ne1$. Hence finite quotients fail to separate this nonidentity element, proving the conclusion.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Both displayed matrices have determinant one and integer entries, so the generated [group](../../../group.md) $M$ lies in $\operatorname{SL}_2(\mathbb Z)$. For any nonidentity matrix $g\in M$, some entry of $g-I$ is a nonzero integer $k$. Choose a [prime number](../../../number-theory.md#prime-number) $p$ not dividing $k$. The [reduction modulo a prime in an integral matrix group](../../../group-theory.md#reduction-modulo-a-prime-in-an-integral-matrix-group) gives a [group homomorphism](../../../group-theory.md#group-homomorphism)

$$
M\longrightarrow\operatorname{SL}_2(\mathbb F_p)
$$

to a [finite group](../../../group.md#finite-group) in which $g$ is nonidentity. **$\boxed{M\text{ is residually finite}.}$** No determination of the abstract subgroup generated by the two matrices is needed.

## 5

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For a [group presentation](../../../geometric-group-theory.md#group-presentation) $\mathcal P=\langle X\mid R\rangle$ with $X$ finite, let $F(X)$ be its [free group](../../../geometric-group-theory.md#free-group). For a nontrivial relator define

$$
\nu_p(r)=\max\{k\geq0:r=w^{p^k}\text{ for some }w\in F(X)\}.
$$

The [p-deficiency](../../../geometric-group-theory.md#p-deficiency) in the unshifted convention used here is

$$
\boxed{\operatorname{def}_p(\mathcal P)=|X|-\sum_{r\in R}p^{-\nu_p(r)}.}
$$

If the weighted sum diverges the value is $-\infty$; identity relators may be omitted or assigned weight zero. Roots are taken in the [free group](../../../geometric-group-theory.md#free-group), not in the presented quotient. Some authors subtract one from this definition; here the requested threshold is $1$.

Two elementary bounds explain why [p-deficiency](../../../geometric-group-theory.md#p-deficiency) detects infinitude. The [p-rank of a group](../../../geometric-group-theory.md#p-rank-of-a-group) is

$$
d_p(G)=\dim_{\mathbb F_p}\bigl(G/[G,G]G^p\bigr).
$$

Here $G^p$ denotes the subgroup generated by all $p$th powers. Each relator that is not a $p$th power imposes at most one linear relation in this [vector space](../../../vector-space.md), and a $p$th-power relator imposes none. If there are $s$ relators of the first type, then

$$
d_p(G)\geq |X|-s\geq\operatorname{def}_p(\mathcal P).
$$

The second bound is the [index-p rewriting bound for p-deficiency](../../../geometric-group-theory.md#index-p-rewriting-bound-for-p-deficiency). Suppose $H\trianglelefteq G$ has index $p$, and its preimage in $F(X)$ is $V$. The [Nielsen–Schreier formula](../../../geometric-group-theory.md#nielsen-schreier-formula) gives $V$ rank $1+p(|X|-1)$. For a relator $r=w^{p^k}$, there are two cases in the [Reidemeister–Schreier theorem](../../../geometric-group-theory.md#reidemeister-schreier-theorem). If $w\in V$, its $p$ coset-conjugates are all $p^k$th powers in $V$, with total weight at most $p\,p^{-k}$. If $w\notin V$, then $k\geq1$, since $r\in V$. Its cosets generate $F(X)/V$, so representatives $1,w,\ldots,w^{p-1}$ show that the $p$ rewritten conjugates of $r$ are redundant up to conjugation in $V$. One relator suffices, and $r=(w^p)^{p^{k-1}}$ has weight at most $p^{-(k-1)}$. In both cases the total weight is at most $p$ times the old weight. Thus the induced [group presentation](../../../geometric-group-theory.md#group-presentation) $\mathcal Q$ of $H$ satisfies

$$
\boxed{\operatorname{def}_p(\mathcal Q)-1\geq p\bigl(\operatorname{def}_p(\mathcal P)-1\bigr).}
$$

The argument applies termwise to infinitely many relators whenever the weighted sum converges.

If $\operatorname{def}_p(\mathcal P)\geq1$, the [p-rank of a group](../../../geometric-group-theory.md#p-rank-of-a-group) bound gives a surjection to $C_p$, hence a normal subgroup of index $p$. The rewriting bound gives that subgroup another presentation of [p-deficiency](../../../geometric-group-theory.md#p-deficiency) at least one. Iterating produces subgroups of index $p^j$ for every $j$. **[p-deficiency at least one implies infinitude](../../../geometric-group-theory.md#p-deficiency-at-least-one-implies-infinitude).**

Now enumerate the nonidentity elements $w_1,w_2,\ldots$ of $F(x,y)$ and choose the presentation

$$
T=\langle x,y\mid w_i^{p^{i+2}}=1\ (i\geq1)\rangle.
$$

Its [p-deficiency](../../../geometric-group-theory.md#p-deficiency) obeys

$$
\operatorname{def}_p(T)\geq2-\sum_{i\geq1}p^{-(i+2)}=2-\frac1{p^2(p-1)}>1.
$$

The infinitude criterion shows that $T$ is infinite. It is generated by two elements, and every element is represented by some $w_i$ or is the identity; the imposed relation makes its order a power of $p$. Thus **$\boxed{T\text{ is an infinite finitely generated torsion group}}$**. This is a [torsion group construction by p-power relators](../../../geometric-group-theory.md#torsion-group-construction-by-p-power-relators); the presentation intentionally has infinitely many relators.

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

**No prime and no presentation of $G_1$ have [p-deficiency](../../../geometric-group-theory.md#p-deficiency) at least one.** Abelianizing the cyclic squaring relations makes each generator zero: for example $vwv^{-1}=w^2$ becomes $w=2w$, so $w=0$, and the other four relations kill $x,y,z,v$. Thus the [abelianization](../../../group-theory.md#abelianization) of $G_1$ is trivial and $d_p(G_1)=0$ for every [prime number](../../../number-theory.md#prime-number) $p$. The presentation-independent [p-rank of a group](../../../geometric-group-theory.md#p-rank-of-a-group) bound from the general solution gives

$$
\boxed{\operatorname{def}_p(\mathcal P)\leq d_p(G_1)=0}
$$

for every [group presentation](../../../geometric-group-theory.md#group-presentation) $\mathcal P$ of $G_1$. This rules out alternative presentations, not just the one displayed.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

**Yes, for $p=2$.** The displayed [group presentation](../../../geometric-group-theory.md#group-presentation) is that of the infinite [dihedral group](../../../finite-group-theory.md#dihedral-group). Put $u=at$ and $v=t$. Then $v^2=1$ and

$$
u^2=atat=a(tat^{-1})t^2=aa^{-1}=1.
$$

Conversely, from $u^2=v^2=1$, set $a=uv$ and $t=v$; then $tat^{-1}=vu=a^{-1}$. These inverse substitutions give

$$
G_2\cong\langle u,v\mid u^2,v^2\rangle\cong C_2*C_2.
$$

Each relator has free-group $2$-root exponent one, so

$$
\boxed{\operatorname{def}_2(\langle u,v\mid u^2,v^2\rangle)=2-\frac12-\frac12=1.}
$$

The change of presentation matters: the original presentation's mixed conjugation relator has weight one and would give a smaller [p-deficiency](../../../geometric-group-theory.md#p-deficiency).

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

**No prime and no presentation of $G_3$ have [p-deficiency](../../../geometric-group-theory.md#p-deficiency) at least one.** Set $r=xy$. The relations give

$$
r^{1024}=1,\qquad x^2=1,\qquad xrx^{-1}=r^{-1},\qquad y=xr.
$$

Every element has form $r^j$ or $r^jx$ with $0\leq j<1024$. Conversely, the usual rotations and reflections of a regular $1024$-gon satisfy the presentation and give $2048$ distinct elements. Hence $G_3$ is the finite [dihedral group](../../../finite-group-theory.md#dihedral-group) of order $2048$. The criterion [p-deficiency at least one implies infinitude](../../../geometric-group-theory.md#p-deficiency-at-least-one-implies-infinitude) excludes every alternative presentation and every prime. As a check, the given presentation has

$$
\operatorname{def}_2=2-\frac12-\frac12-\frac1{1024}=1-\frac1{1024}<1.
$$

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

**Yes: the displayed presentation already has [p-deficiency](../../../geometric-group-theory.md#p-deficiency) exactly one for $p=2$.** The words $x,y,z,xy,yz,zx$ are not proper powers in the [free group](../../../geometric-group-theory.md#free-group). For the length-two words this follows directly from their distinct consecutive letters in a [cyclically reduced word](../../../geometric-group-theory.md#cyclically-reduced-word). Thus each relator's $2$-root exponent is precisely the exponent of $2$ in its displayed power. The relator weights, in the given order, are

$$
\frac12,\quad1,\quad\frac14,\quad\frac1{16},\quad\frac1{16},\quad\frac18.
$$

Their sum is $2$, giving

$$
\boxed{\operatorname{def}_2=3-\left(\frac12+1+\frac14+\frac1{16}+\frac1{16}+\frac18\right)=1.}
$$

In particular the infinitude criterion proves that this group is infinite, although the question only asks for the existence of the presentation and prime.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
