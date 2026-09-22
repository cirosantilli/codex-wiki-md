# Paper 149

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_149.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_149.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)

## 1

↑ **Parent:** [Paper 149](paper-149.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Plünnecke-Ruzsa inequality](../../../additive-combinatorics.md#plunnecke-ruzsa-inequality) states that, for all [nonnegative integers](../../../arithmetic.md#natural-number) $m,n$,

$$
\boxed{|mA-nA|\leq K^{m+n}|A|.}
$$

Here $mA$ is the [iterated sumset](../../../additive-combinatorics.md#iterated-sumset) of $m$ copies of $A$, with $0A=\{0\}$. In particular, $|mA|\leq K^m|A|$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Noncommutative Ruzsa triangle inequality](../../../additive-combinatorics.md#noncommutative-ruzsa-triangle-inequality) says that nonempty finite subsets $B,C,D$ of a [group](../../../group.md) satisfy

$$
|B|\,|CD^{-1}|\leq |CB^{-1}|\,|BD^{-1}|.
$$

The [Ruzsa covering lemma](../../../additive-combinatorics.md#ruzsa-covering-lemma) says that if $|CD|\leq K|D|$, then some $X\subseteq C$ with $|X|\leq K$ satisfies

$$
C\subseteq XDD^{-1}.
$$

Now let $A$ be a [symmetric subset of a group](../../../additive-combinatorics.md#symmetric-subset-of-a-group), so $A^{-1}=A$ and $1\in A$. Apply the triangle inequality with the middle set $A$ to obtain, for $m\geq4$,

$$
|A|\,|A^m|\leq |A^{m-1}|\,|A^3|.
$$

The hypothesis therefore gives $|A^m|\leq K|A^{m-1}|$. Starting from $|A^3|\leq K|A|$ proves

$$
\boxed{|A^m|\leq K^{m-2}|A|\qquad(m\geq3).}
$$

In particular $|A^5|\leq K^3|A|$. Apply the covering lemma to $C=A^4$ and $D=A$. There is $X\subseteq A^4$ with $|X|\leq K^3$ such that

$$
A^4\subseteq XAA^{-1}=XA^2.
$$

The set $A^2$ is symmetric and contains the [identity element](../../../group.md#identity-element), so this inclusion is exactly the covering condition showing that

$$
\boxed{A^2\text{ is a }K^3\text{-approximate group}.}
$$

Small doubling alone is insufficient in a [noncommutative group](../../../group.md#non-abelian-group). Let $H$ be a finite group, let $G=H*\langle x\rangle$ be its [free product](../../../algebraic-topology.md#free-product) with an [infinite cyclic group](../../../group.md#infinite-cyclic-group), and put

$$
A=H\cup\{x,x^{-1}\}.
$$

Then $A$ is symmetric and $|A^2|\leq5|H|+4=O(|A|)$, while $A^3$ contains the [double coset](../../../group-theory.md#double-coset) $HxH$. Distinct pairs $(h_1,h_2)\in H^2$ give distinct reduced words $h_1xh_2$, so $|HxH|=|H|^2$. Letting $|H|\to\infty$ proves the [small doubling does not control tripling in a noncommutative group](../../../additive-combinatorics.md#small-doubling-does-not-control-tripling-in-a-noncommutative-group) phenomenon.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

By the [Plünnecke-Ruzsa inequality](../../../additive-combinatorics.md#plunnecke-ruzsa-inequality),

$$
|4A|\leq K^4|A|.
$$

Apply the [Ruzsa covering lemma](../../../additive-combinatorics.md#ruzsa-covering-lemma) to $3A$ and $A$. Since $A=-A$, there is a set $X\subseteq3A$ with $|X|\leq K^4$ such that

$$
3A\subseteq X+A-A=X+2A.
$$

Adding $A$ and reusing this inclusion inductively gives

$$
\boxed{mA\subseteq(m-2)X+2A\qquad(m\geq3).}
$$

A sum of $m-2$ members of the fixed set $X$ depends only on the multiplicity of each member. The number of possible multiplicity vectors is at most $m^{|X|}$, and therefore

$$
|(m-2)X|\leq m^{|X|}\leq m^{K^4}.
$$

Since $|2A|\leq K|A|\leq K^m|A|$, it follows that

$$
\boxed{|mA|\leq K^m m^{K^4}|A|.}
$$

For fixed $K$, this differs from the Plünnecke–Ruzsa bound $K^m|A|$ only by a [polynomial](../../../polynomial.md) factor in $m$, so both have the same leading [exponential function](../../../calculus.md#exponential-function) factor $K^m$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Choose a covering set $X$ of size at most $K$ such that $A^2\subseteq XA$, as allowed by the definition of an [approximate group](../../../additive-combinatorics.md#approximate-group). Discard every $x\in X$ for which $xA$ does not meet $A^2$. Each remaining $x$ belongs to $A^2A^{-1}=A^3$, so $X\subseteq\langle A\rangle$. Induction gives

$$
A^m\subseteq X^{m-1}A.
$$

Because $A$ is symmetric and contains the identity, $\langle A\rangle=\bigcup_{m\geq1}A^m$. Hence

$$
\langle A\rangle=\langle X\rangle A.
$$

We use the [bounded-exponent finitely generated nilpotent group order bound](../../../group-theory.md#bounded-exponent-finitely-generated-nilpotent-group-order-bound). In an $s$-step [nilpotent group](../../../group-theory.md#nilpotent-group), a subgroup generated by $k$ elements is generated in collected form by the simple [group commutators](../../../group.md#group-commutator) in those generators of weights at most $s$. There are at most

$$
k+k^2+\cdots+k^s\leq sk^s
$$

such commutators. Every one has order at most $r$, so

$$
|\langle X\rangle|\leq r^{s|X|^s}\leq r^{sK^s}.
$$

Taking $H=\langle A\rangle$ now gives

$$
\boxed{A\subseteq H,\qquad |H|\leq|\langle X\rangle|\,|A|
\leq r^{sK^s}|A|.}
$$

## 2

↑ **Parent:** [Paper 149](paper-149.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $\pi:G\to G/[G,G]$ be the [abelianization](../../../group-theory.md#abelianization) map. Its image $\pi(A)$ is again a $K$-[approximate group](../../../additive-combinatorics.md#approximate-group). Apply the large-progression form of the [Freiman-Green-Ruzsa theorem](../../../additive-combinatorics.md#freiman-ruzsa-theorem) to $\pi(A)$. It gives a finite subgroup $H$, elements $x_1,\ldots,x_r$, and lengths $L_1,\ldots,L_r$, with

$$
r\leq K^{O(1)},\qquad
HP(x_1,\ldots,x_r;L_1,\ldots,L_r)\subseteq\pi(A^4),
$$

and

$$
|HP|\geq\exp(-K^{O(1)})|\pi(A)|.
$$

The [large lifted product from a coset progression](../../../additive-combinatorics.md#large-lifted-product-from-a-coset-progression) applied to this progression gives

$$
\left|
\bigl(A^{16}\cap\pi^{-1}(H)\bigr)
\prod_{i=1}^r\bigl(A^{22}\cap\pi^{-1}(\langle x_i\rangle)\bigr)
\right|
\geq \exp(-K^{O(1)})|A|.
$$

Briefly, choose a section of $\pi$ on $\pi(A^6)$. Multiplication by that section is multiplicative up to $A^{12}\cap[G,G]$; lifting successively the subgroup part and each progression direction therefore places every element of $A^6\cap\pi^{-1}(HP)$ in the displayed product. The [fiber-counting lemma for a quotient map](../../../additive-combinatorics.md#fiber-counting-lemma-for-a-quotient-map) gives $|A^6\cap\pi^{-1}(HP)|\geq\exp(-K^{O(1)})|A|$, which proves the estimate.

Set

$$
A_0=A^{16}\cap\pi^{-1}(H),\qquad
A_i=A^{22}\cap\pi^{-1}(\langle x_i\rangle)\quad(1\leq i\leq r).
$$

The [intersection of an approximate group power with a subgroup](../../../additive-combinatorics.md#intersection-of-an-approximate-group-power-with-a-subgroup) shows that each $A_i$ is a $K^{O(1)}$-approximate group contained in $A^{O(1)}$. The preimage of a [cyclic subgroup](../../../group.md#cyclic-subgroup) of $G/[G,G]$ has step less than $s$. The same is true of the preimage of the finite subgroup $H$ because $G$ is a [torsion-free group](../../../group.md#torsion-free-group). Consequently each $\langle A_i\rangle$ has step less than $s$, and the displayed estimate is the required conclusion.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Write

$$
C=A_0A_1\cdots A_r.
$$

Under the improved bounds allowed in the question, $r=O(\log^{O(1)}(2K))$ and

$$
|C|\geq\exp\bigl(-O(\log^{O(1)}(2K))\bigr)|A|.
$$

Moreover $AC\subseteq A^{O(1)}$, whose size is at most $K^{O(1)}|A|$ by the [higher product bound for an approximate group](../../../additive-combinatorics.md#higher-product-bound-for-an-approximate-group). Thus

$$
|AC|\leq\exp\bigl(O(\log^{O(1)}(2K))\bigr)|C|.
$$

The [Ruzsa covering lemma](../../../additive-combinatorics.md#ruzsa-covering-lemma) supplies $X\subseteq A$ of size at most $\exp(O(\log^{O(1)}(2K)))$ such that

$$
A\subseteq XCC^{-1}
=XA_0A_1\cdots A_rA_r\cdots A_1A_0.
$$

Taking the $B_i$ to be the factors in this last product gives

$$
\boxed{A\subseteq XB_1\cdots B_k,}
$$

where $k\leq O(\log^{O(1)}(2K))$ and every $B_i$ is a $K^{O(1)}$-approximate group in $A^{O(1)}$ generating a subgroup of step less than $s$.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

We induct on the [nilpotency class](../../../group-theory.md#nilpotency-class) $s$. For $s=1$, the group is [Abelian](../../../group.md#abelian-group), so take $C_1=A$ and no $X_i$. For $s>1$, part (i) writes

$$
A\subseteq XB_1\cdots B_k
$$

with $X$ small and every $\langle B_i\rangle$ of class at most $s-1$. Apply the induction hypothesis to each $B_i$. Since $B_i\subseteq A^{O(1)}$ and its approximation parameter is $K^{O(1)}$, all resulting small sets lie in $A^{O_s(1)}$, all their sizes are at most

$$
\exp\bigl(O_s(\log^{O(1)}(2K))\bigr),
$$

and all resulting approximate groups lie in $A^{O_s(1)}$ and have approximation parameter $K^{O_s(1)}$. Their generated subgroups are [abelian groups](../../../group.md#abelian-group).

There are $O(\log^{O(1)}(2K))$ factors at each of at most $s$ induction levels. Absorbing the resulting products of the bounds into the $O_s$ notation gives

$$
\boxed{m,n\leq O_s(\log^{O_s(1)}(2K)).}
$$

Keeping the factors in the order supplied by the induction yields the required product of the $X_i$ and $C_j$ containing $A$.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Use the product from part (ii). Move each selected element of each small set $X_i$ to the left, conjugating every approximate-group factor that it crosses. For each tuple $\mathbf x\in X_1\times\cdots\times X_m$, the corresponding part of the product is therefore contained in

$$
y_{\mathbf x}D_{1,\mathbf x}\cdots D_{n,\mathbf x},
$$

where every $D_{j,\mathbf x}$ is a [conjugate subset](../../../group-theory.md#conjugate-subset) of some $C_j$. Conjugation preserves cardinality, the approximation parameter, and the property that the generated subgroup is abelian. The conjugating elements belong to $A^{O_s(1)}$, so $D_{j,\mathbf x}\subseteq A^{O_s(1)}$ after enlarging the implicit constant.

The number of tuples is at most

$$
\prod_{i=1}^m|X_i|
\leq\exp\bigl(O_s(\log^{O_s(1)}(2K))\bigr).
$$

These translated products cover $A$, so one has size at least the reciprocal fraction of $|A|$. For that tuple, put $D_j=D_{j,\mathbf x}$. Then

$$
\boxed{|D_1\cdots D_q|
\geq\exp\bigl(-O_s(\log^{O_s(1)}(2K))\bigr)|A|,}
$$

where $q=n\leq O_s(\log^{O_s(1)}(2K))$, and each $D_j$ is a $K^{O_s(1)}$-approximate group generating an [abelian subgroup](../../../group.md#abelian-subgroup).

## 3

↑ **Parent:** [Paper 149](paper-149.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Composition and inversion in the [Affine group of the complex line](../../../group-theory.md#affine-group-of-the-complex-line) are

$$
f_{a,b}\circ f_{a',b'}=f_{aa',\,ab'+b},
\qquad
f_{a,b}^{-1}=f_{a^{-1},\,-a^{-1}b}.
$$

The map

$$
\rho:G\longrightarrow\mathbb C^\times,\qquad
\rho(f_{a,b})=a
$$

is therefore a surjective [group homomorphism](../../../group-theory.md#group-homomorphism) with kernel

$$
N=\{f_{1,b}:b\in\mathbb C\}\cong(\mathbb C,+).
$$

Its target is [Abelian](../../../group.md#abelian-group), so $[G,G]\subseteq N$. On the other hand, the stated computation gives

$$
[f_{a,1},f_{1,b}]=f_{1,b(1-a^{-1})}.
$$

Fixing any $a\ne1$ and varying $b$ produces every translation. Thus $N\subseteq[G,G]$, and hence

$$
\boxed{[G,G]=N\cong(\mathbb C,+),\qquad
G/[G,G]\cong\mathbb C^\times,\qquad
\pi(f_{a,b})=a.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [Solymosi sum-product theorem over the complex numbers](../../../additive-combinatorics.md#solymosi-sum-product-theorem-over-the-complex-numbers) states that if finite $U,V,W\subseteq\mathbb C$ satisfy $U\ne\{0\}$ and $W\ne\{0\}$, then

$$
\boxed{|U+V|\,|UW|
\geq\frac1{56}|U|^{3/2}|V|^{1/2}|W|^{1/2}.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Write $N=[G,G]$ and identify it with $(\mathbb C,+)$ as in part (a). If every two members of $A$ commuted, then $\langle A\rangle$ would be [Abelian](../../../group.md#abelian-group), contrary to hypothesis. Thus some commutator of two members of $A$ is a nonidentity translation in $A^4\cap N$. Consequently the translation-coordinate set

$$
T=\{c\in\mathbb C:f_{1,c}\in A^4\cap N\}
$$

contains both zero and a nonzero element.

The identity

$$
f_{a,b}\circ f_{1,c}\circ f_{a,b}^{-1}=f_{1,ac}
$$

shows that $T\pi(A)$ is contained in the translation coordinates of $A^6\cap N$, while $T+T$ is contained in those of $A^8\cap N$. The [intersection of an approximate group power with a subgroup](../../../additive-combinatorics.md#intersection-of-an-approximate-group-power-with-a-subgroup) therefore gives

$$
|T+T|\leq K^{O(1)}|T|,
\qquad
|T\pi(A)|\leq K^{O(1)}|T|.
$$

Apply the [Solymosi sum-product theorem over the complex numbers](../../../additive-combinatorics.md#solymosi-sum-product-theorem-over-the-complex-numbers) with $U=V=T$ and $W=\pi(A)$. Since $1\in\pi(A)$, its hypotheses hold, and

$$
K^{O(1)}|T|^2
\geq |T+T|\,|T\pi(A)|
\geq\frac1{56}|T|^2|\pi(A)|^{1/2}.
$$

Cancelling $|T|^2$ and absorbing the absolute constant proves

$$
\boxed{|\pi(A)|\leq K^{O(1)}.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Choose one representative from $A$ above each point of $\pi(A)$ and collect them in $X$. Part (c) gives $|X|\leq K^{O(1)}$. If $a\in A$ has the same image as $x\in X$, then $x^{-1}a\in A^2\cap N$, so

$$
A\subseteq X(A^2\cap N).
$$

This is the required covering of $A$ by at most $K^{O(1)}$ left cosets of the abelian translation subgroup $N$.

The set $B=A^2\cap N$ is a $K^{O(1)}$-approximate group by the [intersection of an approximate group power with a subgroup](../../../additive-combinatorics.md#intersection-of-an-approximate-group-power-with-a-subgroup). Apply the [Freiman-Green-Ruzsa theorem](../../../additive-combinatorics.md#freiman-ruzsa-theorem) inside $N\cong(\mathbb C,+)$. Because the additive group of the [complex numbers](../../../complex-analysis.md#complex-number) is a [torsion-free group](../../../group.md#torsion-free-group), the finite subgroup part is trivial, so there is an [abelian progression](../../../additive-combinatorics.md#abelian-progression) $P$ with

$$
B\subseteq P,\qquad
\operatorname{rank}P\leq K^{O(1)},\qquad
|P|\leq\exp(K^{O(1)})|B|.
$$

Since $|B|\leq|A^2|\leq K|A|$, enlarging the implicit constant gives

$$
\boxed{A\subseteq XP,\qquad |X|\leq K^{O(1)},\qquad
\operatorname{rank}P\leq K^{O(1)},\qquad
|P|\leq\exp(K^{O(1)})|A|.}
$$

## 4

↑ **Parent:** [Paper 149](paper-149.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Put $t=\lceil\sqrt n\rceil$ and consider the powers

$$
S^t,S^{5t},S^{5^2t},\ldots,S^{5^{L+1}t},
$$

where $L$ is maximal subject to $5^{L+1}t\leq n/20$. For $n$ sufficiently large in terms of $d$, one has $L+1\geq\frac13\log_5n$. Since the successive growth ratios telescope,

$$
\prod_{i=0}^L\frac{|S^{5^{i+1}t}|}{|S^{5^it}|}
\leq\frac{|S^n|}{|S|}
\leq n^d.
$$

Thus one ratio is at most $n^{d/(L+1)}\leq5^{3d}$. For the corresponding $m=5^it$,

$$
\sqrt n\leq m\leq\frac n{100},
\qquad
|S^{5m}|\leq O_d(1)|S^m|.
$$

Set $B=S^m$. Then $|B^3|\leq O_d(1)|B|$, so the small-tripling argument from Question 1(b) makes

$$
A=B^2=S^{2m}
$$

an $O_d(1)$-approximate group. Apply the [Breuillard-Green-Tao structure theorem for approximate groups](../../../additive-combinatorics.md#breuillard-green-tao-structure-theorem-for-approximate-groups). It gives subgroups

$$
H\trianglelefteq C<G
$$

such that

$$
H\subseteq A^4=S^{8m}\subseteq S^{\lfloor n/2\rfloor},
$$

$C/H$ is a [nilpotent group](../../../group-theory.md#nilpotent-group) of class $O_d(1)$, and $A$ is covered by $O_d(1)$ left cosets of $C$.

It remains to pass from a covering to an index bound. The ball $S^m\subseteq A$ meets only $O_d(1)$ vertices of the [Schreier graph](../../../geometric-group-theory.md#schreier-graph) of $G/C$. If $G/C$ had more vertices, a simple path from $C$ would give more than that many distinct cosets within distance $O_d(1)$. Since $m\geq\sqrt n$ and $n$ is sufficiently large, this is impossible. Therefore

$$
\boxed{H\trianglelefteq C<G,\quad H\subseteq S^{\lfloor n/2\rfloor},
\quad [G:C]=O_d(1),\quad C/H\text{ is }O_d(1)\text{-step nilpotent}.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Apply part (a). The subgroup $H$ is finite because it lies in the finite set $S^{\lfloor n/2\rfloor}$. Conjugation gives a homomorphism

$$
C\longrightarrow\operatorname{Aut}(H).
$$

Its kernel $C_0$ has finite index in $C$ and centralizes $H$. Since $C_0H/H$ is a subgroup of the $O_d(1)$-step nilpotent group $C/H$, it is itself nilpotent of class $O_d(1)$. Hence

$$
\gamma_{s+1}(C_0)\subseteq H
$$

for some $s=O_d(1)$. As $C_0$ centralizes $H$, one more [group commutator](../../../group.md#group-commutator) vanishes, so $\gamma_{s+2}(C_0)=\{1\}$. Thus $C_0$ is nilpotent of class at most $s+1=O_d(1)$.

Both $[G:C]$ and $[C:C_0]$ are finite, so

$$
\boxed{G\text{ has an }O_d(1)\text{-step nilpotent subgroup of finite index}.}
$$

This is the [Gromov theorem on groups of polynomial growth](../../../geometric-group-theory.md#gromov-s-theorem-on-groups-of-polynomial-growth) in the form needed here.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

The [Cayley graph](../../../geometric-group-theory.md#cayley-graph) $\operatorname{Cay}_S(G)$ is a connected graph with $|G|$ vertices. A shortest path never repeats a vertex, so it has at most $|G|-1$ edges. Therefore

$$
\boxed{\operatorname{diam}_S(G)\leq|G|-1<|G|.}
$$

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Fix $\varepsilon>0$ and set $d=2/\varepsilon$. Suppose, towards a contradiction, that

$$
D=\operatorname{diam}_S(G)>\max\{|G|^\varepsilon,\lambda\},
$$

where $\lambda$ will absorb constants depending only on $\varepsilon$. Put $n=\lfloor|G|^\varepsilon\rfloor$. Once $\lambda$ is large enough, $n\geq N(d)$, $n<D$, and

$$
|S^n|\leq|G|\leq n^d|S|.
$$

Part (a) yields $H\trianglelefteq C<G$ with $[G:C]=O_\varepsilon(1)$, $H\subseteq S^{\lfloor n/2\rfloor}$, and $C/H$ nilpotent of class $O_\varepsilon(1)$.

The [subgroup core](../../../group-theory.md#core-group-theory) $\bigcap_{g\in G}gCg^{-1}$ is normal in $G$ and has index at most $[G:C]!$. Since $G$ is a [simple group](../../../finite-group-theory.md#simple-group), the core is either $\{1\}$ or $G$. In the first case $|G|\leq [G:C]!=O_\varepsilon(1)$, which is excluded by increasing $\lambda$. Hence the core is $G$, so $C=G$.

Now $H\trianglelefteq G$. Since $n/2<D$, the ball $S^{\lfloor n/2\rfloor}$ is not all of $G$, so $H\ne G$. Simplicity gives $H=\{1\}$, and therefore $G=C/H$ is a [nilpotent group](../../../group-theory.md#nilpotent-group). A nontrivial finite nilpotent group has nontrivial [center of a group](../../../group-theory.md#center-of-a-group); simplicity would force that center to be all of $G$, making $G$ [Abelian](../../../group.md#abelian-group). This contradicts the assumption that $G$ is non-abelian. Consequently

$$
\boxed{\operatorname{diam}_S(G)\leq\max\{|G|^\varepsilon,\lambda(\varepsilon)\}.}
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
