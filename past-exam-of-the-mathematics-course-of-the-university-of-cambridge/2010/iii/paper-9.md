# Paper 9

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper9.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper9.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For $a<b$, give the pair $\{a,b\}$ the color determined by $v_2(b-a)\bmod2$, where $v_2$ is the [2-adic valuation](../../../number-theory.md#2-adic-valuation): use red for even valuation and blue for odd valuation. This [finite coloring](../../../ramsey-theory.md#finite-coloring) works because the pairs $\{a,a+d\}$ and $\{a,a+2d\}$ have valuations $v_2(d)$ and $v_2(d)+1$. They therefore have opposite colors. In particular, **no three-term [arithmetic progression](../../../arithmetic.md#arithmetic-progression) has all its pairs [monochromatic](../../../ramsey-theory.md#monochromatic-set)**.

For the second assertion, $m=1$ is immediate: every singleton is a blue complete [arithmetic progression](../../../arithmetic.md#arithmetic-progression), since it has no pairs to check. Assume $m\geq2$. If some $m$-term [arithmetic progression](../../../arithmetic.md#arithmetic-progression) has all its pairs blue, we are done. Otherwise, every such [arithmetic progression](../../../arithmetic.md#arithmetic-progression) contains a red pair. For each $(a,d)\in\mathbb N^2$, choose, say lexicographically, indices $0\leq r<s<m$ for which $\{a+rd,a+sd\}$ is red, and color $(a,d)$ by this chosen pair $(r,s)$. This is a [finite coloring](../../../ramsey-theory.md#finite-coloring) with at most $\binom m2$ colors.

We need a lattice pattern that works whichever pair becomes the common color. Fix, before applying the [Gallai theorem for an integer lattice](../../../ramsey-theory.md#gallai-theorem-for-an-integer-lattice), the finite set

$$
F=\bigcup_{0\leq r<s<m}\{(si-rj,j-i):0\leq i,j<m\}\subseteq\mathbb Z^2.
$$

Translate $F$ into the positive quadrant and apply the [Gallai theorem for an integer lattice](../../../ramsey-theory.md#gallai-theorem-for-an-integer-lattice) to that translated pattern. Absorbing the translation into the base point gives integers $a_0,d_0$ and $q>0$ such that $(a_0,d_0)+qF\subseteq\mathbb N^2$ is [monochromatic](../../../ramsey-theory.md#monochromatic-set). Write $(r,s)$ for its common color. Since $(0,0)\in F$, the base point itself has positive coordinates.

For each $0\leq i,j<m$, the parameter point

$$
(a,d)=\bigl(a_0+q(si-rj),\ d_0+q(j-i)\bigr)
$$

belongs to that [monochromatic](../../../ramsey-theory.md#monochromatic-set) copy and has chosen red pair $(r,s)$. Its red endpoints simplify to

$$
a+rd=a_0+rd_0+q(s-r)i,\qquad a+sd=a_0+sd_0+q(s-r)j.
$$

Consequently, putting

$$
A=\{a_0+rd_0+q(s-r)i:0\leq i<m\},\qquad B=\{a_0+sd_0+q(s-r)j:0\leq j<m\},
$$

gives two $m$-term [arithmetic progressions](../../../arithmetic.md#arithmetic-progression) of positive [common difference](../../../arithmetic.md#common-difference) $q(s-r)$, with every cross-pair red. These [arithmetic progressions](../../../arithmetic.md#arithmetic-progression) really are disjoint: the parameter point corresponding to $i=m-1,j=0$ has positive second coordinate, so $d_0>q(m-1)$. Hence

$$
\min B-\max A=(s-r)\bigl(d_0-q(m-1)\bigr)>0.
$$

This proves the **[arithmetic-progression bipartite Ramsey dichotomy](../../../ramsey-theory.md#arithmetic-progression-bipartite-ramsey-dichotomy)**, including the required disjointness.

## 2

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Here is the matrix form of [Rado's theorem](../../../ramsey-theory.md#rado-s-theorem). A [matrix](../../../vector-space.md#matrix) $A$ with entries in the [rational numbers](../../../number-theory.md#rational-number) and columns $a_1,\ldots,a_n$ is a [partition regular matrix](../../../ramsey-theory.md#partition-regular-matrix) if every [finite coloring](../../../ramsey-theory.md#finite-coloring) of the [positive integers](../../../number-theory.md#positive-integer) admits a vector $x\in\mathbb N^n$ whose coordinates are [monochromatic](../../../ramsey-theory.md#monochromatic-set) and for which $Ax=0$. Its [columns condition](../../../ramsey-theory.md#columns-property) asks for an ordered partition into nonempty blocks $B_1,\ldots,B_s$, with

$$
b_1:=\sum_{i\in B_1}a_i=0,\qquad b_j:=\sum_{i\in B_j}a_i\in\operatorname{span}_{\mathbb Q}\{a_i:i\in B_1\cup\cdots\cup B_{j-1}\}\quad(j>1).
$$

**[Rado's theorem](../../../ramsey-theory.md#rado-s-theorem) states that these two conditions are equivalent.** Coordinates need not be distinct; positivity is required for every coordinate.

First prove necessity using the [finite separating-functional proof of the columns condition](../../../ramsey-theory.md#finite-separating-functional-proof-of-the-columns-condition). Clearing denominators does not change either the [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) or the [columns condition](../../../ramsey-theory.md#columns-property), so assume that $A$ has [integer](../../../number-theory.md#integer) entries. For each pair of disjoint index sets $I,B\subseteq\{1,\ldots,n\}$, with $B$ nonempty, for which $b_B=\sum_{i\in B}a_i$ is outside the rational [linear span](../../../vector-space.md#linear-span) of the $I$-columns, choose an integer [linear functional](../../../linear-algebra.md#linear-functional) $\ell_{I,B}$ such that

$$
\ell_{I,B}(a_i)=0\ (i\in I),\qquad \ell_{I,B}(b_B)\ne0.
$$

Such a [linear functional](../../../linear-algebra.md#linear-functional) exists: extend a [basis](../../../vector-space.md#basis) over the [rational numbers](../../../number-theory.md#rational-number) of the indicated [linear span](../../../vector-space.md#linear-span) by $b_B$, prescribe values zero on the former basis and one on $b_B$, extend to a [basis](../../../vector-space.md#basis) of the ambient [vector space over the rational numbers](../../../vector-space.md#vector-space-over-the-rational-numbers), and then clear the functional's denominators. There are only finitely many pairs $(I,B)$. Choose a [prime number](../../../number-theory.md#prime-number) $p$ larger than the absolute values of all their nonzero evaluations; if there are none, choose any [prime number](../../../number-theory.md#prime-number).

Color $x>0$ by its [last nonzero digit coloring](../../../ramsey-theory.md#last-nonzero-digit-coloring) value, namely

$$
u(x):=x/p^{v_p(x)}\pmod p\in\{1,\ldots,p-1\},
$$

where $v_p$ is the [P-adic valuation](../../../number-theory.md#p-adic-valuation). By [partition regularity](../../../ramsey-theory.md#partition-regular-matrix), choose a positive solution $Ax=0$ all of whose coordinates have the same nonzero digit $u$. Group its indices into nonempty blocks $B_1,\ldots,B_s$ according to increasing distinct [P-adic valuations](../../../number-theory.md#p-adic-valuation) $\nu_1<\cdots<\nu_s$.

Suppose that a block sum $b_j$ is outside the rational [linear span](../../../vector-space.md#linear-span) of the earlier columns, and put $I=B_1\cup\cdots\cup B_{j-1}$, taking $I=\varnothing$ for $j=1$. Apply the selected [linear functional](../../../linear-algebra.md#linear-functional) $\ell_{I,B_j}$ to $Ax=0$. The earlier terms vanish exactly. Divide the remaining integer equality by $p^{\nu_j}$ and reduce modulo $p$. Later blocks vanish modulo $p$, while each coordinate in $B_j$ contributes its common digit $u$. We obtain

$$
0\equiv u\,\ell_{I,B_j}(b_j)\pmod p,
$$

which is impossible by the choice of $p$ and because $u\not\equiv0\pmod p$. Thus each block sum lies in the earlier [linear span](../../../vector-space.md#linear-span). For the first block, this span is zero, so $b_1=0$. This proves the [columns condition](../../../ramsey-theory.md#columns-property).

For sufficiency, assume the [columns condition](../../../ramsey-theory.md#columns-property) and choose rational coefficients $\lambda_{ij}$, for $i\in B_1\cup\cdots\cup B_{j-1}$, such that

$$
b_j+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\lambda_{ij}a_i=0\qquad(j>1).
$$

Choose a positive integer $c$ clearing all these coefficients' denominators and a positive integer $p$ with $p\geq|c\lambda_{ij}|$ for every coefficient. Use the permitted [monochromatic m-p-c set theorem](../../../ramsey-theory.md#monochromatic-m-p-c-set-theorem), in the suffix convention for an [m-p-c set](../../../ramsey-theory.md#m-p-c-set), to obtain positive generators $z_1,\ldots,z_s$ such that the full set

$$
D=\bigcup_{h=1}^s\left\{cz_h+\sum_{j>h}\mu_jz_j:\mu_j\in\mathbb Z,\ |\mu_j|\leq p\right\}
$$

is positive and [monochromatic](../../../ramsey-theory.md#monochromatic-set). The positivity of the full [m-p-c set](../../../ramsey-theory.md#m-p-c-set) is important: we do not discard expressions that happen to be negative. For $i\in B_h$, set

$$
x_i=cz_h+\sum_{j>h}c\lambda_{ij}z_j.
$$

All these coordinates belong to $D$, so they are positive and [monochromatic](../../../ramsey-theory.md#monochromatic-set). On collecting coefficients of each $z_j$, their matrix product is

$$
Ax=c z_1b_1+\sum_{j=2}^s c z_j\left(b_j+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\lambda_{ij}a_i\right)=0.
$$

This explicit [Rado solution inside an m-p-c set](../../../ramsey-theory.md#rado-solution-inside-an-m-p-c-set) proves sufficiency and completes the proof of [Rado's theorem](../../../ramsey-theory.md#rado-s-theorem).

To deduce the [Finite sums theorem](../../../ramsey-theory.md#finite-sums-theorem) directly from the [columns condition](../../../ramsey-theory.md#columns-property), introduce one positive variable $y_F$ for each nonempty $F\subseteq\{1,\ldots,k\}$ and impose

$$
\sum_{i\in F}y_{\{i\}}-y_F=0\qquad(|F|\geq2).
$$

For $k=1$ there are no equations and any positive integer works. For $k\geq2$, write $a_F$ for the column belonging to $y_F$. Partition the columns into blocks $B_j=\{F:\min F=j\}$ in the order $j=1,\ldots,k$. Consider the row indexed by a set $H$ with $|H|\geq2$. The sum of the columns in $B_j$ has row value

$$
\boldsymbol{1}_{\{j\in H\}}-\boldsymbol{1}_{\{\min H=j\}}.
$$

For $j=1$ this is always zero. For $j>1$ it equals one exactly for those $H$ with $\min H<j$ and $j\in H$. Each such $a_H$ is the negative coordinate vector in row $H$, and it belongs to an earlier block. Therefore

$$
\sum_{F\in B_j}a_F=-\sum_{\substack{|H|\geq2,\ \min H<j\\j\in H}}a_H\quad(j>1),
$$

which verifies the [columns condition](../../../ramsey-theory.md#columns-property), rather than assuming the desired [Finite sums theorem](../../../ramsey-theory.md#finite-sums-theorem). Apply [Rado's theorem](../../../ramsey-theory.md#rado-s-theorem) to this system. Its [monochromatic](../../../ramsey-theory.md#monochromatic-set) positive solution satisfies $y_F=\sum_{i\in F}x_i$ with $x_i=y_{\{i\}}$, and hence

$$
\boxed{\operatorname{FS}(x_1,\ldots,x_k)=\left\{\sum_{i\in F}x_i:\varnothing\ne F\subseteq\{1,\ldots,k\}\right\}\text{ is monochromatic}.}
$$

## 3

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Call $A\subseteq\mathbb N$ an [IP set](../../../ramsey-theory.md#ip-set) when it contains an infinite [finite-sums set](../../../ramsey-theory.md#finite-sums-set) $\operatorname{FS}(x_1,x_2,\ldots)$ with all $x_i>0$. We first need the relative consequence of the [Hindman theorem](../../../ramsey-theory.md#hindman-theorem): **a finite union can be an [IP set](../../../ramsey-theory.md#ip-set) only if one of its constituents is an [IP set](../../../ramsey-theory.md#ip-set)**. This does not follow by simply applying the theorem to a coloring of all integers, because its [monochromatic](../../../ramsey-theory.md#monochromatic-set) [finite-sums set](../../../ramsey-theory.md#finite-sums-set) might lie outside the given set.

Here is a reduction that proves the [partition regularity of IP sets](../../../ramsey-theory.md#partition-regularity-of-ip-sets). Suppose $\operatorname{FS}(x_i)\subseteq A$ and $A$ is finitely colored. Index the generators by $i\geq0$. For $n>0$, let $S(n)$ be the set of positions of the nonzero digits in its [binary expansion](../../../arithmetic.md#binary-expansion), and color $n$ by the color of $\sum_{i\in S(n)}x_i$. By the [Hindman theorem](../../../ramsey-theory.md#hindman-theorem), there are $w_1,w_2,\ldots>0$ with $\operatorname{FS}(w_i)$ [monochromatic](../../../ramsey-theory.md#monochromatic-set) in this new [finite coloring](../../../ramsey-theory.md#finite-coloring).

We can take disjoint, successively later finite blocks of the $w_i$ whose sums $v_1,v_2,\ldots$ have separated [binary expansion](../../../arithmetic.md#binary-expansion) supports. Start with $v_1=w_1$. Having chosen finitely many blocks, take $K$ larger than every binary position used in their sums. On a fresh tail of the $w_i$, consider $2^K+1$ partial sums, including the zero partial sum. Two have the same [residue class](../../../number-theory.md#residue-class) modulo $2^K$, by the [pigeonhole principle](../../../algebra.md#pigeonhole-principle). Their positive difference is a consecutive block sum $v_{j+1}$ divisible by $2^K$. Discard all indices up to that block's end and repeat. Thus every bit of $v_{j+1}$ is above every bit in the preceding block sums.

There are no carries in a sum of distinct $v_j$, so

$$
S\left(\sum_{j\in J}v_j\right)=\bigsqcup_{j\in J}S(v_j)\qquad(\varnothing\ne J\text{ finite}).
$$

Also $\operatorname{FS}(v_j)\subseteq\operatorname{FS}(w_i)$, since the underlying blocks are disjoint. Consequently

$$
y_j:=\sum_{i\in S(v_j)}x_i
$$

satisfies $\operatorname{FS}(y_j)\subseteq\operatorname{FS}(x_i)\subseteq A$, with all these sums the same original color. This proves the relative assertion. In particular, if $A_1\cup\cdots\cup A_r$ contains an infinite [finite-sums set](../../../ramsey-theory.md#finite-sums-set), color its points by the first constituent containing them and apply this argument; one $A_j$ is an [IP set](../../../ramsey-theory.md#ip-set).

Let $\mathcal I$ be the family of sets that are not [IP sets](../../../ramsey-theory.md#ip-set). It is closed under subsets and, by the preceding argument, under finite unions. It contains every [finite set](../../../set.md#finite-set), since positive successive partial sums of an infinite sequence are unbounded. It does not contain $\mathbb N$. Therefore

$$
\mathcal F=\{A\subseteq\mathbb N:A^c\in\mathcal I\}
$$

is a proper [filter on a set](../../../set-theory.md#filter-set-theory): it contains $\mathbb N$, excludes the empty set, is upward closed, and is closed under finite intersections. Its members are exactly the [IP-star sets](../../../ramsey-theory.md#ip-star-set), the sets meeting every [IP set](../../../ramsey-theory.md#ip-set). Indeed, failure to meet an [IP set](../../../ramsey-theory.md#ip-set) is equivalent to having an IP complement. This identifies the sets that must belong to the required [ultrafilter](../../../set-theory.md#ultrafilter).

Apply the [ultrafilter lemma](../../../set-theory.md#ultrafilter-lemma) to extend the [IP-star filter](../../../ramsey-theory.md#ip-star-filter) $\mathcal F$ to an [ultrafilter](../../../set-theory.md#ultrafilter) $\mathcal U$. For completeness, [Zorn lemma](../../../set-theory.md#zorn-s-lemma) applies to its proper filter extensions ordered by inclusion, because the union of a chain is still a proper [filter on a set](../../../set-theory.md#filter-set-theory). A maximal extension decides every set $A$: if $A$ cannot be adjoined while keeping the filter proper, some filter member is disjoint from $A$, forcing $A^c$ into the filter. This is the defining [ultrafilter](../../../set-theory.md#ultrafilter) property.

If $A\in\mathcal U$ were not an [IP set](../../../ramsey-theory.md#ip-set), then $A^c\in\mathcal F\subseteq\mathcal U$, contradicting properness. Hence **every member of $\mathcal U$ contains an infinite [finite-sums set](../../../ramsey-theory.md#finite-sums-set)**. Conversely, any [ultrafilter with finite-sums members](../../../set-theory.md#ultrafilter-with-finite-sums-members) must contain every [IP-star set](../../../ramsey-theory.md#ip-star-set), since it cannot contain such a set's non-IP complement. Thus this construction captures precisely the forced filter, without making an unnecessary claim about idempotence.

To prove nonuniqueness, put

$$
E=\bigcup_{j\geq0}\bigl([2^{2j},2^{2j+1})\cap\mathbb N\bigr).
$$

For a nonempty finite set of exponents with largest exponent $J$, the associated sum of distinct powers of four satisfies

$$
4^J\leq\sum_{j\in F}4^j\leq\frac{4^{J+1}-1}{3}<2\cdot4^J.
$$

Thus $\operatorname{FS}(4^j:j\geq0)\subseteq E$. Doubling the inequality gives

$$
2\cdot4^J\leq\sum_{j\in F}2\cdot4^j<4\cdot4^J,
$$

so $\operatorname{FS}(2\cdot4^j:j\geq0)\subseteq E^c$. These [alternating dyadic intervals contain disjoint IP sets](../../../ramsey-theory.md#alternating-dyadic-intervals-contain-disjoint-ip-sets).

Every member of $\mathcal F$ meets $E$ and also $E^c$, because it meets every [IP set](../../../ramsey-theory.md#ip-set). A finite intersection of members of $\mathcal F$ is again a member, so both $\mathcal F\cup\{E\}$ and $\mathcal F\cup\{E^c\}$ have the [finite intersection property](../../../topology.md#finite-intersection-property). Extend the proper filters they generate to [ultrafilters](../../../set-theory.md#ultrafilter) $\mathcal U_0$ and $\mathcal U_1$. Each extends $\mathcal F$, so the previous argument makes each an [ultrafilter with finite-sums members](../../../set-theory.md#ultrafilter-with-finite-sums-members). But $E\in\mathcal U_0$ and $E^c\in\mathcal U_1$, so

$$
\boxed{\mathcal U_0\ne\mathcal U_1.}
$$

## 4

↑ **Parent:** [Paper 9](paper-9.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write $X=[\mathbb N]^\omega$ for the [space of infinite subsets of the natural numbers](../../../ramsey-theory.md#space-of-infinite-subsets-of-the-natural-numbers), and $[M]^\omega$ for all infinite subsets of an infinite $M$. A family $Y\subseteq X$ is a [Ramsey set of infinite subsets](../../../ramsey-theory.md#ramsey-set-of-infinite-subsets) if for every infinite $M$ there is an infinite $L\subseteq M$ with either $[L]^\omega\subseteq Y$ or $[L]^\omega\cap Y=\varnothing$.

A non-[Ramsey set of infinite subsets](../../../ramsey-theory.md#ramsey-set-of-infinite-subsets) is obtained by [finite-symmetric-difference parity colouring](../../../ramsey-theory.md#finite-symmetric-difference-parity-colouring). Declare $A\sim B$ when their [symmetric difference](../../../set.md#symmetric-difference) is finite, and use the [axiom of choice](../../../set-theory.md#axiom-of-choice) to select a representative $R$ for each [equivalence class](../../../set-theory.md#equivalence-class). Put

$$
\varepsilon(A)=|A\mathbin{\triangle}R|\pmod2,\qquad Y=\{A\in X:\varepsilon(A)=0\}.
$$

For every infinite $L$, both $L$ and $L\setminus\{\min L\}$ belong to $[L]^\omega$ and have the same representative. Toggling one element changes the parity of the finite [symmetric difference](../../../set.md#symmetric-difference), so these two sets have opposite colors. Thus no $[L]^\omega$ is homogeneous, and **$Y$ is not a [Ramsey set of infinite subsets](../../../ramsey-theory.md#ramsey-set-of-infinite-subsets)**. Only finite differences are counted; no parity is being assigned to an infinite cardinal.

We use the [Ellentuck topology](../../../ramsey-theory.md#ellentuck-topology) for the star notation. Its basic neighborhoods are

$$
[s,A]=\{s\cup B:B\in[A]^\omega\},
$$

where $s$ is a finite stem (the [initial segment](../../../set.md#initial-segment) of each member of the neighborhood) and every element of the infinite reservoir $A$ exceeds $\max s$; the empty stem is allowed. A star-[nowhere dense set](../../../topological-analysis.md#nowhere-dense-set) $N$ has star-[closure](../../../topology.md#closure-topology) with empty star-[interior](../../../topology.md#interior-topology); a star-[meagre set](../../../topological-analysis.md#meagre-set) is a [countable](../../../set-theory.md#countable-set) union of star-[nowhere dense sets](../../../topological-analysis.md#nowhere-dense-set).

We need the following stem-preserving open-set conclusion: a star-[open set](../../../topology.md#open-set) $G$ has, in every $[s,A]$, an infinite $B\subseteq A$ such that $[s,B]\subseteq G$ or $[s,B]\cap G=\varnothing$. Here is the [fusion proof for open Ellentuck sets](../../../ramsey-theory.md#fusion-proof-for-open-ellentuck-sets), so that the precise form being used is explicit. A reservoir $T$ accepts a finite extension $t$ of $s$ when $[t,T]\subseteq G$, and rejects it when no infinite subreservoir accepts it. Every reservoir can be thinned to decide a prescribed stem: take an accepting subreservoir if one exists, and otherwise it already rejects. Acceptance and rejection are hereditary under further infinite thinning.

First thin $A$ to decide $s$. If it accepts, we have finished. Otherwise, choose successive points $b_0<b_1<\cdots$, thinning the unused tail after each selection to decide every stem $s\cup t$ with $t$ a subset of the finitely many points already selected. Each stage requires only finitely many decisions. The final set $B$ therefore decides every such finite extension, using the tail above its largest point. It rejects $s$.

For any rejected stem $s\cup t$, only finitely many possible next points $b$ of $B$ have accepting tails for $s\cup t\cup\{b\}$. Otherwise collect infinitely many such points into $C$. Every member of $[s\cup t,C]$ starts with some such $b$, and its remaining points lie in the accepting tail above $b$. Hence $[s\cup t,C]\subseteq G$, contradicting rejection. A second selection now gives $C\subseteq B$ all of whose finite extensions of $s$ are rejected: at each stage avoid the finitely many forbidden next points for each subset of the chosen prefix. Previous rejections persist on thinning. If $Z\in[s,C]\cap G$, star-openness gives an initial stem $s\cup t$ of $Z$ and an infinite tail of $Z$ whose entire neighborhood lies in $G$. This is an accepting subreservoir for a stem we made rejected, a contradiction. Thus $[s,C]\cap G=\varnothing$, proving the needed open-set conclusion.

Apply this conclusion to $G=X\setminus\overline N^{\,*}$ when $N$ is star-[nowhere dense](../../../topological-analysis.md#nowhere-dense-set). This $G$ is star-[open](../../../topology.md#open-set) and star-[dense](../../../topology.md#dense-set). The alternative $[s,B]\cap G=\varnothing$ would give a nonempty star-[open set](../../../topology.md#open-set) inside $\overline N^{\,*}$, contradicting empty [interior](../../../topology.md#interior-topology). Consequently **every star-[nowhere dense set](../../../topological-analysis.md#nowhere-dense-set) can be avoided without extending the finite stem**.

Now let $N=\bigcup_{j\geq0}N_j$, each $N_j$ star-[nowhere dense](../../../topological-analysis.md#nowhere-dense-set), and fix $[s,A]$. Construct $b_0<b_1<\cdots$ with nested infinite unused reservoirs. At stage $j$, let $P_j=\{b_0,\ldots,b_{j-1}\}$. For every $t\subseteq P_j$, in turn, thin the current reservoir using the preceding avoidance property until

$$
[s\cup t,C_j]\cap N_j=\varnothing\qquad(t\subseteq P_j).
$$

There are only finitely many such $t$, and subsequent thinning preserves all previous avoidances. Choose $b_j=\min C_j$ and retain the part of $C_j$ above $b_j$ for the next stage. Put $B=\{b_j:j\geq0\}$. For any $Z\in[s,B]$ and any $j$, the finite part $t=(Z\setminus s)\cap P_j$ is one of the stems tested at stage $j$, and the rest of $Z\setminus(s\cup t)$ lies in $C_j$. Hence $Z\in[s\cup t,C_j]$ and $Z\notin N_j$. This proves $[s,B]\cap N=\varnothing$.

The final $[s,B]$ is star-[open](../../../topology.md#open-set) and disjoint from $N$, so it is also disjoint from the star-[closure](../../../topology.md#closure-topology) of $N$. Every basic neighborhood therefore has a nonempty open refinement missing that closure. This [Ellentuck meagre-set fusion lemma](../../../ramsey-theory.md#ellentuck-meagre-set-fusion-lemma) proves

$$
\boxed{\text{star-meagre}\ \Longrightarrow\ \text{star-nowhere dense}.}
$$

Indeed, we obtained the stronger [completely Ramsey-null](../../../ramsey-theory.md#completely-ramsey-null-set) property. Testing all subsets of the selected prefix was essential; testing just the entire prefix would not cover every infinite subset of $B$.

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Take $\tau$ to be the [ordinary topology on infinite subsets](../../../ramsey-theory.md#ordinary-topology-on-infinite-subsets), whose basic cylinders $[s]$ fix a finite [initial segment](../../../set.md#initial-segment). Let

$$
D=\{Z\in[\mathbb N]^\omega:\mathbb N\setminus Z\text{ is finite}\}.
$$

This is a [dense countable family of cofinite infinite subsets](../../../ramsey-theory.md#dense-countable-family-of-cofinite-infinite-subsets). It is countable because finite complements form a countable family. Each singleton is $\tau$-[closed](../../../topology.md#closed-set): distinct increasing enumerations differ at some finite coordinate, which separates them by cylinders. No singleton has [interior](../../../topology.md#interior-topology), since every cylinder admits more than one infinite continuation. Thus every singleton is $\tau$-[nowhere dense](../../../topological-analysis.md#nowhere-dense-set), and $D$ is $\tau$-[meagre](../../../topological-analysis.md#meagre-set).

On the other hand, every cylinder $[s]$ contains the [cofinite set](../../../set-theory.md#cofinite-set) $s\cup\{n:n>\max s\}$, with $\max\varnothing=0$. Hence $D$ is $\tau$-[dense](../../../topology.md#dense-set), its [closure](../../../topology.md#closure-topology) is all of $X$, and

$$
\boxed{D\text{ is }\tau\text{-meagre but not }\tau\text{-nowhere dense}.}
$$

The paper does not define its symbol $\tau$. If the course instead uses it for the [Ramsey cone topology](../../../ramsey-theory.md#ramsey-cone-topology), with basic neighborhoods $[A]^\omega$ and no finite stem, use $X$ itself as the example. For $D_j=\{Z:\min Z=j\}$, its cone-[closure](../../../topology.md#closure-topology) is $\{Z:j\in Z\}$: every cone neighborhood of a set containing $j$ contains an infinite subset of minimum $j$, while a cone based on a set omitting $j$ misses $D_j$. This [closure](../../../topology.md#closure-topology) has empty [interior](../../../topology.md#interior-topology), because every infinite reservoir can be thinned to omit $j$. Thus every $D_j$ is cone-[nowhere dense](../../../topological-analysis.md#nowhere-dense-set), and $X=\bigcup_{j\geq1}D_j$ is cone-[meagre](../../../topological-analysis.md#meagre-set) but is not cone-[nowhere dense](../../../topological-analysis.md#nowhere-dense-set). This supplies the requested example under either convention, without conflating the two topologies.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For $n\geq1$, let $C_n=\{Z\in X:n\notin Z\}$. The presence or absence of $n$ is determined by a sufficiently long finite [initial segment](../../../set.md#initial-segment), so $C_n$ and its complement are [open sets](../../../topology.md#open-set) in the [ordinary topology on infinite subsets](../../../ramsey-theory.md#ordinary-topology-on-infinite-subsets). The [Ellentuck topology](../../../ramsey-theory.md#ellentuck-topology) is finer, hence each $C_n$ is star-[clopen](../../../topology.md#clopen-set) and in particular star-[closed](../../../topology.md#closed-set). Their union is

$$
\bigcup_{n\geq1}C_n=X\setminus\{\mathbb N\}.
$$

Every basic star-neighborhood $[s,A]$ of $\mathbb N$ has $s=\{1,\ldots,k\}$ for some $k\geq0$, and its reservoir $A$ contains every integer greater than $k$. Choosing $n>k$ gives $\mathbb N\setminus\{n\}\in[s,A]\cap C_n$. Thus $\mathbb N$ is in the star-[closure](../../../topology.md#closure-topology) of the union, but not in the union itself. Therefore

$$
\boxed{\bigcup_{n\geq1}C_n\text{ is not star-closed, although every }C_n\text{ is star-closed}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
