# Paper 12

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper12.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper12.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

We take $\mathbb N=\{1,2,\ldots\}$ and require the [common difference](../../../arithmetic.md#common-difference) of an [arithmetic progression](../../../arithmetic.md#arithmetic-progression) to be positive. An [ultrafilter](../../../set-theory.md#ultrafilter) $\mathcal U$ is a proper [filter on a set](../../../set-theory.md#filter-set-theory) deciding each [subset](../../../set.md#subset): exactly one of $B$ and $\mathbb N\setminus B$ belongs to $\mathcal U$.

For the fixed length $m$, let $\mathcal B_m$ be the family of sets containing no m-term [arithmetic progression](../../../arithmetic.md#arithmetic-progression). Any acceptable [ultrafilter](../../../set-theory.md#ultrafilter) must contain every complement $\mathbb N\setminus B$ with $B\in\mathcal B_m$. These mandatory sets have the [finite intersection property](../../../topology.md#finite-intersection-property). Otherwise finitely many $B_1,\ldots,B_r\in\mathcal B_m$ would cover $\mathbb N$. Colour an [integer](../../../number-theory.md#integer) by the first $i$ for which it belongs to $B_i$. The [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem) gives a [monochromatic](../../../ramsey-theory.md#monochromatic-set) m-term [arithmetic progression](../../../arithmetic.md#arithmetic-progression), contained in the corresponding $B_i$, a contradiction.

Generate a proper [filter](../../../set-theory.md#filter-set-theory) from those complements and extend it by the [ultrafilter lemma](../../../set-theory.md#ultrafilter-lemma). If some $B\in\mathcal U$ were in $\mathcal B_m$, its complement would also belong to $\mathcal U$, forcing the empty set into the [filter](../../../set-theory.md#filter-set-theory). Thus

$$
\boxed{\exists\mathcal U_m\quad\forall B\in\mathcal U_m,\ B\text{ contains an }m\text{-term arithmetic progression}.}
$$

Notice that sets avoiding one fixed length need not be closed under finite unions; the argument uses the [finite intersection property](../../../topology.md#finite-intersection-property), not an unsupported ideal claim.

For the unbounded-length version, let $\mathcal B$ consist of sets whose [arithmetic progression](../../../arithmetic.md#arithmetic-progression) lengths are bounded. Each $B_i\in\mathcal B$ fails to contain a progression of some length $m_i$, and hence of every greater length. If finitely many $B_i$ covered $\mathbb N$, colour by the first containing index and apply the [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem) at length $M=\max_i m_i$. Again a contradiction results. The complements of all members of $\mathcal B$ therefore have the [finite intersection property](../../../topology.md#finite-intersection-property). Extending their generated [filter](../../../set-theory.md#filter-set-theory) gives an [ultrafilter with arithmetic-progression-rich members](../../../set-theory.md#ultrafilter-with-arithmetic-progression-rich-members):

$$
\boxed{\exists\mathcal U\quad\forall B\in\mathcal U\quad\forall m\ge1,\ B\text{ contains an }m\text{-term arithmetic progression}.}
$$

All [finite sets](../../../set.md#finite-set) lie in $\mathcal B$, so this [ultrafilter](../../../set-theory.md#ultrafilter) contains every [cofinite set](../../../set-theory.md#cofinite-set) and is a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter). The same is true of the fixed-length construction when $m\ge2$, because no singleton is allowed; for $m=1$ a [principal ultrafilter](../../../set-theory.md#principal-ultrafilter) also works. These constructions illustrate [ultrafilter selection from a partition-rich family](../../../set-theory.md#ultrafilter-selection-from-a-partition-rich-family).

The infinite-length answer is **no**. Colour $n$ by $\lfloor\log_2n\rfloor\bmod2$, so successive intervals $[2^j,2^{j+1})$ alternate colours. An infinite [arithmetic progression](../../../arithmetic.md#arithmetic-progression) $a+td$, $t\ge0$, meets every sufficiently large such interval: its first term at least $2^j$ is less than $2^j+d$, which is at most $2^{j+1}$ once $2^j\ge d$. It therefore has terms of both colours. Neither colour class contains an infinite [arithmetic progression](../../../arithmetic.md#arithmetic-progression), but every [ultrafilter](../../../set-theory.md#ultrafilter) contains one of the two colour classes. This [dyadic block obstruction to infinite arithmetic progressions](../../../arithmetic.md#dyadic-block-obstruction-to-infinite-arithmetic-progressions) rules out the proposed [ultrafilter](../../../set-theory.md#ultrafilter).

## 2

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a finite alphabet $K$, a [combinatorial line](../../../ramsey-theory.md#combinatorial-line) in $K^N$ has a nonempty active set $J\subseteq\{1,\ldots,N\}$, fixed letters outside $J$, and the same variable letter at every coordinate in $J$. The [Hales-Jewett theorem](../../../ramsey-theory.md#hales-jewett-theorem) states that for every alphabet size $k\ge1$ and number of colours $r\ge1$, some $N$ makes every r-colouring of $\{1,\ldots,k\}^N$ contain a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [combinatorial line](../../../ramsey-theory.md#combinatorial-line).

We first prove the [alphabet insensitivity lemma](../../../ramsey-theory.md#alphabet-insensitivity-lemma) with a concrete bound. Fix two distinct letters $a,b$, a desired dimension $d$, and a colouring $\chi:K^N\to\{1,\ldots,r\}$. A [combinatorial subspace](../../../ramsey-theory.md#combinatorial-subspace) of dimension $d$ has disjoint nonempty active blocks $J_1,\ldots,J_d$ and fixed other coordinates. It is $(a,b)$-insensitive when exchanging $a,b$ in any one variable leaves the colour unchanged, whatever the other variable letters are.

Choose consecutive blocks of lengths $L_1,\ldots,L_d$ recursively by

$$
P_i=\sum_{j<i}L_j,\qquad L_i=r^{\,k^{P_i+d-i}},\qquad N=\sum_{i=1}^dL_i.
$$

Process these blocks from right to left. When block $i$ is reached, the later blocks already have one variable each; the earlier $P_i$ coordinates are still entirely unrestricted. For each of the $L_i+1$ words $a^t b^{L_i-t}$ in block $i$, form its complete [colour profile](../../../ramsey-theory.md#colour-profile-of-a-finite-block) over all $k^{P_i}$ earlier words and all $k^{d-i}$ assignments to the later variables. There are at most $r^{k^{P_i+d-i}}=L_i$ profiles. The [pigeonhole principle](../../../algebra.md#pigeonhole-principle) gives $s<t$ with equal profiles. Fix the first $s$ coordinates of this block to $a$, the coordinates after $t$ to $b$, and make the interval from $s+1$ to $t$ variable. Substitution of $b$ gives the chain word indexed by $s$, and substitution of $a$ gives the one indexed by $t$; they have identical profiles. Thus this variable is insensitive to $a,b$ for every remaining context. Previously constructed later variables remain insensitive, because their colour equalities held for every possible earlier word. After all $d$ blocks, we have the required insensitive [combinatorial subspace](../../../ramsey-theory.md#combinatorial-subspace). This proves the [explicit block bound for alphabet insensitivity](../../../ramsey-theory.md#explicit-block-bound-for-alphabet-insensitivity).

Now induct on $k$, simultaneously for every $r$. The case $k=1$ is immediate with $N=1$. For $k\ge2$, assume the [Hales-Jewett theorem](../../../ramsey-theory.md#hales-jewett-theorem) for the alphabet of size $k-1$, and take $d$ large enough for that theorem with $r$ colours. Apply the proved [alphabet insensitivity lemma](../../../ramsey-theory.md#alphabet-insensitivity-lemma) to the letters $k-1,k$, obtaining a d-dimensional [combinatorial subspace](../../../ramsey-theory.md#combinatorial-subspace) $\phi:K^d\to K^N$. On $\{1,\ldots,k-1\}^d$, the induced colouring $\chi\circ\phi$ has a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [combinatorial line](../../../ramsey-theory.md#combinatorial-line). Its value at letter $k$ has the same colour as its value at $k-1$: change the active variables one at a time and use insensitivity. The [union](../../../set.md#set-union) of their nonempty active blocks is the active set of a [combinatorial line](../../../ramsey-theory.md#combinatorial-line) in the original word space. All its k points have one colour, completing the induction and the proof.

To deduce the [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem), take $K=\{0,\ldots,m-1\}$ and pull a colouring of the [positive integers](../../../number-theory.md#positive-integer) back through

$$
\pi(w)=1+\sum_{j=1}^Nw_j.
$$

A [combinatorial line](../../../ramsey-theory.md#combinatorial-line) with active set $J$ maps to

$$
a,a+d,\ldots,a+(m-1)d,\qquad
 a=1+\sum_{j\notin J}w_j,\quad d=|J|>0.
$$

Hence **every [finite colouring](../../../ramsey-theory.md#finite-coloring) has a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [arithmetic progression](../../../arithmetic.md#arithmetic-progression) of every prescribed finite length**. In finite form, if $H(k,r)$ is a word-length bound for the [Hales-Jewett theorem](../../../ramsey-theory.md#hales-jewett-theorem), then $W(r,m)\le1+(m-1)H(m,r)$ is a valid interval bound.

The [Strengthened Van der Waerden theorem](../../../ramsey-theory.md#strengthened-van-der-waerden-theorem) also puts the [common difference](../../../arithmetic.md#common-difference) in the colour class:

$$
\boxed{\{d,a,a+d,\ldots,a+(m-1)d\}\text{ is monochromatic for some }a,d>0.}
$$

Here is a finite proof by induction on the number $r$ of colours. For $m=1$ choose $a=d=1$. For $r=1$ choose $a=d=1$ in $[m]$. For $m\ge2,r\ge2$, let $M$ be a bound for the strengthened theorem with $r-1$ colours, put $L=(m-1)M+1$, and let $W=W(r,L)$ be an ordinary [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem) bound. Work in $[MW]$. Its first $W$ points contain a [monochromatic](../../../ramsey-theory.md#monochromatic-set) progression

$$
a,a+d,\ldots,a+(L-1)d
$$

of colour $c$. Every $jd$, $1\le j\le M$, lies in $[MW]$. If some $jd$ has colour $c$, then $a,a+jd,\ldots,a+(m-1)jd$, together with its difference $jd$, gives the answer. Otherwise the colouring of $\{d,2d,\ldots,Md\}$ uses only $r-1$ colours. Pull it back to $[M]$ and apply the induction hypothesis to get a [monochromatic](../../../ramsey-theory.md#monochromatic-set) set $\{e,b,b+e,\ldots,b+(m-1)e\}$. Multiplication by $d$ gives the required configuration in the original colouring. This proves the strengthened theorem, including finite bounds.

The [Gallai theorem for an integer lattice](../../../ramsey-theory.md#gallai-theorem-for-an-integer-lattice) states that every [finite colouring](../../../ramsey-theory.md#finite-coloring) of $\mathbb Z^h$ contains a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [homothetic copy](../../../geometry-and-topology.md#homothetic-copy-of-a-finite-configuration) $u+tF$ of every prescribed finite nonempty pattern $F\subseteq\mathbb Z^h$, where $t$ is a [positive integer](../../../number-theory.md#positive-integer). The positive-lattice version holds for finite $F\subseteq\mathbb N^h$ as well. Write $F=\{v_1,\ldots,v_k\}$ and colour $w\in\{1,\ldots,k\}^N$ by the colour of

$$
\pi(w)=b+\sum_{j=1}^Nv_{w_j}.
$$

A [monochromatic](../../../ramsey-theory.md#monochromatic-set) [combinatorial line](../../../ramsey-theory.md#combinatorial-line) maps to $u+|J|F$, with $u=b+\sum_{j\notin J}v_{w_j}$. Thus the [Hales-Jewett theorem](../../../ramsey-theory.md#hales-jewett-theorem) supplies the copy, with nonzero dilation $|J|$. Choosing $b$ large and positive places all these word sums in the positive lattice if required. This [sum map from words to homothetic copies](../../../ramsey-theory.md#sum-map-from-words-to-homothetic-copies) also proves the real-vector-space version: replace $\mathbb Z^h$ by $\mathbb R^h$ and allow an arbitrary finite real pattern, while retaining [positive integer](../../../number-theory.md#positive-integer) dilations.

## 3

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For a [rational matrix](../../../vector-space.md#rational-matrix) $A$ with columns $a_1,\ldots,a_n$, [partition regularity](../../../ramsey-theory.md#partition-regular-matrix) means that every [finite colouring](../../../ramsey-theory.md#finite-coloring) of the [positive integers](../../../number-theory.md#positive-integer) admits a positive [monochromatic](../../../ramsey-theory.md#monochromatic-set) [vector](../../../vector-space.md#vector) $x$ with $Ax=0$. Repeated coordinates are allowed. The [columns condition](../../../ramsey-theory.md#columns-property) is an ordered partition $\{1,\ldots,n\}=B_1\sqcup\cdots\sqcup B_s$ into nonempty blocks such that

$$
\sum_{i\in B_1}a_i=0,\qquad
\sum_{i\in B_j}a_i\in\operatorname{span}_{\mathbb Q}\{a_i:i\in B_1\cup\cdots\cup B_{j-1}\}\quad(j\ge2).
$$

[Rado's theorem](../../../ramsey-theory.md#rado-s-theorem) says that **$A$ is partition regular if and only if it satisfies the [columns condition](../../../ramsey-theory.md#columns-property)**. We prove both directions.

For necessity, clear denominators so the columns are [integer](../../../number-theory.md#integer) [vectors](../../../vector-space.md#vector). For every pair of disjoint index sets $I,B$ with $B\ne\varnothing$ for which $\sum_{i\in B}a_i$ is not in the rational [linear span](../../../vector-space.md#linear-span) of the I-columns, choose an [integer](../../../number-theory.md#integer) [linear functional](../../../linear-algebra.md#linear-functional) $\ell_{I,B}$ that vanishes on those I-columns but not on that sum. Such a functional exists by finite-dimensional [linear algebra](../../../linear-algebra.md); clear its rational denominators. There are only finitely many pairs, so choose a [prime number](../../../number-theory.md#prime-number) $p$ dividing none of the nonzero [integers](../../../number-theory.md#integer)

$$
\ell_{I,B}\left(\sum_{i\in B}a_i\right).
$$

If there are no offending pairs, any [prime number](../../../number-theory.md#prime-number) suffices.

Colour a [positive integer](../../../number-theory.md#positive-integer) $x=p^{v_p(x)}u$, $p\nmid u$, by $u\bmod p$. This is the [last nonzero digit coloring](../../../ramsey-theory.md#last-nonzero-digit-coloring), using $p-1$ colours. [Partition regularity](../../../ramsey-theory.md#partition-regular-matrix) gives a positive [monochromatic](../../../ramsey-theory.md#monochromatic-set) solution. Group its coordinate indices by their distinct [P-adic valuations](../../../number-theory.md#p-adic-valuation) $e_1<\cdots<e_s$, writing $B_j=\{i:v_p(x_i)=e_j\}$. All units $x_i/p^{e_j}$ have the same nonzero residue $\alpha$ modulo $p$.

For each $j$, let $I=B_1\cup\cdots\cup B_{j-1}$. If its block sum failed the required span condition, apply the chosen $\ell_{I,B_j}$ to $\sum_i a_ix_i=0$. The earlier terms vanish exactly, not just modulo a power of $p$. Divide by $p^{e_j}$; terms with later valuations are still divisible by $p$. Reduction modulo $p$ then yields

$$
0=\alpha\,\ell_{I,B_j}\left(\sum_{i\in B_j}a_i\right)\pmod p,
$$

contrary to the choice of $p$. Thus every required span relation holds, and with $I=\varnothing$ the first block sum is zero. This is the [finite separating-functional proof of the columns condition](../../../ramsey-theory.md#finite-separating-functional-proof-of-the-columns-condition); it avoids an unjustified passage from congruences to rational equality.

For sufficiency, assume the [columns condition](../../../ramsey-theory.md#columns-property). Choose rational coefficients $\lambda_{ij}$, for $j\ge2$ and $i\in B_1\cup\cdots\cup B_{j-1}$, such that

$$
\sum_{i\in B_j}a_i+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\lambda_{ij}a_i=0.
$$

Choose a [positive integer](../../../number-theory.md#positive-integer) $c$ clearing every denominator, and a [positive integer](../../../number-theory.md#positive-integer) $p\ge\max|c\lambda_{ij}|$, taking $p=1$ if the list is empty. By the allowed [monochromatic m-p-c set theorem](../../../ramsey-theory.md#monochromatic-m-p-c-set-theorem), there are positive generators $z_1,\ldots,z_s$ such that all numbers

$$
cz_h+\sum_{j>h}\mu_jz_j,\qquad \mu_j\in\mathbb Z,\quad |\mu_j|\le p,
$$

are positive and have one colour. This is a full [m-p-c set](../../../ramsey-theory.md#m-p-c-set); positivity is part of its definition, not a rule discarding negative expressions. For $i\in B_h$, put

$$
x_i=cz_h+\sum_{j>h}c\lambda_{ij}z_j.
$$

These coordinates all belong to that [monochromatic](../../../ramsey-theory.md#monochromatic-set) [m-p-c set](../../../ramsey-theory.md#m-p-c-set). Collecting coefficients of $z_j$ gives

$$
\sum_i a_ix_i
=c z_1\sum_{i\in B_1}a_i+
\sum_{j=2}^s c z_j\left(\sum_{i\in B_j}a_i+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\lambda_{ij}a_i\right)=0.
$$

Thus the [Rado solution inside an m-p-c set](../../../ramsey-theory.md#rado-solution-inside-an-m-p-c-set) proves [partition regularity](../../../ramsey-theory.md#partition-regular-matrix) and completes the theorem.

To obtain the [Finite sums theorem](../../../ramsey-theory.md#finite-sums-theorem) from [Rado's theorem](../../../ramsey-theory.md#rado-s-theorem), introduce a positive variable $y_F$ for every nonempty $F\subseteq\{1,\ldots,k\}$ and impose

$$
y_F-\sum_{i\in F}y_{\{i\}}=0\qquad(|F|\ge2).
$$

Partition the columns of this system into $B_j=\{F:\min F=j\}$. The $B_1$-column sum is zero: in a row indexed by $F$ containing $1$, the contributions of $y_F$ and $y_{\{1\}}$ cancel, and other rows receive neither. For $j>1$, the $B_j$-column sum is

$$
-\sum_{\substack{F:\min F<j\\j\in F}}a_F,
$$

where $a_F$ is the column of $y_F$. Those columns lie in earlier blocks. Hence the [columns condition](../../../ramsey-theory.md#columns-property) holds. A [monochromatic](../../../ramsey-theory.md#monochromatic-set) positive solution gives $x_i=y_{\{i\}}$ and $y_F=\sum_{i\in F}x_i$, proving

$$
\boxed{\operatorname{FS}(x_1,\ldots,x_k)\text{ is monochromatic}.}
$$

For $k=1$ the system has no rows and the conclusion is immediate. The construction is also visible directly in the sufficiency proof: a [monochromatic](../../../ramsey-theory.md#monochromatic-set) $(k,1,1)$-set contains every nonempty sum of its generators, classified by the smallest chosen index.

## 4

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write $[\mathbb N]^\omega$ for the [space of infinite subsets of the natural numbers](../../../ramsey-theory.md#space-of-infinite-subsets-of-the-natural-numbers), with each [subset](../../../set.md#subset) identified with its increasing enumeration. In the homogeneous-cone convention, a family $\mathcal A\subseteq[\mathbb N]^\omega$ is a [Ramsey family in the homogeneous-cone sense](../../../ramsey-theory.md#ramsey-family-in-the-homogeneous-cone-sense) when some infinite $M$ satisfies

$$
[M]^\omega\subseteq\mathcal A\quad\text{or}\quad[M]^\omega\cap\mathcal A=\varnothing.
$$

The stronger [Ramsey set of infinite subsets](../../../ramsey-theory.md#ramsey-set-of-infinite-subsets) convention asks for such an infinite $M\subseteq A$ inside every given infinite ground set $A$. We will prove the open-set assertion in this stronger form, and our Ramsey-but-not-completely-Ramsey example will satisfy it as well. Thus the distinction in conventions does not affect any of the conclusions below.

For a non-Ramsey example, declare $X\sim Y$ if their [symmetric difference](../../../set.md#symmetric-difference) is finite, and choose a representative $R$ from each [equivalence class](../../../set-theory.md#equivalence-class) using the [axiom of choice](../../../set-theory.md#axiom-of-choice). Set

$$
\varepsilon(X)=|X\triangle R|\pmod2
$$

for the representative of the class of $X$. Removing one point reverses this colour, because its [symmetric difference](../../../set.md#symmetric-difference) with $R$ changes by exactly one point. Consequently every cone $[M]^\omega$ contains the oppositely coloured sets $M$ and $M\setminus\{\min M\}$. Either colour class of this [finite-symmetric-difference parity colouring](../../../ramsey-theory.md#finite-symmetric-difference-parity-colouring) is not a [Ramsey family in the homogeneous-cone sense](../../../ramsey-theory.md#ramsey-family-in-the-homogeneous-cone-sense). No definability is claimed for the representative selection.

The [ordinary topology on infinite subsets](../../../ramsey-theory.md#ordinary-topology-on-infinite-subsets), denoted $\tau$, has basic cylinders $[s]=\{X:s\sqsubset X\}$, where $s$ is a [finite stem](../../../ramsey-theory.md#finite-stem-of-an-infinite-subset) of the increasing enumeration. Let $O$ be a $\tau$-open family and fix an arbitrary infinite ground set $A$. We give a complete fusion proof of a homogeneous cone inside $A$.

Use the convention $\max\varnothing=0$. For finite $s$ and an infinite reservoir $B$ above $\max s$, say that $B$ accepts $s$ if $[s,B]\subseteq O$, where

$$
[s,B]=\{s\cup X:X\in[B]^\omega\}.
$$

Say that $B$ rejects $s$ if no infinite [subset](../../../set.md#subset) of $B$ accepts $s$. There is always a refinement deciding $s$: choose an accepting subreservoir if one exists, and otherwise retain $B$, which rejects. Both decisions persist under further thinning.

A first fusion produces an infinite $H\subseteq A$ deciding every finite $s\subseteq H$ on its tail $H/s=\{h\in H:h>\max s\}$. First decide the empty stem. Choose the first point, and thin the remaining reservoir successively to decide every [subset](../../../set.md#subset) of the selected prefix. Repeat after choosing each new point. There are finitely many [subsets](../../../set.md#subset) to decide at each stage. The diagonal sequence of chosen points has the required property, since its tail after the largest point of any stem lies in the reservoir where that stem was decided. The empty-stem decision persists too. This is [deciding all finite stems by fusion](../../../ramsey-theory.md#deciding-all-finite-stems-by-fusion).

If $H$ accepts the empty stem, $[H]^\omega\subseteq O$ and we are done. Suppose it rejects. For a rejected finite $s\subseteq H$, only finitely many $h\in H/s$ can have $H/h$ accepting $s\cup\{h\}$. Otherwise let $D$ be their [infinite set](../../../set.md#infinite-set). Every infinite $X\subseteq D$ starts with some such $h$, and its remaining tail lies in $H/h$, so $s\cup X\in O$. Then $D$ accepts $s$, contradicting rejection. This proves [finitely many accepting extensions of a rejected stem](../../../ramsey-theory.md#finitely-many-accepting-extensions-of-a-rejected-stem).

A second fusion constructs $K\subseteq H$ whose every finite [subset](../../../set.md#subset) is rejected. If a finite prefix of chosen points has been selected, all its [subsets](../../../set.md#subset) are rejected by induction. Avoid the [union](../../../set.md#set-union) of their finitely many accepting successor sets when choosing the next point. The first fusion already decides every successor, so every new [subset](../../../set.md#subset) is rejected. An infinite reservoir remains after each finite exclusion.

If some $X\in[K]^\omega$ belonged to $O$, openness would give an [initial segment](../../../set.md#initial-segment) $s\sqsubset X$ with $[s]\subseteq O$. Its reservoir $H/s$ would then accept $s$, contradicting the second fusion. Therefore $[K]^\omega\cap O=\varnothing$. In either case we have a homogeneous cone inside the arbitrary ground set $A$. **Every $\tau$-open family is a [Ramsey set of infinite subsets](../../../ramsey-theory.md#ramsey-set-of-infinite-subsets)**, under both conventions.

A [completely Ramsey set](../../../ramsey-theory.md#completely-ramsey-set) requires more: for every finite $s$ and infinite reservoir $A$ above $\max s$, there is an infinite $B\subseteq A$ such that

$$
[s,B]\subseteq\mathcal A\quad\text{or}\quad[s,B]\cap\mathcal A=\varnothing.
$$

The [finite stem](../../../ramsey-theory.md#finite-stem-of-an-infinite-subset) must be kept fixed. These $[s,A]$ are the basic [neighbourhoods](../../../topology.md#neighbourhood-mathematics) of the [Ellentuck topology](../../../ramsey-theory.md#ellentuck-topology), also called the [star topology](../../../ramsey-theory.md#ellentuck-topology).

Let $E$ be the even [positive integers](../../../number-theory.md#positive-integer), and construct the [finite-symmetric-difference parity colouring](../../../ramsey-theory.md#finite-symmetric-difference-parity-colouring) $\varepsilon$ on $[E]^\omega$. Define

$$
\mathcal R=\{\{1\}\cup X:X\in[E]^\omega,\ \varepsilon(X)=0\}.
$$

For any infinite ground set $A$, the set $A\setminus\{1\}$ is still infinite and its whole cone misses $\mathcal R$. Thus $\mathcal R$ is a [Ramsey set of infinite subsets](../../../ramsey-theory.md#ramsey-set-of-infinite-subsets) even in the stronger convention. But inside $[\{1\},E]$, every infinite refinement $B\subseteq E$ gives the two sets $\{1\}\cup B$ and $\{1\}\cup(B\setminus\{\min B\})$ of opposite colours. Hence no such refinement is homogeneous. **The family $\mathcal R$ is Ramsey but not [completely Ramsey](../../../ramsey-theory.md#completely-ramsey-set).** The [stem-supported Ramsey family need not be completely Ramsey](../../../ramsey-theory.md#stem-supported-ramsey-family-need-not-be-completely-ramsey) construction explains this example: forgetting the stem $\{1\}$ is precisely what loses the obstruction.

Finally take $D=[E]^\omega$. It is nonempty and star-open, since it equals $[\varnothing,E]$. It is $\tau$-closed: if an [infinite set](../../../set.md#infinite-set) contains an odd [integer](../../../number-theory.md#integer), an [initial segment](../../../set.md#initial-segment) witnessing that [integer](../../../number-theory.md#integer) has a cylinder disjoint from $D$. Its $\tau$-interior is empty: after any [finite stem](../../../ramsey-theory.md#finite-stem-of-an-infinite-subset) of even [integers](../../../number-theory.md#integer), append an arbitrarily large odd [integer](../../../number-theory.md#integer) and then infinitely many further points. Thus

$$
\boxed{D\text{ is nonempty and star-open, but }\tau\text{-nowhere dense}.}
$$

This is the [cone on an infinite coinfinite ground set](../../../ramsey-theory.md#cone-on-an-infinite-coinfinite-ground-set). Choose its [subset](../../../set.md#subset) $Y=\{X\in[E]^\omega:\varepsilon(X)=0\}$. Since $\overline Y^{\,\tau}\subseteq D$, $Y$ is also $\tau$-nowhere dense. Nevertheless every $[\varnothing,B]$ with infinite $B\subseteq E$ contains both $B$ and $B\setminus\{\min B\}$, of opposite colours. Hence $Y$ is not [completely Ramsey](../../../ramsey-theory.md#completely-ramsey-set). We have proved explicitly that [ordinarily nowhere-dense sets need not be completely Ramsey](../../../ramsey-theory.md#ordinarily-nowhere-dense-sets-need-not-be-completely-ramsey); the [topology](../../../topology.md) in the nowhere-dense hypothesis cannot be silently changed to the [star topology](../../../ramsey-theory.md#ellentuck-topology).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
