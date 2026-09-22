# Paper 109

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_109.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_109.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 109](paper-109.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For a [uniform set family](../../../extremal-set-theory.md#uniform-set-family) $\mathcal A\subseteq[n]^{(r)}$, the [Local LYM inequality](../../../extremal-set-theory.md#local-lym-inequality) is

$$
\frac{|\partial\mathcal A|}{\binom n{r-1}}
\geq
\frac{|\mathcal A|}{\binom nr}.
$$

To prove it, count the incident pairs $(B,A)$ with $B\in\partial\mathcal A$, $A\in\mathcal A$, and $B\subset A$. Every $A$ contributes exactly $r$ pairs, whereas every $B$ belongs to at most $n-r+1$ members of $[n]^{(r)}$. Therefore

$$
r|\mathcal A|\leq(n-r+1)|\partial\mathcal A|,
$$

which is the displayed inequality after using the [binomial coefficient](../../../combinatorics.md#binomial-coefficient) identity $r\binom nr=(n-r+1)\binom n{r-1}$.

The [LYM inequality](../../../extremal-set-theory.md#lubell-yamamoto-meshalkin-inequality) says that every [antichain](../../../extremal-set-theory.md#antichain) $\mathcal A\subseteq\mathcal P([n])$ satisfies

$$
\boxed{\displaystyle \sum_{A\in\mathcal A}\binom n{|A|}^{-1}\leq1.}
$$

For the proof from the local inequality, take the lowest occupied level below the middle and replace that level by its [upper shadow](../../../extremal-set-theory.md#upper-shadow). The result remains an [antichain](../../../extremal-set-theory.md#antichain): any new containment involving a set in the upper shadow would already give a containment involving the member of $\mathcal A$ immediately below it. The dual form of the [Local LYM inequality](../../../extremal-set-theory.md#local-lym-inequality) says that this replacement cannot decrease the [Lubell mass](../../../extremal-set-theory.md#lubell-mass). Repeating upward below the middle, and similarly replacing high levels by their [lower shadows](../../../extremal-set-theory.md#lower-shadow), eventually puts the whole family in one middle level. Its final Lubell mass is at most one, so the original mass is also at most one.

For the [maximal chain in a Boolean lattice](../../../extremal-set-theory.md#maximal-chain-in-a-boolean-lattice) proof, choose a [Uniformly random maximal chain in a Boolean lattice](../../../extremal-set-theory.md#uniformly-random-maximal-chain-in-a-boolean-lattice). An $h$-element set lies on it with [probability](../../../probability-theory.md#probability) $1/\binom nh$. Because an [antichain](../../../extremal-set-theory.md#antichain) meets each chain at most once, the [expected value](../../../probability-theory.md#expected-value) of the number of its members on the chain is at most one. By [linearity of expectation](../../../probability-theory.md#linearity-of-expectation), that expected value is precisely the displayed sum.

The [Sperner theorem](../../../extremal-set-theory.md#sperner-s-theorem) follows because $\binom n{|A|}\leq\binom n{\lfloor n/2\rfloor}$ for every $A$. If equality holds in the resulting cardinality bound, every member lies on a largest level. For even $n$ this is the unique middle level. For odd $n$, the two middle levels have equal size; the regular connected inclusion graph between them and equality in [Local LYM inequality](../../../extremal-set-theory.md#local-lym-inequality) force a chosen portion of the lower level to be either empty or the whole level. Hence the maximum [antichains](../../../extremal-set-theory.md#antichain) are **exactly the complete middle level, with either middle level allowed when $n$ is odd**.

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The hypothesis says exactly that $\mathcal A$ is a [k-Sperner family](../../../extremal-set-theory.md#k-sperner-family) with $k=2$: it contains no three members forming a strict inclusion chain. Every [maximal chain in a Boolean lattice](../../../extremal-set-theory.md#maximal-chain-in-a-boolean-lattice) consequently contains at most two members of $\mathcal A$, so the same random-chain argument gives $\lambda(\mathcal A)\leq2$. For a fixed amount of [Lubell mass](../../../extremal-set-theory.md#lubell-mass), cardinality is maximized by using the levels with the two largest [binomial coefficients](../../../combinatorics.md#binomial-coefficient). The [Erdős theorem on k-Sperner families](../../../extremal-set-theory.md#erdos-theorem-on-k-sperner-families) therefore gives

$$
\boxed{
|\mathcal A|\leq
\begin{cases}
\binom{2m}{m}+\binom{2m}{m-1},&n=2m,\\[2mm]
2\binom{2m+1}{m},&n=2m+1.
\end{cases}}
$$

The bound is attained by taking the union of two levels having those sizes.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Let $\mathcal A\subseteq[n]^{(r)}$ be an [intersecting family](../../../extremal-set-theory.md#intersecting-family), with $n\geq2r$. By the [Iterated local LYM inequality](../../../extremal-set-theory.md#iterated-local-lym-inequality), its upper shadow in level $n-r$ satisfies

$$
|\nabla^{,n-2r}\mathcal A|
\geq
\frac{\binom n{n-r}}{\binom nr}|\mathcal A|
=|\mathcal A|.
$$

The family of complements $\mathcal A^c=\{[n]\setminus A:A\in\mathcal A\}$ also lies in level $n-r$ and has cardinality $|\mathcal A|$. It is disjoint from the upper shadow: if $A\subseteq[n]\setminus B$ for $A,B\in\mathcal A$, then $A\cap B=\varnothing$, contradicting intersection. Both families fit inside the $(n-r)$th level, so

$$
2|\mathcal A|\leq\binom n{n-r}=\binom nr.
$$

Thus replacing the [Kruskal-Katona theorem](../../../extremal-set-theory.md#kruskal-katona-theorem) by Local LYM gives only

$$
\boxed{|\mathcal A|\leq\frac12\binom nr.}
$$

This agrees with the [Erdős-Ko-Rado theorem](../../../extremal-set-theory.md#erdos-ko-rado-theorem) when $n=2r$ but is weaker when $n>2r$.

## 2

↑ **Parent:** [Paper 109](paper-109.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The [Kruskal-Katona theorem](../../../extremal-set-theory.md#kruskal-katona-theorem) states that if $\mathcal A\subseteq[n]^{(r)}$ has the unique [binomial representation](../../../combinatorics.md#combinatorial-number-system)

$$
|\mathcal A|=\binom{a_r}{r}+\binom{a_{r-1}}{r-1}+\cdots+\binom{a_s}{s},
\qquad a_r>a_{r-1}>\cdots>a_s\geq s,
$$

then its [lower shadow](../../../extremal-set-theory.md#lower-shadow) obeys

$$
|\partial\mathcal A|\geq
\binom{a_r}{r-1}+\binom{a_{r-1}}{r-2}+\cdots+\binom{a_s}{s-1}.
$$

An initial segment of [colexicographic order](../../../extremal-set-theory.md#colexicographic-order) has exactly this shadow.

Here is the [UV-compression proof of the Kruskal-Katona theorem](../../../extremal-set-theory.md#uv-compression-proof-of-the-kruskal-katona-theorem). For disjoint equal-size sets $U,V$, the [UV-compression](../../../extremal-set-theory.md#uv-compression) $C_{U,V}$ replaces the pattern $V$ by $U$ when the image is not already in the family. If the family is not an initial colexicographic segment, choose a changing pair with $\max U<\max V$ and $|U|$ minimal. Minimality ensures that for every $x\in U$ an appropriate smaller compression $C_{U\setminus\{x\},V\setminus\{y\}}$ already fixes the family. The [Shadow lemma for UV-compressions](../../../extremal-set-theory.md#shadow-lemma-for-uv-compressions) then gives

$$
|\partial C_{U,V}(\mathcal A)|\leq|\partial\mathcal A|.
$$

Meanwhile the binary weight $\sum_{A\in\mathcal A}\sum_{i\in A}2^i$ strictly decreases. Iterating must terminate, and a terminal family is an initial colexicographic segment. Computing that segment's shadow from its [binomial representation](../../../combinatorics.md#combinatorial-number-system) proves the theorem.

We next classify pairs that decrease the shadow for _every_ uniform family. The answer, including the identity case, is

$$
\boxed{|U|=|V|\leq1.}
$$

For $|U|=0$ the operation is the identity. For $|U|=1$, the hypotheses of the [Shadow lemma for UV-compressions](../../../extremal-set-theory.md#shadow-lemma-for-uv-compressions) reduce to stability under the empty compression and therefore hold for every family.

To see failure for larger pairs, relabel freely. If $|U|=|V|=2$, write $U=\{u_1,u_2\}$ and $V=\{v_1,v_2\}$. The family

$$
\mathcal A=\{u_1v_1,u_1v_2,v_1v_2\}
$$

has a three-point lower shadow, whereas its compression replaces $v_1v_2$ by $u_1u_2$ and has a four-point lower shadow. If the common size is $m\geq3$, take

$$
\mathcal A=\left\{V,\ \{u_1\}\cup(V\setminus\{v_m\})\right\}.
$$

The old two shadows overlap once and have size $2m-1$. Compression replaces $V$ by $U$; the two resulting $m$-sets intersect in only $u_1$, so their lower shadows are disjoint and have size $2m$.

For the two specified pairs, the answer is **no in both cases**, even after assuming the family is [left-compressed](../../../extremal-set-theory.md#left-compressed-set-family).

For $(U,V)=(345,126)$, take

$$
\mathcal A=\{123,124,125,126\}.
$$

This family is left-compressed. Its compression replaces $126$ by $345$. The old shadow is

$$
\{12,13,23,14,24,15,25,16,26\},
$$

of size nine, while the new shadow replaces the last two pairs by $34,35,45$ and has size ten.

For $(U,V)=(145,236)$, take the left-compressed family

$$
\mathcal A=\{123,124,125,126,134,135,136,234,235,236\}.
$$

Its shadow consists of $12,13,23$ and the nine pairs having one element in $\{1,2,3\}$ and one in $\{4,5,6\}$, so it has size twelve. Compression replaces $236$ by $145$; all twelve old shadow pairs remain and $45$ is added. The new shadow therefore has size thirteen.

## 3

↑ **Parent:** [Paper 109](paper-109.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Write $N[A]$ for the [closed graph neighbourhood](../../../graph-theory.md#closed-graph-neighbourhood) of $A$. Since $|N[A]|=|A|+|\partial_vA|$, minimizing the [external vertex boundary](../../../graph-theory.md#external-vertex-boundary) at fixed cardinality is equivalent to minimizing the closed neighbourhood. The [vertex-isoperimetric inequality in a grid](../../../combinatorics.md#vertex-isoperimetric-inequality-in-a-grid) says that, among all $t$-vertex subsets of $[k]^n$, the first $t$ vertices in the [simplicial order on a grid](../../../combinatorics.md#simplicial-order-on-a-grid) minimize this quantity.

We prove the theorem by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on $n$, using the allowed two-dimensional case. Fix a coordinate $i$ and write $A_j\subseteq[k]^{n-1}$ for the section in which that coordinate equals $j$. Replace each $A_j$ by the equally large initial simplicial segment $B_j$. By induction, $|N[B_j]|\leq|N[A_j]|$. The [section formula for a grid neighbourhood](../../../combinatorics.md#section-formula-for-a-grid-neighbourhood) gives

$$
N[A]_j=N[A_j]\cup A_{j-1}\cup A_{j+1},
\qquad A_0=A_{k+1}=\varnothing.
$$

For the compressed family, $N[B_j],B_{j-1},B_{j+1}$ are nested initial segments, so the size of their union is the maximum of their sizes. That maximum is no larger than the size of the corresponding uncompressed union. Summing over $j$ proves that [coordinate compression in a product of paths](../../../combinatorics.md#coordinate-compression-in-a-product-of-paths) does not enlarge the boundary.

Apply these compressions in every coordinate, choosing among boundary-minimizing outcomes one with least coordinate-sum weight. If the result were not an initial simplicial segment, it would contain a later vertex while omitting an earlier one. After cancelling coordinates in which they agree, this gives an inversion in a two-coordinate face. Replacing the occupied portion of that face by the equal-size initial segment in $[k]^2$ does not increase its neighbourhood by the assumed two-dimensional theorem, while it strictly lowers the weight. This contradiction is the [local-to-global lemma for simplicial grid order](../../../combinatorics.md#local-to-global-lemma-for-simplicial-grid-order), and completes the induction.

For the second assertion, list the vertices of $Q_2$ in the [Gray code](../../../graph.md#gray-code) order

$$
00,\ 01,\ 11,\ 10.
$$

The three consecutive edges form a copy of the four-vertex path $P_4$. Pairing the $2n$ binary coordinates and applying this identification in each pair realizes

$$
[4]^n=P_4^n
$$

as a [spanning subgraph](../../../graph-theory.md#spanning-subgraph) of the [hypercube graph](../../../graph.md#hypercube-graph) $Q_{2n}$. For any fixed vertex set, adding graph edges can only enlarge its [external vertex boundary](../../../graph-theory.md#external-vertex-boundary). Hence a $t$-set in $Q_{2n}$ has boundary at least that of the same $t$ vertices in $[4]^n$, which by hypothesis is at least $s$. Therefore

$$
\boxed{|\partial_{Q_{2n}}A|\geq s\quad\text{whenever }|A|=t.}
$$

## 4

↑ **Parent:** [Paper 109](paper-109.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A multiset $\mathcal C$ of subsets of $[n]$ is a [uniform cover](../../../combinatorics.md#uniform-cover) of multiplicity $k$ when each coordinate occurs in exactly $k$ members. The [uniform covers theorem](../../../combinatorics.md#uniform-covers-theorem) states that every [Euclidean body](../../../combinatorics.md#euclidean-body) $S\subseteq\mathbb R^n$ satisfies

$$
\boxed{|S|^k\leq\prod_{A\in\mathcal C}|S_A|,}
$$

where $S_A$ is the [coordinate projection of a Euclidean body](../../../combinatorics.md#coordinate-projection-of-a-euclidean-body) onto the coordinates in $A$.

We prove it by induction on $n$. Split the cover into $\mathcal C^-$, whose members omit $n$, and $\mathcal C^+$, whose members contain $n$. Exactly $k$ members lie in $\mathcal C^+$. For a last-coordinate value $x$, let $S(x)\subseteq\mathbb R^{n-1}$ be the corresponding slice. Removing $n$ from the members of $\mathcal C^+$ and retaining the members of $\mathcal C^-$ gives a $k$-uniform cover of $[n-1]$. The inductive hypothesis and [Fubini's theorem](../../../measure-theory.md#fubini-s-theorem) give

$$
\begin{aligned}
|S|
&=\int |S(x)|\,dx\\
&\leq
\prod_{A\in\mathcal C^-}|S_A|^{1/k}
\int\prod_{A\in\mathcal C^+}|S(x)_{A\setminus\{n\}}|^{1/k}\,dx.
\end{aligned}
$$

Apply [Hölder's inequality](../../../real-analysis.md#holder-s-inequality) to the $k$ factors in the integral. Since

$$
\int|S(x)_{A\setminus\{n\}}|\,dx=|S_A|,
$$

we obtain $|S|\leq\prod_{A\in\mathcal C}|S_A|^{1/k}$, which is the result after taking the $k$th power. The one-dimensional base case is immediate.

The [Bollobas--Thomason box theorem](../../../combinatorics.md#box-theorem) states that for every body $S\subseteq\mathbb R^n$ there is an [axis-parallel box](../../../combinatorics.md#axis-parallel-box) $B$ such that

$$
\boxed{|B|=|S|\quad\text{and}\quad |B_A|\leq|S_A|\text{ for every }A\subseteq[n].}
$$

An [irreducible uniform cover](../../../combinatorics.md#irreducible-uniform-cover) cannot be decomposed into two smaller uniform covers. There are only finitely many such covers of $[n]$: encode a cover by its multiplicity vector in $\mathbb N^{2^n}$ and apply the [Dickson lemma](../../../combinatorics.md#dickson-s-lemma).

Choose a componentwise minimal positive array $(x_A)_{A\subseteq[n]}$ satisfying

$$
x_A\leq|S_A|,
\qquad
|S|^k\leq\prod_{A\in\mathcal C}x_A
$$

for every irreducible $k$-uniform cover $\mathcal C$, together with

$$
x_A\leq\prod_{i\in A}x_{\{i\}}.
$$

The actual projection volumes are feasible by the [uniform covers theorem](../../../combinatorics.md#uniform-covers-theorem), and finiteness gives a minimal array. Every uniform cover is a disjoint union of irreducible ones, so its cover inequality also holds for this array.

Minimality implies that, for each coordinate $i$, some tight uniform-cover inequality can be chosen whose cover contains the singleton $\{i\}$. Indeed, either such an inequality already blocks decreasing $x_{\{i\}}$, or a tight product inequality $x_A=\prod_{j\in A}x_{\{j\}}$ does; in the latter case take a tight cover containing $A$ and replace that occurrence of $A$ by its singleton coordinates. Let these tight covers be $\mathcal C_i$, of multiplicities $k_i$, and let $K=\sum_i k_i$. Their multiset union is a $K$-uniform cover. Removing one copy of every singleton leaves a $(K-1)$-uniform cover, so comparison of its cover inequality with the product of all the tight equalities yields

$$
\prod_{i=1}^n x_{\{i\}}\leq|S|.
$$

The singleton cover gives the reverse inequality, hence

$$
\prod_i x_{\{i\}}=|S|.
$$

For any $A\subseteq[n]$, the one-uniform cover consisting of $A$ and the singletons $\{i\}$ for $i\notin A$ now gives $x_A\geq\prod_{i\in A}x_{\{i\}}$. The defining product inequality gives the reverse bound. Thus all these quantities are equal. Taking the side lengths of $B$ to be $x_{\{1\}},\ldots,x_{\{n\}}$ proves the theorem.

Finally suppose that the proper body $S\subseteq\mathbb R^3$ satisfies

$$
|S|^2=|S_{12}|\,|S_{13}|\,|S_{23}|.
$$

This is equality in the three-dimensional [Loomis--Whitney inequality](../../../combinatorics.md#loomis-whitney-inequality). In its proof, equality must hold in both applications of [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Their equality conditions force the three projection indicators to factor through one-dimensional measurable sets $E_1,E_2,E_3$, and force

$$
S=E_1\times E_2\times E_3
$$

up to a set of [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) zero; this is [Equality in the three-dimensional Loomis--Whitney inequality](../../../combinatorics.md#equality-in-the-three-dimensional-loomis-whitney-inequality).

Because $S$ is connected, each one-coordinate projection is connected and hence is an interval. Because $S$ is a finite union of positive-volume [axis-parallel boxes](../../../combinatorics.md#axis-parallel-box), a proper difference between $S$ and the product of those three intervals would contain a positive-volume rectangular cell in a common finite subdivision. That would contradict equality up to measure zero. Consequently the equality is exact and

$$
\boxed{S\text{ is an axis-parallel box}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
