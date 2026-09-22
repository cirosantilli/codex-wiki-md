# Paper 11

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_11.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_11.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)

## 1

↑ **Parent:** [Paper 11](paper-11.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $e(A)$ count internal edges of the [hypercube graph](../../../graph.md#hypercube-graph). Since each vertex has degree $n$, its [edge boundary](../../../combinatorics.md#edge-boundary-in-a-graph) is $b_e(A)=n|A|-2e(A)$. The [edge-isoperimetric inequality in the discrete cube](../../../combinatorics.md#edge-isoperimetric-inequality-in-the-discrete-cube) gives $e(A)\le |A|\log_2|A|/2$, hence $b_e(A)\ge |A|(n-\log_2|A|)$.

For completeness, the [entropy proof of cube edge-isoperimetry](../../../combinatorics.md#entropy-proof-of-cube-edge-isoperimetry) splits the final coordinate into sections of sizes $a,b$. Their internal edges contribute at most $(a\log_2a+b\log_2b)/2$ by induction, and their crossing edges at most $\min(a,b)$. For $m=a+b$ and $t=\min(a,b)/m$, the [binary entropy function](../../../combinatorics.md#binary-entropy-function) satisfies $H_2(t)\ge2t$, so $a\log_2a+b\log_2b+2\min(a,b)\le m\log_2m$. The convention is $0\log_20=0$.

A $k$-dimensional coordinate subcube has $2^k$ vertices and $k2^{k-1}$ internal edges, attaining the bound. Therefore

$$
\boxed{f(2^k)=2^k(n-k)}.
$$

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

A [down-set](../../../extremal-set-theory.md#down-set) in the [Boolean lattice](../../../extremal-set-theory.md#boolean-lattice) is a family closed under taking subsets. Restricting the minimization to down-sets cannot decrease the minimum from the [edge-isoperimetric inequality in the discrete cube](../../../combinatorics.md#edge-isoperimetric-inequality-in-the-discrete-cube).

The coordinate subcube consisting of all subsets of a fixed $k$-element set is itself a down-set and attains that minimum. Thus

$$
\boxed{g(2^k)=2^k(n-k)}.
$$

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Identify cube vertices with subsets of $[n]$. In a [down-set](../../../extremal-set-theory.md#down-set) $D$, every $A\in D$ has all its $|A|$ immediate lower neighbors in $D$. Counting each internal edge by its upper endpoint gives the [edge boundary of a down-set in a cube](../../../extremal-set-theory.md#edge-boundary-of-a-down-set-in-a-cube)

$$
b_e(D)=nm-2\sum_{A\in D}|A|,\qquad m=|D|.
$$

To maximize it, minimize the sum of set sizes. Among all families of $m$ sets, the minimum is obtained by taking the smallest ranks first. This choice is a down-set: take every set of size below $r$, followed by any required selection of $r$-sets.

Write $M_j=\sum_{i=0}^j\binom ni$, with $M_{-1}=0$, and choose $r$ such that $M_{r-1}\le m\le M_r$. The [largest edge boundary of a down-set](../../../extremal-set-theory.md#largest-edge-boundary-of-a-down-set) is therefore

$$
\boxed{h(m)=nm-2\left[\sum_{j=0}^{r-1}j\binom nj+r(m-M_{r-1})\right]}.
$$

Equivalently, it is $\sum_{j<r}(n-2j)\binom nj+(n-2r)(m-M_{r-1})$. This includes $m=0$ and $m=2^n$, with boundary zero. If $m$ is exactly a complete-level size, either adjacent choice of $r$ gives the same value.

## 2

↑ **Parent:** [Paper 11](paper-11.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [Erdős-Ko-Rado theorem](../../../extremal-set-theory.md#erdos-ko-rado-theorem) states that for $1\le r\le n/2$, an [intersecting family](../../../extremal-set-theory.md#intersecting-family) $\mathcal F$ of $r$-subsets of $[n]$ satisfies

$$
\boxed{|\mathcal F|\le\binom{n-1}{r-1}}.
$$

The bound is sharp: take all $r$-sets containing one fixed element.

Use the [Katona circle method](../../../extremal-set-theory.md#katona-circle-method). In any cyclic ordering of $[n]$, the [cyclic interval intersection bound](../../../extremal-set-theory.md#cyclic-interval-intersection-bound) permits at most $r$ members of $\mathcal F$ to appear as length-$r$ intervals. To see the bound directly, rotate a chosen interval so that it ends at $n$. Intervals ending at $r,\ldots,n-r$ miss it. Pair the remaining endpoints except $n$ as $(j,j+n-r)$, $1\le j\le r-1$; the two intervals in each pair are disjoint, so at most one is chosen. Including the fixed interval gives at most $r$.

There are $(n-1)!$ oriented cyclic orders. A fixed $r$-set appears consecutively in $r!(n-r)!$ of them: collapse it to a block, cyclically order that block with the other $n-r$ elements, and order its members internally. [Double counting](../../../combinatorics.md#double-counting-proof-technique) the compatible family-member/order pairs gives $|\mathcal F|r!(n-r)!\le r(n-1)!$, proving the theorem.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Form the family $\mathcal F=\{A\subseteq[n]:\sum_{i\in A}c_i>1/2\}$. The nonnegative weights make it an [up-set](../../../extremal-set-theory.md#up-set). It is an [intersecting family](../../../extremal-set-theory.md#intersecting-family), since two disjoint members would have combined weight exceeding one. The no-tie hypothesis makes it a [self-dual set family](../../../extremal-set-theory.md#self-dual-set-family): exactly one of $A,A^c$ belongs.

Let $a_j=|\mathcal F\cap\binom{[n]}j|/\binom nj$. Self-duality gives $a_{n-j}=1-a_j$. The [Erdős-Ko-Rado theorem](../../../extremal-set-theory.md#erdos-ko-rado-theorem) gives $a_j\le j/n$ for $j<n/2$; at $j=0$ this is immediate. If $n$ is even, $a_{n/2}=1/2$.

The [biased measure of a set family](../../../extremal-set-theory.md#biased-measure-of-a-set-family) is $\mu_p(\mathcal F)=\sum_j\binom nj a_jp^j(1-p)^{n-j}$. By independence of the [Bernoulli random variables](../../../discrete-probability-distribution.md#bernoulli-distribution), it equals $\mathbb P(Z\ge1/2)$, since equality is excluded. Subtract $p=\sum_j\binom nj(j/n)p^j(1-p)^{n-j}$ and pair complementary levels. The [complementary-layer bound for biased measure](../../../extremal-set-theory.md#complementary-layer-bound-for-biased-measure) gives

$$
\mu_p(\mathcal F)-p=\sum_{j<n/2}\binom nj\left(\frac jn-a_j\right)\left[p^{n-j}(1-p)^j-p^j(1-p)^{n-j}\right]\ge0.
$$

Both factors are nonnegative for $p\ge1/2$. The endpoints $p=1/2,1$ also follow directly, or by continuity. Thus the [weighted Bernoulli majority bound](../../../extremal-set-theory.md#weighted-bernoulli-majority-bound) is

$$
\boxed{\mathbb P(Z\ge1/2)\ge p}.
$$

## 3

↑ **Parent:** [Paper 11](paper-11.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The [Ahlswede–Daykin inequality](../../../extremal-set-theory.md#ahlswede-daykin-inequality), also called the [four functions theorem](../../../extremal-set-theory.md#ahlswede-daykin-inequality), concerns nonnegative functions $\alpha,\beta,\gamma,\delta$ on $\mathcal P([n])$. If

$$
\alpha(A)\beta(B)\le\gamma(A\cup B)\delta(A\cap B)\qquad\text{for all }A,B,
$$

then

$$
\boxed{\left(\sum_A\alpha(A)\right)\left(\sum_A\beta(A)\right)\le\left(\sum_A\gamma(A)\right)\left(\sum_A\delta(A)\right)}.
$$

Prove it by induction on $n$. The case $n=0$ is the single assumed inequality. For the induction step, sum each function over the last coordinate to obtain $\alpha',\beta',\gamma',\delta'$ on $\mathcal P([n-1])$. For fixed $A,B$ in this smaller cube, set $a_i=\alpha(A\cup i\{n\})$, $b_i=\beta(B\cup i\{n\})$, $c_i=\gamma((A\cup B)\cup i\{n\})$, and $d_i=\delta((A\cap B)\cup i\{n\})$, where $i\{n\}$ is empty for $i=0$ and $\{n\}$ for $i=1$.

The hypotheses give $a_0b_0\le c_0d_0$, $a_1b_1\le c_1d_1$ and $a_0b_1,a_1b_0\le c_1d_0$. The [two-point four-functions inequality](../../../extremal-set-theory.md#two-point-four-functions-inequality) shows that these imply $(a_0+a_1)(b_0+b_1)\le(c_0+c_1)(d_0+d_1)$. Here is its key algebra: put $x=a_0b_1$, $y=a_1b_0$, $M=c_1d_0$, $N=c_0d_1$. Then $x,y\le M$ and $xy\le MN$. If $M>0$, $(M-x)(M-y)\ge0$ gives $x+y\le M+xy/M\le M+N$; if $M=0$, both cross terms vanish. Adding the two diagonal bounds proves the claim.

Thus the primed functions satisfy the same hypothesis, and the induction hypothesis applies. Their totals equal the original totals, completing the proof.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

In the [four functions theorem](../../../extremal-set-theory.md#ahlswede-daykin-inequality), take $\alpha=\mathbf1_{\mathcal A}$, $\beta=\mathbf1_{\mathcal B}$, $\gamma=\mathbf1_{\mathcal A\vee\mathcal B}$ and $\delta=\mathbf1_{\mathcal A\wedge\mathcal B}$, where the [union and intersection of set families](../../../extremal-set-theory.md#union-and-intersection-of-set-families) are the collections of all pairwise unions and intersections.

If $\alpha(A)\beta(B)=1$, then $A\cup B\in\mathcal A\vee\mathcal B$ and $A\cap B\in\mathcal A\wedge\mathcal B$, so the pointwise hypothesis holds. Otherwise its left side is zero. Summing these [indicator functions](../../../measure-theory.md#indicator-function) gives

$$
\boxed{|\mathcal A\vee\mathcal B|\,|\mathcal A\wedge\mathcal B|\ge|\mathcal A|\,|\mathcal B|}.
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Complement the members of $\mathcal B$ in the fixed ground set: $\mathcal C=\{[n]\setminus B:B\in\mathcal B\}$, so $|\mathcal C|=|\mathcal B|$. The [set difference](../../../set.md#set-difference) identities

$$
A\cap B^c=A\setminus B,\qquad A\cup B^c=(B\setminus A)^c
$$

show that $\mathcal A\wedge\mathcal C=\mathcal A-\mathcal B$, while complementation bijects $\mathcal A\vee\mathcal C$ with $\mathcal B-\mathcal A$. Applying the [four functions theorem](../../../extremal-set-theory.md#ahlswede-daykin-inequality) to $\mathcal A,\mathcal C$ therefore gives

$$
\boxed{|\mathcal A-\mathcal B|\,|\mathcal B-\mathcal A|\ge|\mathcal A|\,|\mathcal B|}.
$$

The products count distinct resulting sets, with repeated pairwise differences included only once.

## 4

↑ **Parent:** [Paper 11](paper-11.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

An [independence graph of events](../../../probabilistic-combinatorics.md#dependency-graph-of-events), also called a [dependency graph of events](../../../probabilistic-combinatorics.md#dependency-graph-of-events), has one vertex for each event $E_i$, with $E_i$ independent of the entire family of events indexed by its nonneighbors. Precisely, $E_i$ is independent of the [sigma-algebra](../../../measure-theory.md#sigma-algebra) generated by those events. Pairwise independence alone is insufficient.

The [asymmetric Lovász local lemma](../../../probabilistic-combinatorics.md#asymmetric-lovasz-local-lemma) says that if numbers $0\le x_i<1$ satisfy

$$
\mathbb P(E_i)\le x_i\prod_{j\in N(i)}(1-x_j),
$$

then $\mathbb P(\bigcap_iE_i^c)\ge\prod_i(1-x_i)>0$ for a finite family. In the commonly used symmetric [Lovász local lemma](../../../probabilistic-combinatorics.md#lovasz-local-lemma), if each probability is at most $q$ and the maximum graph degree is at most $d$, the sufficient condition is

$$
\boxed{eq(d+1)\le1}.
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Color each integer independently and uniformly with one of $k$ colors. For a translate $S+t$, let $E_t$ be the event that some color is missing. The [union bound](../../../probability-inequality.md#boole-s-inequality) gives

$$
\mathbb P(E_t)\le k(1-1/k)^s\le ke^{-s/k}.
$$

Join two events in the [dependency graph of events](../../../probabilistic-combinatorics.md#dependency-graph-of-events) when their translates overlap. Nonneighbors depend on disjoint sets of independent colors, giving the required joint independence. Overlap occurs only if $u-t\in S-S$, so the maximum degree is at most $s(s-1)$.

With natural logarithms, $s\ge6k\log k$ and $k\ge20$ imply

$$
eq(d+1)\le ek s^2e^{-s/k}\le\frac{36e(\log k)^2}{k^3}\le\frac{36e}{k^2}\le\frac{36e}{400}<1.
$$

The middle estimate uses that $s^2e^{-s/k}$ is decreasing for $s\ge2k$, and the next uses $\log k\le\sqrt{k}$. Therefore the [Lovász local lemma](../../../probabilistic-combinatorics.md#lovasz-local-lemma) supplies a coloring avoiding every bad event in any specified finite family of translates.

To obtain one coloring for all translates, use the [compactness extension of the Lovász local lemma](../../../probabilistic-combinatorics.md#compactness-extension-of-the-lovasz-local-lemma). At level $N$, consider colorings of $[-N,N]\cap\mathbb Z$ satisfying every constraint whose translate is contained in that interval. There are finitely many constraints, and the preceding argument makes the level nonempty. Restrictions connect these colorings into a finitely branching [tree](../../../combinatorics.md#tree-graph-theory). The [König infinity lemma](../../../combinatorics.md#konig-s-lemma) gives an infinite branch, hence a coloring of all integers. Every translate eventually lies in a level of this branch, so it contains every color.

Thus **there exists a $k$-coloring of $\mathbb Z$ in which every translate of $S$ contains all $k$ colors**. This is a [polychromatic coloring of integer translates](../../../hypergraph.md#polychromatic-coloring-of-integer-translates); the compactness step establishes existence of one simultaneous coloring.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
