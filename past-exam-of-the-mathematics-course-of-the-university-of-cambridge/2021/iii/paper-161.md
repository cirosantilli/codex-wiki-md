# Paper 161

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_161.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_161.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)

## 1

↑ **Parent:** [Paper 161](paper-161.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $X$ be the number of crossings in the drawing, placed in general position. Deleting at most one edge at each crossing leaves a [planar graph](../../../graph-theory.md#planar-graph), so the [Euler formula for a connected planar graph](../../../graph-theory.md#euler-formula-for-a-connected-planar-graph) gives

$$
m-X\leq3n,
\qquad\text{hence}\qquad X\geq m-3n.
$$

Now retain every vertex independently with probability $p$, together with every edge whose endpoints survive. The expected numbers of retained vertices, edges and crossings are $pn,p^2m,p^4X$. Applying the preceding inequality to each sampled drawing and taking expectations gives

$$
p^4X\geq p^2m-3pn.
$$

Because $m\geq6n$, choose $p=6n/m\leq1$. Then

$$
p^2m-3pn=\frac{18n^2}{m},
$$

and therefore

$$
X\geq\frac{18n^2/m}{(6n/m)^4}
=\frac1{72}\frac{m^3}{n^2}.
$$

**Thus the [Crossing lemma](../../../graph-theory.md#crossing-lemma) holds here with the absolute constant $c=1/72$.**

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Regard each equation $P_i(x_j)=y_j$ as an incidence between the point $(x_j,y_j)$ and the graph of $P_i$. On each polynomial graph, join consecutive incident points by the intervening arc. If $I$ is the number of incidences, the resulting topological graph has

$$
M\geq I-m
$$

edges and $n$ vertices.

Two distinct degree-$d$ polynomial graphs meet in at most $d$ points because a nonzero polynomial of degree at most $d$ has at most $d$ real roots. Their drawn arcs therefore create at most $d$ genuine crossings. Parallel arcs with the same endpoints may be perturbed to cross once; for each pair of polynomials, such crossing-free lenses occur only between consecutive roots of their difference and hence at most $d$ times. The total number of genuine and added crossings is consequently

$$
O(dm^2).
$$

After these perturbations, a crossing-free subgraph is simple, so the sampling proof of the [Crossing lemma](../../../graph-theory.md#crossing-lemma) applies to this topological graph.

If $M<6n$, then $I<m+6n$. Otherwise the crossing lemma gives

$$
c\frac{M^3}{n^2}\leq C_0dm^2,
$$

and hence

$$
M=O(d^{1/3}m^{2/3}n^{2/3}).
$$

Since $I\leq M+m$, both cases combine to prove the [incidences between points and polynomial graphs](../../../combinatorics.md#incidences-between-points-and-polynomial-graphs) bound

$$
\boxed{I\leq C\left(m+n+d^{1/3}m^{2/3}n^{2/3}\right)}
$$

for an absolute constant $C$.

## 2

↑ **Parent:** [Paper 161](paper-161.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy) and [conditioning reduces entropy](../../../information-theory.md#conditioning-reduces-entropy) give

$$
H(X,Y)=H(X)+H(Y\mid X)\leq H(X)+H(Y).
$$

Thus [subadditivity of information entropy](../../../information-theory.md#subadditivity-of-information-entropy) holds for two finitely valued [random variables](../../../random-variable.md). Applying this inequality to $(X_1,\ldots,X_{n-1})$ and $X_n$ and then inducting gives

$$
\boxed{H(X_1,\ldots,X_n)\leq\sum_{i=1}^nH(X_i)}.
$$

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

[Shearer's inequality](../../../information-theory.md#shearer-s-inequality) states that if $X=(X_1,\ldots,X_n)$ is a discrete [random vector](../../../random-variable.md#random-vector) and $\mathcal F$ is a collection of subsets of $[n]$ in which every index occurs at least $t$ times, then

$$
\boxed{tH(X)\leq\sum_{F\in\mathcal F}H(X_F)}.
$$

Order the coordinates naturally. For every $F\in\mathcal F$, the [chain rule for information entropy](../../../information-theory.md#chain-rule-for-information-entropy) gives

$$
H(X_F)=\sum_{i\in F}H\left(X_i\mid X_j:j\in F,\ j<i\right).
$$

Removing conditioning variables cannot decrease entropy, so every summand is at least

$$
H(X_i\mid X_1,\ldots,X_{i-1}).
$$

After summing over $F$, each index $i$ contributes at least $t$ times. A final application of the chain rule yields

$$
\sum_{F\in\mathcal F}H(X_F)
\geq t\sum_{i=1}^nH(X_i\mid X_1,\ldots,X_{i-1})
=tH(X),
$$

which proves the lemma.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Choose $A$ uniformly from $\mathcal A$, and let $X_i=\mathbf1_{\{i\in A\}}$. The [characteristic vector of a set](../../../extremal-set-theory.md#characteristic-vector-of-a-set) determines $A$, so

$$
H(X_1,ldots,X_n)=\log|\mathcal A|.
$$

For $F\in\mathcal F$, the projected vector $X_F$ determines the intersection $A\cap F$ and therefore takes values in the [trace of a set family](../../../extremal-set-theory.md#trace-of-a-set-family) $T_F(\mathcal A)$. The maximum-entropy bound on a finite set gives

$$
H(X_F)\leq\log|T_F(\mathcal A)|.
$$

Every coordinate belongs to at least $t$ members of $\mathcal F$, so [Shearer's inequality](../../../information-theory.md#shearer-s-inequality) gives

$$
t\log|\mathcal A|
\leq\sum_{F\in\mathcal F}\log|T_F(\mathcal A)|.
$$

Exponentiation proves the [Shearer trace inequality](../../../extremal-set-theory.md#shearer-trace-inequality)

$$
\boxed{|\mathcal A|\leq
\left(\prod_{F\in\mathcal F}|T_F(\mathcal A)|\right)^{1/t}}.
$$

## 3

↑ **Parent:** [Paper 161](paper-161.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

The coefficient form of the [Combinatorial Nullstellensatz](../../../combinatorics.md#combinatorial-nullstellensatz) is the following. Let $f\in F[x_1,\ldots,x_n]$ have total degree at most $d_1+\cdots+d_n$, and suppose

$$
[x_1^{d_1}\cdots x_n^{d_n}]f\ne0.
$$

For arbitrary subsets $S_i\subseteq F$ with $|S_i|=d_i+1$, there is an $x\in S_1\times\cdots\times S_n$ such that $f(x)\ne0$.

For the proof, define

$$
\phi_i'(a)=\prod_{b\in S_i\setminus\{a\}}(a-b).
$$

Successive [Lagrange interpolation](../../../numerical-analysis.md#lagrange-polynomial) in the variables gives the [Alon-Tarsi lemma](../../../combinatorics.md#alon-tarsi-lemma)

$$
[x_1^{d_1}\cdots x_n^{d_n}]f
=\sum_{a_i\in S_i}
\frac{f(a_1,\ldots,a_n)}{\prod_i\phi_i'(a_i)}.
$$

Every denominator is nonzero because the elements of $S_i$ are distinct. If $f$ vanished throughout the product grid, the right side and hence the assumed nonzero coefficient would vanish. This contradiction proves the theorem.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Consider the degree-$n$ polynomial

$$
f(x_1,\ldots,x_n)=\prod_{i=1}^n\left(\sum_{j=1}^na_{ij}x_j-b_i\right).
$$

To form the square-free monomial $x_1\cdots x_n$, one must choose each variable exactly once from the $n$ factors. Such choices are indexed by permutations, so

$$
[x_1\cdots x_n]f
=\sum_{\sigma\in S_n}\prod_{i=1}^na_{i,\sigma(i)}
=\operatorname{perm}A.
$$

This coefficient is nonzero by hypothesis. Apply the [Combinatorial Nullstellensatz](../../../combinatorics.md#combinatorial-nullstellensatz) with every $d_i=1$ and the given two-element sets $S_i$. It supplies $x\in\prod_iS_i$ with $f(x)\ne0$. Every factor is then nonzero, so

$$
(Ax)_i\ne b_i
$$

for all $i$. This is [coordinate avoidance from a nonzero permanent](../../../combinatorics.md#coordinate-avoidance-from-a-nonzero-permanent).

## 4

↑ **Parent:** [Paper 161](paper-161.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For each $A\in\mathcal A$, define over $\mathbb F_p$

$$
P_A(x_1,\ldots,x_n)
=\prod_{e\in E}\left(\sum_{i\in A}x_i-e\right).
$$

Replace every power $x_i^r$ with $r\geq1$ by $x_i$; this does not change the values on [characteristic vectors of sets](../../../extremal-set-theory.md#characteristic-vector-of-a-set) and produces a multilinear polynomial of degree at most $m$.

At the characteristic vector of $B\in\mathcal A$,

$$
P_A(\mathbf1_B)=\prod_{e\in E}(|A\cap B|-e).
$$

This is zero when $A\ne B$, whereas

$$
P_A(\mathbf1_A)=\prod_{e\in E}(|A|-e)\ne0.
$$

The evaluation matrix is diagonal with nonzero diagonal, so the polynomials $P_A$ are [linearly independent](../../../vector-space.md#linear-independence). The space of multilinear polynomials of degree at most $m$ has the monomial basis $\prod_{i\in S}x_i$ for $|S|\leq m$ and dimension $\sum_{i=0}^m\binom ni$. Hence the [modular intersection bound for a set family](../../../combinatorics.md#modular-intersection-bound-for-a-set-family) gives

$$
\boxed{|\mathcal A|\leq\binom n0+\binom n1+\cdots+\binom nm}.
$$

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Let $\mathcal A$ be an [independent set](../../../graph-theory.md#independent-set-graph-theory) in the graph. Every member has size $p^2\equiv0\pmod p$, while for distinct $A,B\in\mathcal A$, independence means $|A\cap B|$ is nonzero modulo $p$. Apply part i with

$$
E=\mathbb F_p\setminus\{0\},
\qquad m=p-1.
$$

This gives

$$
\alpha(G)\leq\sum_{i=0}^{p-1}\binom{p^3}{i}.
$$

Moreover,

$$
\sum_{i=0}^{p-1}\binom{p^3}{i}
\leq p(p^3)^{p-1}=p^{3p-2}<p^{3p}.
$$

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Let $\mathcal C$ be a [clique](../../../graph-theory.md#clique-graph-theory) and choose the given prime $q$ with $p^2<q<2p^2$. For distinct $A,B\in\mathcal C$, the intersection size is a multiple of $p$ strictly below $p^2$. In $\mathbb F_q$, set

$$
E=\{0,p,2p,\ldots,(p-1)p\}.
$$

These are $p$ distinct residues because $q>p^2$, every off-diagonal intersection size lies in $E$, and the diagonal size $p^2$ does not. Part i, now over $\mathbb F_q$, yields

$$
\omega(G)\leq\sum_{i=0}^{p}\binom{p^3}{i}.
$$

The subsets of a $p^3$-element set having size at most $p$ inject into its ordered $p$-tuples: list a nonempty subset increasingly and repeat its final element, while assigning the empty set one decreasing tuple not used in this way. The injection is not surjective, so

$$
\boxed{\sum_{i=0}^{p}\binom{p^3}{i}<(p^3)^p=p^{3p}.}
$$

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Put $k=p^{3p}$. Parts ii and iii give a graph with neither a [clique](../../../graph-theory.md#clique-graph-theory) nor an [independent set](../../../graph-theory.md#independent-set-graph-theory) of size $k$. Its number of vertices satisfies the standard binomial lower bound

$$
\binom{p^3}{p^2}
\geq\left(\frac{p^3}{p^2}\right)^{p^2}
=p^{p^2}.
$$

Consequently the [modular-intersection graph Ramsey lower bound](../../../ramsey-theory.md#modular-intersection-graph-ramsey-lower-bound) gives

$$
\boxed{R(k,k)\geq p^{p^2}}.
$$

For every fixed $C>0$,

$$
\log(p^{p^2})=p^2\log p,
\qquad
\log(k^C)=3Cp\log p.
$$

The first quantity exceeds the second when $p>3C$. Thus $p^{p^2}$ is eventually larger than $k^C$ for every fixed $C$, so this lower bound grows faster than every [polynomial](../../../polynomial.md) in $k$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
