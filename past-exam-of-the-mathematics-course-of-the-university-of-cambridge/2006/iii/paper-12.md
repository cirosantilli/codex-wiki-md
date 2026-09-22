# Paper 12

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper12.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper12.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
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

## 1

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For $1\le r\le n$ and a rank-$r$ [uniform set family](../../../extremal-set-theory.md#uniform-set-family) $\mathcal F$, let $\partial\mathcal F$ be its [lower shadow](../../../extremal-set-theory.md#lower-shadow). Count pairs $(B,A)$ with $A\in\mathcal F$, $B\subset A$ and $|B|=r-1$. Every $A$ contributes $r$ pairs, whereas each shadow member lies in at most $n-r+1$ rank-$r$ sets. Thus

$$
r|\mathcal F|\le(n-r+1)|\partial\mathcal F|,
\qquad
\boxed{\frac{|\partial\mathcal F|}{\binom n{r-1}}\ge
\frac{|\mathcal F|}{\binom nr}.}
$$

This is the [Local LYM inequality](../../../extremal-set-theory.md#local-lym-inequality). Complementation gives the upper-shadow form $|\nabla\mathcal F|/\binom n{r+1}\ge|\mathcal F|/\binom nr$ for $r<n$.

To deduce the [LYM inequality](../../../extremal-set-theory.md#lubell-yamamoto-meshalkin-inequality), let $\mathcal A$ be an [antichain](../../../extremal-set-theory.md#antichain), $\mathcal A_r$ its rank-$r$ part, and $U_r$ all rank-$r$ sets containing some member of $\mathcal A$. For $r\ge1$,

$$
U_r=\nabla U_{r-1}\ \dot\cup\ \mathcal A_r.
$$

The union is disjoint because an [antichain](../../../extremal-set-theory.md#antichain) member cannot contain a smaller member; every other set of $U_r$ contains a rank-$(r-1)$ superset of its smaller witnessing member. Apply the upper local inequality and put $u_r=|U_r|/\binom nr$:

$$
u_r\ge u_{r-1}+\frac{|\mathcal A_r|}{\binom nr}.
$$

Since $u_0=|\mathcal A_0|$ and $u_n\le1$, summing gives

$$
\boxed{\sum_{r=0}^n\frac{|\mathcal A_r|}{\binom nr}\le1.}
$$

Thus the deduction uses the local inequality explicitly, rather than quoting a separate maximal-chain argument.

Let $M=\binom n{\lfloor n/2\rfloor}$, the largest rank size. The LYM sum is at least $|\mathcal A|/M$, proving the [Sperner theorem](../../../extremal-set-theory.md#sperner-s-theorem) bound. If $|\mathcal A|=M$, equality forces all its members onto ranks with [binomial coefficient](../../../combinatorics.md#binomial-coefficient) $M$. For even $n$, there is only the middle rank, so the family is that whole rank.

For $n=2m+1$, only ranks $m,m+1$ are possible, each of size $M$. Let $\mathcal B=\mathcal A_{m+1}$. Antichainness gives $\mathcal A_m\cap\partial\mathcal B=\varnothing$, and local LYM gives $|\partial\mathcal B|\ge|\mathcal B|$. Since the two [antichain](../../../extremal-set-theory.md#antichain) parts together have size $M$, equality must hold. The inclusion [graph](../../../graph.md) between these ranks is $(m+1)$-regular on each side. Its [edges](../../../graph-theory.md#edge-of-a-graph) from $\mathcal B$ already number $(m+1)|\mathcal B|$, so equality leaves no edge from $\partial\mathcal B$ to the complementary upper [vertices](../../../graph.md#vertex-graph-theory).

The [graph](../../../graph.md) is connected: exchanging one element between two $m$-sets joins them through their $(m+1)$-element union, and successive exchanges connect all lower [vertices](../../../graph.md#vertex-graph-theory); every upper vertex has a lower neighbour. Consequently $\mathcal B$ is either empty or the entire upper rank. This [connectedness of adjacent-level incidence in a Boolean lattice](../../../extremal-set-theory.md#connectedness-of-adjacent-level-incidence-in-a-boolean-lattice) excludes mixed extremizers. Hence

$$
\boxed{\text{the maximum antichains are exactly the full middle levels}.}
$$

There is one choice for even $n$ and two for odd $n$. For $n=0$, the sole maximum family is $\{\varnothing\}$, agreeing with this description.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Proceed by induction on the ground-set size, starting with the one-element chain $\{\varnothing\}$ in the [Boolean lattice](../../../extremal-set-theory.md#boolean-lattice) on no coordinates. Suppose a [symmetric chain decomposition of a Boolean lattice](../../../extremal-set-theory.md#symmetric-chain-decomposition-of-a-boolean-lattice) on $[n]$ has been constructed. Write one of its chains as

$$
S_r\subset S_{r+1}\subset\cdots\subset S_{n-r},\qquad |S_j|=j.
$$

On adjoining the new coordinate $v=n+1$, replace its two copies by

$$
S_r\subset\cdots\subset S_{n-r}\subset S_{n-r}\cup\{v\}
$$

and, when nonempty,

$$
S_r\cup\{v\}\subset S_{r+1}\cup\{v\}\subset\cdots\subset S_{n-r-1}\cup\{v\}.
$$

The first chain has endpoint ranks $r,n-r+1$, summing to $n+1$. The second has endpoint ranks $r+1,n-r$, also summing to $n+1$. Both are saturated chains, increasing rank by one at every step. If the original chain was a singleton, the second chain is omitted.

These new chains are disjoint: the first contains every old set without $v$ and just the last old set with $v$; the second contains precisely the remaining old sets with $v$. Thus together they cover both lifted copies of the old chain. Different old chains have disjoint copies, so performing this construction for each yields a partition of all subsets of $[n+1]$ into [symmetric chains](../../../extremal-set-theory.md#symmetric-chain-in-a-boolean-lattice). This completes the induction and proves **a [symmetric chain](../../../extremal-set-theory.md#symmetric-chain-in-a-boolean-lattice) partition exists for every $n$**.

## 2

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Identify the [hypercube graph](../../../graph.md#hypercube-graph) $Q_n$ with subsets of $[n]$, adjacent when they differ by one element. Write $N(\mathcal F)$ for a family's closed [vertex neighbourhood](../../../graph.md#vertex-neighbourhood). The [simplicial order on the discrete cube](../../../combinatorics.md#simplicial-order-on-the-discrete-cube) orders first by size and then, within a rank, by [lexicographic order](../../../extremal-set-theory.md#lexicographic-order): the least element of a [symmetric difference](../../../set.md#symmetric-difference) belongs to the earlier set. The [Harper theorem](../../../combinatorics.md#vertex-isoperimetric-inequality-in-the-discrete-cube) says that if $I$ is the initial simplicial segment with $|I|=|\mathcal F|$, then

$$
\boxed{|N(\mathcal F)|\ge|N(I)|.}
$$

Equivalently this minimizes the [external vertex boundary](../../../graph-theory.md#external-vertex-boundary) at fixed [cardinality](../../../set-theory.md#cardinality). This is the vertex-isoperimetric assertion, distinct from the edge version in Question 3.

Here is the deduction of [Kruskal-Katona theorem](../../../extremal-set-theory.md#kruskal-katona-theorem). For a family $\mathcal B\subseteq[n]^{(k)}$, adjoin every lower rank and set $\mathcal D=[n]^{(<k)}\cup\mathcal B$. For $k\ge1$,

$$
N(\mathcal D)=[n]^{(\le k)}\cup\nabla\mathcal B.
$$

The corresponding simplicial [initial segment](../../../set.md#initial-segment) is $[n]^{(<k)}\cup L$, where $L$ is the rank-$k$ lexicographic [initial segment](../../../set.md#initial-segment) of size $|\mathcal B|$. Canceling the common lower-rank count in Harper's inequality gives $|\nabla\mathcal B|\ge|\nabla L|$. The rank-zero case is immediate by considering its two possible families.

To turn upper shadows into lower shadows, let $\rho(i)=n+1-i$ and $T(B)=\rho([n]\setminus B)$. This bijection reverses inclusion and changes rank $k$ to $n-k$. If $B$ precedes $C$ in lex order, the largest element of $T(B)\triangle T(C)$ belongs to $T(C)$, so $T(B)$ precedes $T(C)$ in [colexicographic order](../../../extremal-set-theory.md#colexicographic-order). Also $T(\nabla\mathcal B)=\partial(T\mathcal B)$. Hence applying the upper-shadow conclusion to the transformed family proves

$$
\boxed{|\partial\mathcal A|\ge|\partial C|,}
$$

where $C$ is the colex [initial segment](../../../set.md#initial-segment) of the same size and rank as $\mathcal A$. This is the Kruskal-Katona lower-shadow theorem. A colex segment's shadow is itself a colex segment: split its sets by their largest element, giving a full initial block of the preceding ground set followed by an initial block with the new largest element. The same description holds one rank lower. Iteration therefore shows that colex segments minimize shadows at every lower rank. This proves the [Harper theorem implies the Kruskal-Katona theorem](../../../combinatorics.md#harper-theorem-implies-the-kruskal-katona-theorem) deduction, including the necessary complement and coordinate reversal.

The [Erdős-Ko-Rado theorem](../../../extremal-set-theory.md#erdos-ko-rado-theorem) states that for $1\le r\le n/2$, every [intersecting family](../../../extremal-set-theory.md#intersecting-family) $\mathcal A\subseteq[n]^{(r)}$ satisfies

$$
\boxed{|\mathcal A|\le\binom{n-1}{r-1}.}
$$

The family of all $r$-sets containing a fixed point attains the bound. We use the standard convention of positive ranks here.

For the first proof, let $\mathcal B$ be the complements of members of $\mathcal A$, at rank $k=n-r\ge r$, and let $\mathcal S$ be its rank-$r$ [lower shadow](../../../extremal-set-theory.md#lower-shadow). It is disjoint from $\mathcal A$, since $A\subseteq[n]\setminus A'$ would make two family members disjoint. Suppose $|\mathcal A|>\binom{n-1}{r-1}=\binom{n-1}k$. The colex rank-$k$ segment of that size contains every $k$-set on $[n-1]$ and at least one set containing $n$. Its rank-$r$ shadow therefore contains all $\binom{n-1}r$ old $r$-sets and at least one new $r$-set containing $n$. The iterated Kruskal-Katona bound gives

$$
|\mathcal S|>\binom{n-1}r.
$$

Then $|\mathcal A|+|\mathcal S|>\binom{n-1}{r-1}+\binom{n-1}r=\binom nr$, impossible for disjoint subfamilies of rank $r$. This proves the [Erdős-Ko-Rado theorem from shadows](../../../extremal-set-theory.md#erdos-ko-rado-theorem-from-shadows).

For the second proof use the [Katona circle method](../../../extremal-set-theory.md#katona-circle-method). In any [cyclic ordering](../../../combinatorics.md#cyclic-ordering) of the $n$ points, an intersecting collection of length-$r$ intervals has at most $r$ members. To prove this, rotate one selected interval to end at position $n$, so it occupies $n-r+1,\ldots,n$. Intervals ending at $r,\ldots,n-r$ miss it and cannot be selected. Among the remaining endpoints other than $n$, pair $j$ with $j+n-r$ for $1\le j\le r-1$. The two intervals in each pair are disjoint because $n\ge2r$, so at most one can be selected. Including the fixed interval gives at most $1+(r-1)=r$.

Now count pairs consisting of a family member and a [permutation](../../../combinatorics.md#permutation) in which it is a cyclic interval. A fixed $r$-set has $nr!(n-r)!$ such [permutations](../../../combinatorics.md#permutation): choose its final position, its internal order, and the order of the remaining points. Each of the $n!$ [permutations](../../../combinatorics.md#permutation) contributes at most $r$ family intervals by the proved [cyclic interval intersection bound](../../../extremal-set-theory.md#cyclic-interval-intersection-bound). Thus

$$
|\mathcal A|nr!(n-r)!\le rn!,\qquad
|\mathcal A|\le\frac rn\binom nr=\binom{n-1}{r-1}.
$$

This is the required cyclic-ordering proof, with its interval lemma established explicitly.

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

**Always true**, for the ordinary positive-rank intersecting-family convention. The [Erdős-Ko-Rado theorem](../../../extremal-set-theory.md#erdos-ko-rado-theorem) bounds the family's size by $\binom{n-1}{r-1}$. In [lexicographic order](../../../extremal-set-theory.md#lexicographic-order), the first exactly that many rank-$r$ sets are all those containing one. Therefore the [initial segment](../../../set.md#initial-segment) of the given size is contained in that star and any two members intersect at one. This proves that [lexicographic initial segments preserve ordinary intersection](../../../extremal-set-theory.md#lexicographic-initial-segments-preserve-ordinary-intersection). Empty families cause no exception. If rank zero is admitted, its layer has just one set and replacement by either [initial segment](../../../set.md#initial-segment) changes nothing, so all three preservation assertions at that rank hold trivially.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

**False in general.** On $[5]$ take the rank-two star

$$
\mathcal A=\{12,13,14,15\}.
$$

It is an [intersecting family](../../../extremal-set-theory.md#intersecting-family) of four sets and $r=2\le5/2$. The first four rank-two sets in [colexicographic order](../../../extremal-set-theory.md#colexicographic-order) are

$$
\{12,13,23,14\}.
$$

The members $23$ and $14$ are disjoint. Thus [colexicographic replacement can destroy intersection](../../../extremal-set-theory.md#colexicographic-replacement-can-destroy-intersection), despite its shadow-minimizing property.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

**False in general.** Take $n=8$, $r=4$, and

$$
\mathcal A=\{A\subseteq[8]:|A|=4,\ |A\cap[4]|\ge3\}.
$$

It is a [Frankl family](../../../extremal-set-theory.md#complete-intersection-candidate-family) with $\binom43\binom41+\binom44=17$ members. Two members each use at least three of the first four points, so they share at least two of those points. Hence it is [t-intersecting](../../../extremal-set-theory.md#t-intersecting-family) with $t=2$, and $r=n/2$.

The first fifteen rank-four sets in [lexicographic order](../../../extremal-set-theory.md#lexicographic-order) are precisely those containing $1,2$. The sixteenth is $1345$, which intersects the earlier set $1278$ only at one. Therefore the lex [initial segment](../../../set.md#initial-segment) of size seventeen is not two-intersecting. This proves that [lexicographic replacement can destroy two-intersection](../../../extremal-set-theory.md#lexicographic-replacement-can-destroy-two-intersection); an ordinary intersecting bound cannot justify preservation of higher-order intersection.

## 3

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Use binary encoding $b(S)=\sum_{i\in S}2^{i-1}$ for [vertices](../../../graph.md#vertex-graph-theory) of the [hypercube graph](../../../graph.md#hypercube-graph), and write $I_m=\{S:b(S)<m\}$. Let $e(\mathcal A)$ count [edges](../../../graph-theory.md#edge-of-a-graph) with both endpoints in a family. The exact [edge-isoperimetric theorem for binary initial segments](../../../combinatorics.md#edge-isoperimetric-theorem-for-binary-initial-segments), due to Harper, Lindsey, Bernstein and Hart, is

$$
\boxed{e(\mathcal A)\le e(I_m)=\sum_{j=0}^{m-1}s_2(j),\qquad m=|\mathcal A|,}
$$

where $s_2(j)$ is the number of ones in the binary expansion. Equivalently,

$$
\boxed{|\partial_e\mathcal A|\ge nm-2\sum_{j=0}^{m-1}s_2(j).}
$$

The equality for $I_m$ follows by assigning each internal edge to its larger endpoint: each one-bit of that endpoint can be cleared, giving an earlier endpoint still in $I_m$. This is the exact extremal statement, stronger than the logarithmic entropy bound.

We prove it by induction on $n$. The case $n=1$ follows by checking sizes zero, one and two. Fix a coordinate $i$ and delete it from the two sections $\mathcal A_0,\mathcal A_1$. The edge count splits as

$$
e(\mathcal A)=e(\mathcal A_0)+e(\mathcal A_1)+|\mathcal A_0\cap\mathcal A_1|.
$$

Replace each section by a [binary initial segment](../../../combinatorics.md#binary-initial-segment) of the same size. By induction its internal [edges](../../../graph-theory.md#edge-of-a-graph) cannot decrease. The two replacement segments are nested, so their intersection size is the smaller section size, at least the previous intersection size. Thus this [section compression in binary order](../../../combinatorics.md#section-compression-in-binary-order) cannot decrease $e(\mathcal A)$.

Repeatedly perform any nontrivial section compression. The sum $\sum_{S\in\mathcal A}b(S)$ strictly decreases each time: in a fixed section, the original numerical order is exactly the numerical order after deleting its fixed coordinate. This nonnegative integer potential ensures termination at a family compressed in every coordinate section.

Classify such a terminal family. If an absent vertex $S$ precedes a present vertex $T$, they cannot agree in any coordinate, because their common section is compressed and its earlier vertex would then have to be present. Hence $T=[n]\setminus S$. There can be no vertex strictly between them: if present, it would also have to be the complement of $S$; if absent, it would have to be the complement of $T$. Thus they are consecutive complementary binary integers, forcing

$$
b(S)=2^{n-1}-1,\qquad b(T)=2^{n-1}.
$$

No other inversion is possible for the same reason. Therefore a terminal family is either a [binary initial segment](../../../combinatorics.md#binary-initial-segment) or the sole exceptional form

$$
\bigl(\mathcal P([n-1])\setminus\{[n-1]\}\bigr)\cup\{\{n\}\}.
$$

This exception has size $2^{n-1}$. For $n\ge2$, compared with the half-cube $I_{2^{n-1}}$, it removes a vertex of internal degree $n-1$ and adds a vertex joined only to the retained empty set. Its edge count is thus $e(I_{2^{n-1}})-(n-1)+1\le e(I_{2^{n-1}})$. The $n=1$ case was already handled. Since compression never decreased [edges](../../../graph-theory.md#edge-of-a-graph), every original family has at most the [initial segment](../../../set.md#initial-segment)'s edge count. This proves the theorem, including the exceptional terminal configuration rather than assuming all compressed families are [initial segments](../../../set.md#initial-segment).

For the remaining requests it is useful to obtain the [entropy proof of cube edge-isoperimetry](../../../combinatorics.md#entropy-proof-of-cube-edge-isoperimetry), including its equality cases. Inductively a family of size $m$ satisfies

$$
e(\mathcal A)\le\tfrac12m\log_2m.
$$

Indeed let the two sections have sizes $a\ge b\ge0$, $m=a+b>0$. Their internal [edges](../../../graph-theory.md#edge-of-a-graph) are bounded inductively and the crossing [edges](../../../graph-theory.md#edge-of-a-graph) are at most $b$, so

$$
\begin{aligned}
e(\mathcal A)&\le\tfrac12(a\log_2a+b\log_2b)+b\\
&=\tfrac12m\log_2m-\tfrac12mH_2(t)+mt,
\qquad t=b/m.
\end{aligned}
$$

Here $0\log_20=0$ and $H_2(t)=-t\log_2t-(1-t)\log_2(1-t)$ is the [binary entropy function](../../../combinatorics.md#binary-entropy-function). Its concavity and its endpoint values at zero and one-half give $H_2(t)\ge2t$ for $0\le t\le1/2$. This proves the bound, starting from the zero-dimensional cube.

Define the [isoperimetric number of a graph](../../../combinatorics.md#isoperimetric-number-of-a-graph) by

$$
i(G)=\min_{0<|A|\le|V(G)|/2}\frac{|\partial_eA|}{|A|}.
$$

Since every cube vertex has degree $n$, the internal-edge bound gives

$$
|\partial_eA|=n|A|-2e(A)\ge |A|\log_2\frac{2^n}{|A|}\ge|A|
$$

when $|A|\le2^{n-1}$. A coordinate half-cube has one crossing edge per vertex, attaining ratio one. Hence, for $n\ge1$,

$$
\boxed{i(Q_n)=1.}
$$

Now establish the [equality cases of entropy cube edge-isoperimetry](../../../combinatorics.md#equality-cases-of-entropy-cube-edge-isoperimetry). Strict concavity of $H_2$ makes $H_2(t)>2t$ for $0<t<1/2$. Equality in the internal-edge bound therefore requires either one section to be empty, or two equal-size sections. In the equal-size case equality in the crossing bound forces the sections to coincide; each section must also attain its inductive internal-edge bound. Induction gives exactly [coordinate subcubes](../../../combinatorics.md#face-of-the-boolean-hypercube): the empty-section case fixes the coordinate, and the coincident-section case frees it. Conversely every [coordinate subcube](../../../combinatorics.md#face-of-the-boolean-hypercube) attains that bound.

At size $m=2^{n-1}$, an [edge boundary](../../../combinatorics.md#edge-boundary-in-a-graph) of size $m$ means $e(A)=\tfrac12m(n-1)=\tfrac12m\log_2m$, so these equality cases apply. The subcube has dimension $n-1$ and fixes precisely one coordinate. Therefore

$$
\boxed{A=\{x\in\{0,1\}^n:x_i=\epsilon\},\quad i\in[n],\ \epsilon\in\{0,1\}.}
$$

These **$2n$ coordinate half-cubes are the only extremizers** of the requested size.

## 4

↑ **Parent:** [Paper 12](paper-12.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The uniform modular [Frankl-Wilson theorem](../../../extremal-set-theory.md#frankl-wilson-theorem) states the following. Let $p$ be prime, let $L\subseteq\mathbb F_p$ have size $s$, and let $\mathcal F$ be a rank-$k$ family on $[N]$, with $0\le s\le\min\{k,N-k\}$. Assume $k\bmod p\notin L$ and $|A\cap B|\bmod p\in L$ for every distinct $A,B\in\mathcal F$. Then

$$
\boxed{|\mathcal F|\le\binom Ns.}
$$

The restrictions concern distinct pairs; the diagonal size residue is explicitly excluded from $L$.

For each member $A$, over $\mathbb F_p$ form the [intersection polynomial](../../../combinatorics.md#intersection-polynomial)

$$
f_A(z_1,\ldots,z_N)=\prod_{\ell\in L}\left(\sum_{i\in A}z_i-\ell\right).
$$

At the characteristic vector $1_B$, its value vanishes when $B\ne A$ and is nonzero when $B=A$. Thus these functions are [linearly independent](../../../vector-space.md#linear-independence) on the whole rank-$k$ layer: evaluate any linear relation at each family member in turn. Replacing every positive power of $z_i$ by $z_i$ preserves all Boolean evaluations, so the functions are restrictions of [multilinear polynomials](../../../polynomial.md#multilinear-polynomial) of degree at most $s$.

We need the sharp [low-degree evaluation rank on a uniform layer](../../../extremal-set-theory.md#low-degree-evaluation-rank-on-a-uniform-layer), not the larger whole-cube dimension $\sum_{j\le s}\binom Nj$. Let $M$ be the integer incidence [matrix](../../../vector-space.md#matrix) with rows indexed by subsets $S$ of size at most $s$, columns by rank-$k$ sets $B$, and entries $1_{S\subseteq B}$. Over the rationals, if $|S|=j\le s$, then

$$
\sum_{\substack{S\subseteq T\subseteq[N]\\|T|=s}}M_{T,\cdot}
=\binom{k-j}{s-j}M_{S,\cdot}.
$$

This coefficient counts the possible $T$ inside each containing column set and is positive because $s\le k$. Consequently the degree-$s$ rows span all rows over $\mathbb Q$, giving rank at most $\binom Ns$. Every larger square minor is therefore the integer zero. Reducing those minors modulo $p$ shows the rank over $\mathbb F_p$ is also at most $\binom Ns$. This transfer avoids dividing by a [binomial coefficient](../../../combinatorics.md#binomial-coefficient) that might vanish modulo $p$. The independent functions $f_A$ lie in this row space, so their number is at most its rank. This proves the theorem in full.

For the requested forbidden-intersection application, split $\mathcal A$ into sets containing coordinate one and sets avoiding it. In the first part, delete one. Distinct original sets have intersection size between one and $2p-1$, excluding $p$. Their reduced intersections therefore lie between zero and $2p-2$, excluding $p-1$, so their residues belong to $L=\{0,\ldots,p-2\}$. The reduced set size is $2p-1$, whose residue is $p-1\notin L$. Frankl-Wilson on the ground set of size $4p-1$ bounds this part by $\binom{4p-1}{p-1}$.

For the avoiding part, first complement every set. The complements contain one, retain size $2p$, and satisfy

$$
|A^c\cap B^c|=4p-|A\cup B|=|A\cap B|.
$$

Delete one and apply the same argument. The [complement splitting for forbidden midpoint intersections](../../../extremal-set-theory.md#complement-splitting-for-forbidden-midpoint-intersections) yields the stronger bound

$$
\boxed{|\mathcal A|\le2\binom{4p-1}{p-1}\le2\binom{4p}{p-1}.}
$$

The split is essential: a family may contain complementary pairs with intersection zero, preventing direct use of $L=\{1,\ldots,p-1\}$ on the original layer.

The [Borsuk conjecture](../../../geometry-and-topology.md#borsuk-conjecture) asserted that a bounded subset of $\mathbb R^d$ of positive [diameter](../../../topological-analysis.md#diameter) can be partitioned into $d+1$ subsets of strictly smaller [diameter](../../../topological-analysis.md#diameter). Here is the [Kahn-Kalai counterexample to the Borsuk conjecture](../../../geometry-and-topology.md#kahn-kalai-counterexample-to-the-borsuk-conjecture), implemented by balanced cut vectors. For each $X\in[4p]^{(2p)}$, define $v_X\in\mathbb R^{\binom{4p}{2}}$ whose coordinate indexed by an unordered pair $\{i,j\}$ is one when exactly one endpoint lies in $X$, and zero otherwise. Complementary sets give the same cut. Choose the representative with $1\in X$, obtaining exactly

$$
M=\binom{4p-1}{2p-1}
$$

distinct points: a cut determines its two parts, and fixing the side containing one removes its only ambiguity. Every cut has $(2p)^2=4p^2$ occupied coordinates, so all points lie in the [affine hyperplane](../../../vector-space.md#affine-hyperplane) with coordinate sum $4p^2$. Its dimension is

$$
d=\binom{4p}{2}-1.
$$

We can identify this hyperplane isometrically with $\mathbb R^d$; no claim of full [affine span](../../../vector-space.md#affine-hull) is needed.

For two side sets with $t=|X\cap Y|$, their [symmetric difference](../../../set.md#symmetric-difference) has $4p-2t$ points. The two cuts disagree exactly on pairs with one endpoint in that [symmetric difference](../../../set.md#symmetric-difference), giving the [balanced cut-vector distance formula](../../../geometry-and-topology.md#balanced-cut-vector-distance-formula)

$$
\boxed{\|v_X-v_Y\|_2^2=(4p-2t)(2t)=4t(2p-t)
=4\bigl(p^2-(t-p)^2\bigr).}
$$

The [diameter](../../../topological-analysis.md#diameter) is $2p$, attained exactly when $t=p$; such pairs exist even among representatives containing one. Thus a smaller-diameter part contains no pair with side intersection $p$. Since all representative sets already contain one, deleting that common coordinate and applying the preceding Frankl-Wilson argument bounds each part by $\binom{4p-1}{p-1}$. There is no extra factor two at this step. This is the cut construction described in [the original Kahn-Kalai paper](https://arxiv.org/abs/math/9307229); the distance and part-size calculations above give the required justification directly.

An explicit choice is $p=13$. The point set lies in dimension

$$
\boxed{d=\binom{52}{2}-1=1325.}
$$

The exact counts are

$$
M=\binom{51}{25}=247959266474052,\qquad
B=\binom{51}{12}=158753389900.
$$

Their ratio requires at least $\lceil M/B\rceil=1562$ smaller-diameter parts, exceeding $d+1=1326$. In particular,

$$
M-1326B=37452271466652>0.
$$

Rescaling the point set to [diameter](../../../topological-analysis.md#diameter) one changes none of these partition counts. Therefore the [Borsuk counterexample in dimension 1325](../../../geometry-and-topology.md#borsuk-counterexample-in-dimension-1325) is fully explicit. This is a concrete dimension, not a claim that it is the smallest possible counterexample dimension.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
