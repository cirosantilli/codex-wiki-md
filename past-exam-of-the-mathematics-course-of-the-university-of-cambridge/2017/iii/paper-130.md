# Paper 130

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_130.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_130.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
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

## 1

↑ **Parent:** [Paper 130](paper-130.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Write $\mathbb N=\{1,2,\ldots\}$ and let $\chi$ be the given [finite coloring](../../../ramsey-theory.md#finite-coloring) of the [edges](../../../graph-theory.md#edge-of-a-graph) of the [complete graph](../../../graph-theory.md#complete-graph) on the [positive integers](../../../number-theory.md#positive-integer). Construct an increasing [sequence](../../../real-analysis.md#sequence) $(v_i)$ and nested [infinite sets](../../../set.md#infinite-set) $A_0\supset A_1\supset\cdots$ as follows. Set $A_0=\mathbb N$. Having chosen $A_{i-1}$, take $v_i=\min A_{i-1}$, partition $A_{i-1}\setminus\{v_i\}$ by the color of $\{v_i,w\}$, and use the [infinite pigeonhole principle](../../../algebra.md#infinite-pigeonhole-principle) to choose an [infinite set](../../../set.md#infinite-set) $A_i$ on which this color is constant, say $r_i$. Every element of $A_i$ exceeds $v_i$.

The [infinite pigeonhole principle](../../../algebra.md#infinite-pigeonhole-principle) applied again to $(r_i)$ gives an [infinite set](../../../set.md#infinite-set) of indices $I$ and a color $r$ such that $r_i=r$ for all $i\in I$. For $i<j$ in $I$, nesting gives $v_j\in A_i$, so $\chi(\{v_i,v_j\})=r$. Thus the [infinite set](../../../set.md#infinite-set) $X=\{v_i:i\in I\}$ is a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [complete graph](../../../graph-theory.md#complete-graph):

$$
\boxed{\chi\big|_{X^{(2)}}\equiv r.}
$$

This proves the required infinite case of [Ramsey's theorem](../../../ramsey-theory.md#ramsey-s-theorem); finiteness of the color set is used at both applications of the [infinite pigeonhole principle](../../../algebra.md#infinite-pigeonhole-principle).

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Pull the given [finite coloring](../../../ramsey-theory.md#finite-coloring) $\chi:\mathbb N\to[k]$ back to a [finite coloring](../../../ramsey-theory.md#finite-coloring) of unordered pairs by putting

$$
\widetilde\chi(\{a,b\})=\chi(ab^2)\qquad(a<b).
$$

The ordering $a<b$ makes this a well-defined [function](../../../function.md) on the [edges](../../../graph-theory.md#edge-of-a-graph) of a [complete graph](../../../graph-theory.md#complete-graph). By [Ramsey's theorem](../../../ramsey-theory.md#ramsey-s-theorem), some [infinite set](../../../set.md#infinite-set) $X=\{x_1<x_2<\cdots\}$ has all its pairs of one color $r$ under $\widetilde\chi$. Consequently

$$
\boxed{\chi(x_i x_j^2)=r\qquad(i<j).}
$$

Possible coincidences between these products cause no difficulty, since the original [finite coloring](../../../ramsey-theory.md#finite-coloring) assigns each [positive integer](../../../number-theory.md#positive-integer) a single color.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Use the [cyclic logarithmic coloring](../../../ramsey-theory.md#cyclic-logarithmic-coloring)

$$
\boxed{\rho(x)=\left\lfloor\log_{3/2}x\right\rfloor\pmod 3\qquad(x\geq1).}
$$

Here the [floor function](../../../calculus.md#floor-function) places $x$ in the unique half-open [real interval](../../../real-analysis.md#interval-mathematics) $[(3/2)^j,(3/2)^{j+1})$. If $y/x\in[1.9,2]$, then

$$
1<\log_{3/2}(y/x)<2,
$$

because $3/2<1.9\leq2<(3/2)^2$. For any real $t$ and $1<u<2$, $\lfloor t+u\rfloor-\lfloor t\rfloor$ is either $1$ or $2$. Applying this to the [logarithms](../../../calculus.md#logarithm) of $x$ and $y$ shows that their bin indices differ by $1$ or $2$, and hence have different residues in [modular arithmetic](../../../number-theory.md#modular-arithmetic) modulo $3$. This proves the required separation, including both endpoints of the prescribed ratio interval. The half-open bins remove any ambiguity at their boundaries.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Let $\rho$ be the [cyclic logarithmic coloring](../../../ramsey-theory.md#cyclic-logarithmic-coloring) from part (iii). Define a [finite coloring](../../../ramsey-theory.md#finite-coloring) of the [positive integers](../../../number-theory.md#positive-integer) by

$$
\chi(n)=\rho(\log_2 n)\quad(n\geq2),\qquad \chi(1)=0.
$$

The inner [logarithm](../../../calculus.md#logarithm) is at least $1$ whenever $n\geq2$, so this is defined everywhere. Suppose an increasing infinite [sequence](../../../real-analysis.md#sequence) $(x_i)$ made every product with distinct indices [monochromatic](../../../ramsey-theory.md#monochromatic-set). Fix an index $i$ with $x_i\geq2$ and write $a=\log_2 x_i>0$. The [sequence](../../../real-analysis.md#sequence) is unbounded, so choose $j>i$ with $b=\log_2 x_j\geq28a$. Both ordered products are among the supposedly [monochromatic](../../../ramsey-theory.md#monochromatic-set) values, but their [logarithms](../../../calculus.md#logarithm) satisfy

$$
\frac{\log_2(x_i x_j^2)}{\log_2(x_j x_i^2)}
=\frac{a+2b}{2a+b},\qquad
\boxed{1.9\leq\frac{a+2b}{2a+b}<2.}
$$

Indeed, the first inequality is equivalent to $b\geq28a$, and the second uses $a>0$. Part (iii) therefore gives $\chi(x_i x_j^2)\ne\chi(x_j x_i^2)$, a contradiction. Thus **the assertion with all distinct ordered indices is false**. The obstruction needs an infinite unbounded [sequence](../../../real-analysis.md#sequence); it does not assert that every pair of different [positive integers](../../../number-theory.md#positive-integer) gives different colors.

## 2

↑ **Parent:** [Paper 130](paper-130.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

We prove the [Hales-Jewett theorem](../../../ramsey-theory.md#hales-jewett-theorem) by [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) on the [alphabet](../../../information-theory.md#alphabet) size. A [combinatorial line](../../../ramsey-theory.md#combinatorial-line) has a nonempty active coordinate set, with one common letter in all those coordinates. More generally, a $d$-dimensional [combinatorial subspace](../../../ramsey-theory.md#combinatorial-subspace) has $d$ disjoint nonempty active coordinate sets, each with an independently variable letter.

First prove the [alphabet insensitivity lemma](../../../ramsey-theory.md#alphabet-insensitivity-lemma), rather than assume it. Fix distinct letters $a,b\in[m]$, $k$ colors, and dimension $d$. Partition the coordinates into consecutive blocks of lengths $L_1,\ldots,L_d$, chosen from left to right. Put $S_0=0$ and choose

$$
L_i=k^{\,m^{S_{i-1}+d-i}},\qquad S_i=S_{i-1}+L_i,\qquad N=S_d.
$$

Construct the variable blocks from right to left. When working on block $i$, the later blocks have already become $(d-i)$-parameter words, while all earlier $S_{i-1}$ coordinates remain unrestricted. For each $t\in\{0,\ldots,L_i\}$, take the color vector of the word having $a^t b^{L_i-t}$ in block $i$, indexed by every earlier word and every assignment to the later parameters. There are $m^{S_{i-1}+d-i}$ entries and hence at most $L_i$ different vectors. The [pigeonhole principle](../../../algebra.md#pigeonhole-principle) gives $t<s$ with identical vectors. Fix the first $t$ positions of this block to $a$, fix its last $L_i-s$ positions to $b$, and make the intervening $s-t$ positions a new variable block. Substituting $a$ or $b$ there gives exactly the two equal color vectors.

This equality holds for every earlier word and every later parameter assignment. Restricting the earlier coordinates in subsequent steps therefore preserves it. Likewise, the insensitivity already proved in a later block survives every restriction of earlier coordinates. At the end, we obtain a $d$-dimensional [combinatorial subspace](../../../ramsey-theory.md#combinatorial-subspace) whose induced [finite coloring](../../../ramsey-theory.md#finite-coloring) is unchanged whenever any parameter switches between $a$ and $b$, with all other parameters fixed. Multiple switches preserve the color by successive single switches. This is the [alphabet insensitivity lemma](../../../ramsey-theory.md#alphabet-insensitivity-lemma) in full.

For [alphabet](../../../information-theory.md#alphabet) size $1$, one coordinate is already a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [combinatorial line](../../../ramsey-theory.md#combinatorial-line). Suppose the [Hales-Jewett theorem](../../../ramsey-theory.md#hales-jewett-theorem) has been proved for [alphabet](../../../information-theory.md#alphabet) size $m-1$, and let $d=n(m-1,k)$. Apply the proved [alphabet insensitivity lemma](../../../ramsey-theory.md#alphabet-insensitivity-lemma) with letters $m-1,m$ to get a $d$-dimensional [combinatorial subspace](../../../ramsey-theory.md#combinatorial-subspace) in $[m]^N$. Restrict its parameter words to $[m-1]^d$. The induction hypothesis gives a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [combinatorial line](../../../ramsey-theory.md#combinatorial-line) in these parameters. The union of its active parameter blocks is nonempty, so its image is a [combinatorial line](../../../ramsey-theory.md#combinatorial-line) in the original coordinates. Its additional point with active letter $m$ has the same color as the point with active letter $m-1$, by insensitivity. Therefore all $m$ points have one color, proving

$$
\boxed{n(m,k)<\infty\quad\text{for every }m,k\geq1.}
$$

The construction supplies a finite recursive bound; optimal bounds are not needed.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Let the required [arithmetic progression](../../../arithmetic.md#arithmetic-progression) have length $m\geq2$, let $k$ be the number of colors, and take $n=n(m,k)$ from the [Hales-Jewett theorem](../../../ramsey-theory.md#hales-jewett-theorem). Given any [finite coloring](../../../ramsey-theory.md#finite-coloring) $\chi$ of $[mn]$, color a [word over an alphabet](../../../foundations-of-mathematics.md#string) $w\in[m]^n$ by $\chi(w_1+\cdots+w_n)$. For a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [combinatorial line](../../../ramsey-theory.md#combinatorial-line), let $A\ne\varnothing$ be its active coordinate set and let $C$ be the sum of its fixed coordinates. The sums of its $m$ words are

$$
C+|A|,\ C+2|A|,\ldots,\ C+m|A|.
$$

They all lie in $[mn]$, have one color, and form an [arithmetic progression](../../../arithmetic.md#arithmetic-progression) with strictly positive [common difference](../../../arithmetic.md#common-difference) $|A|$. Thus, writing $W(k,m)$ for the finite [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem) bound,

$$
\boxed{W(k,m)\leq m\,n(m,k).}
$$

The length-one case is immediate. Restricting a [finite coloring](../../../ramsey-theory.md#finite-coloring) of the [positive integers](../../../number-theory.md#positive-integer) to this finite [integer interval](../../../number-theory.md#integer-interval) gives the infinite-domain formulation of the [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem) as well.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

A [run of a word](../../../foundations-of-mathematics.md#run-of-a-word) is a maximal consecutive block of equal letters. For every $N\geq1$, use the following [finite coloring](../../../ramsey-theory.md#finite-coloring) of $[3]^N$, with at most nine colors:

$$
\boxed{\chi(w)=\bigl(w_1,\ R(w)\pmod3\bigr),\qquad
R(w)=1+\sum_{j=1}^{N-1}\mathbf1_{\{w_j\ne w_{j+1}\}}.}
$$

We show that this [run-count obstruction to interval-active lines](../../../ramsey-theory.md#run-count-obstruction-to-interval-active-lines) excludes every [monochromatic](../../../ramsey-theory.md#monochromatic-set) [combinatorial line](../../../ramsey-theory.md#combinatorial-line) with an interval active set $[a,b]$. If $a=1$, its three words already have different first coordinates, so their colors differ. Suppose $a>1$ and denote the letter immediately to the left by $p$. All contributions to $R(w)$ away from the two possible boundaries of $[a,b]$ are independent of its active letter $x$; no internal active boundary contributes a change.

If $b=N$, the only variable contribution is $\mathbf1_{\{p\ne x\}}$, which is $0$ at $x=p$ and $1$ at another letter. If $b<N$, write $q$ for the letter immediately to the right. The variable contribution is

$$
\mathbf1_{\{p\ne x\}}+\mathbf1_{\{x\ne q\}}.
$$

When $p=q$, its values are $0$ and $2$. When $p\ne q$, it equals $1$ at $x=p$ or $x=q$, and equals $2$ at the third letter. In every case these values are distinct modulo $3$. Hence **no dimension works for [alphabet](../../../information-theory.md#alphabet) size three and nine colors**, which disproves the proposed universal strengthening. For the PDF's illustrative line, choosing either adjacent letter merges one active run with a neighboring run, while choosing any other letter merges neither; this is exactly the boundary effect measured above. Recording the first letter also handles active intervals meeting the beginning, including the entire coordinate set.

## 3

↑ **Parent:** [Paper 130](paper-130.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Use the standard definition of a [partition regular matrix](../../../ramsey-theory.md#partition-regular-matrix): for every [finite coloring](../../../ramsey-theory.md#finite-coloring) of the [positive integers](../../../number-theory.md#positive-integer), there is a positive solution whose coordinates all have one color. Coordinates may repeat. Clearing denominators lets us assume $a_i\in\mathbb Z\setminus\{0\}$; multiplication of the row by a nonzero [rational number](../../../number-theory.md#rational-number) changes neither its zero-sum [subsets](../../../set.md#subset) nor its solutions. We prove both directions of the [Rado theorem for one equation](../../../ramsey-theory.md#rado-theorem-for-one-equation) directly, without invoking any form of [Rado's theorem](../../../ramsey-theory.md#rado-s-theorem).

For necessity, choose a [prime number](../../../number-theory.md#prime-number) $p>\sum_i|a_i|$ and use the [last nonzero digit coloring](../../../ramsey-theory.md#last-nonzero-digit-coloring): write $x=p^{v_p(x)}u$, with $p\nmid u$, and assign color $u\bmod p$. Given a [monochromatic](../../../ramsey-theory.md#monochromatic-set) solution, let $v=\min_i v_p(x_i)$, let $I=\{i:v_p(x_i)=v\}$, and let $r\ne0$ be the common color. Divide $\sum_i a_i x_i=0$ by $p^v$ and reduce modulo $p$. Terms outside $I$ vanish; the others give

$$
r\sum_{i\in I}a_i\equiv0\pmod p.
$$

The nonzero residue $r$ is invertible modulo the [prime number](../../../number-theory.md#prime-number) $p$, so $p$ divides $\sum_{i\in I}a_i$. This sum has absolute value less than $p$, forcing it to be zero. The set $I$ is nonempty by its definition.

For sufficiency we first derive the needed [Brauer progression theorem](../../../ramsey-theory.md#brauer-progression-theorem) from the permitted [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem). Fix [positive integers](../../../number-theory.md#positive-integer) $s,\ell$. We claim that for every number of colors $r$, a finite [integer interval](../../../number-theory.md#integer-interval) $[B(r,s,\ell)]$ forces a [monochromatic](../../../ramsey-theory.md#monochromatic-set) set

$$
\{sd,\ a,a+d,\ldots,a+(\ell-1)d\},\qquad a,d>0.
$$

The case $\ell=1$ is immediate by taking $a=s$ and $d=1$. For $r=1$ and $\ell\geq2$, take $a=d=1$ in an interval of length at least $\max(s,\ell)$. Suppose the claim holds for $r-1$ and write $M=B(r-1,s,\ell)$. By the [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem), some $R$ forces an [arithmetic progression](../../../arithmetic.md#arithmetic-progression) of length $(\ell-1)M+1$ in $[R]$ with one color $q$. Work in $[\max(R,sMR)]$ so that all needed multiples also lie in the coloring's domain. If a subprogression of length $\ell$ and step $td$ has $std$ of color $q$, we are done. Otherwise, for every $1\leq t\leq M$, the initial long [arithmetic progression](../../../arithmetic.md#arithmetic-progression) contains such a subprogression, and $std$ avoids color $q$. The induced [finite coloring](../../../ramsey-theory.md#finite-coloring) $t\mapsto\chi(sdt)$ of $[M]$ therefore uses at most $r-1$ colors. The induction hypothesis gives a [monochromatic](../../../ramsey-theory.md#monochromatic-set) set $\{se,b,b+e,\ldots,b+(\ell-1)e\}$ for this induced [finite coloring](../../../ramsey-theory.md#finite-coloring). Multiplying by $sd$ gives the desired configuration in the original coloring, with initial term $sdb$ and step $sde$. This proves the claim for $\ell\geq2$; the only use below has $\ell\geq3$.

Now suppose $\sum_{i\in I}a_i=0$ for a nonempty $I$. Choose $i_0\in I$, put $B=\sum_{i\notin I}a_i$, and put $s=|a_{i_0}|$. If $B=0$, then $\sum_i a_i=0$ and any constant positive vector is already a [monochromatic](../../../ramsey-theory.md#monochromatic-set) solution. Otherwise take $L=|B|$ and apply the proved [Brauer progression theorem](../../../ramsey-theory.md#brauer-progression-theorem) with $\ell=2L+1$. All of $sd$ and $a+jd$ for $0\leq j\leq2L$ have one color. Define

$$
x_i=\begin{cases}
sd,&i\notin I,\\
a+Ld,&i\in I\setminus\{i_0\},\\
a+\bigl(L-\operatorname{sgn}(a_{i_0})B\bigr)d,&i=i_0.
\end{cases}
$$

Every coordinate is a [positive integer](../../../number-theory.md#positive-integer) in that [monochromatic](../../../ramsey-theory.md#monochromatic-set) set, since $L-\operatorname{sgn}(a_{i_0})B$ is either $0$ or $2L$. Using the zero sum on $I$ gives

$$
\sum_i a_i x_i=sBd-a_{i_0}\operatorname{sgn}(a_{i_0})Bd=0.
$$

Thus both directions are proved:

$$
\boxed{(a_1,\ldots,a_n)\text{ is partition regular}\iff
\exists\,\varnothing\ne I\subseteq[n]:\ \sum_{i\in I}a_i=0.}
$$

For $n=1$ the right side is impossible, agreeing with the absence of positive solutions for a single nonzero coefficient.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

First justify the finite bound used in the hint. Fix $k$. If no finite $T$ forced a [monochromatic](../../../ramsey-theory.md#monochromatic-set) positive solution of $\sum_i a_i x_i=0$, consider the rooted [tree](../../../combinatorics.md#tree-graph-theory) whose level $t$ consists of the solution-free [finite colorings](../../../ramsey-theory.md#finite-coloring) of $[t]$, with restriction as the predecessor map. Every level is nonempty and every vertex has at most $k$ children. The [König infinity lemma](../../../combinatorics.md#konig-s-lemma) gives an infinite branch, hence a [finite coloring](../../../ramsey-theory.md#finite-coloring) of all [positive integers](../../../number-theory.md#positive-integer) with no such solution, contradicting the [partition regular matrix](../../../ramsey-theory.md#partition-regular-matrix) hypothesis. This is the [compactness bound for partition regularity](../../../ramsey-theory.md#compactness-bound-for-partition-regularity).

Choose such a $T$ and let $S=\operatorname{lcm}(1,\ldots,T)$, the [least common multiple](../../../number-theory.md#least-common-multiple). For a given [finite coloring](../../../ramsey-theory.md#finite-coloring) $\chi$ of the [positive integers](../../../number-theory.md#positive-integer), pull it back to $[T]$ by

$$
\widetilde\chi(t)=\chi(S/t).
$$

Each $S/t$ is a [positive integer](../../../number-theory.md#positive-integer) in $[S]$. The defining property of $T$ gives $x_1,\ldots,x_n\in[T]$ of one color under $\widetilde\chi$, with $\sum_i a_i x_i=0$. Set $y_i=S/x_i$. Their colors under $\chi$ agree, and

$$
\boxed{\sum_{i=1}^n\frac{a_i}{y_i}
=\frac1S\sum_{i=1}^n a_i x_i=0.}
$$

Thus [reciprocal partition regularity](../../../ramsey-theory.md#reciprocal-partition-regularity) follows. This construction is an involution on the divisors of $S$; it permits repeated coordinates and never requires a reciprocal of a [positive integer](../../../number-theory.md#positive-integer) to itself be integral without the common scaling factor $S$.

## 4

↑ **Parent:** [Paper 130](paper-130.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Use the [product topology](../../../geometry-and-topology.md#product-topology) on $\mathcal C=[k]^{\mathbb Z}$, with $[k]$ discrete, and the [left shift](../../../dynamical-systems.md#left-shift) $(\mathcal Lc)(j)=c(j+1)$. A basic [cylinder set](../../../geometry-and-topology.md#cylinder-set) specifies finitely many coordinates. This is a [compact metric space](../../../topological-analysis.md#compact-metric-space), and $\mathcal L$ is a [homeomorphism](../../../topology.md#homeomorphism). Write $Y=\overline{\{\mathcal L^n c:n\geq0\}}$ for the forward [orbit closure](../../../dynamical-systems.md#orbit-closure). A [minimal point](../../../dynamical-systems.md#minimal-point) means that $Y$ is a [minimal dynamical system](../../../dynamical-systems.md#minimal-dynamical-system), equivalently that every point of $Y$ has a dense forward [orbit](../../../dynamical-systems.md#orbit-dynamical-system) in $Y$; it need not be a [fixed point](../../../function.md#fixed-point).

There is a convention needed in the source: the bounded-gaps property concerns every **finite** [integer interval](../../../number-theory.md#integer-interval) $I$, hence every finite [word over an alphabet](../../../foundations-of-mathematics.md#string). Literally allowing $I=\mathbb Z$ would make the displayed condition impossible for finite $U$, although a constant coloring is a [minimal point](../../../dynamical-systems.md#minimal-point). Under the standard finite-word interpretation, the property is precisely [uniform recurrence](../../../dynamical-systems.md#uniform-recurrence).

Suppose first that $Y$ is a [minimal dynamical system](../../../dynamical-systems.md#minimal-dynamical-system). Its nonempty compact forward-invariant [subset](../../../set.md#subset) $\mathcal L(Y)$ must equal $Y$. As the ambient [left shift](../../../dynamical-systems.md#left-shift) is invertible, all [integer](../../../number-theory.md#integer) translates of $c$ belong to $Y$. Let $I=[a,b]\cap\mathbb Z$ have length $\ell=b-a+1$, and let $V=\{z\in Y:z|_I=c|_I\}$. This is a nonempty [clopen set](../../../topology.md#clopen-set). Each forward [orbit](../../../dynamical-systems.md#orbit-dynamical-system) in $Y$ meets $V$, so $\{\mathcal L^{-n}V:n\geq0\}$ covers $Y$. By [compactness](../../../topology.md#compact-space), finitely many suffice; let $D$ be the largest index in this finite cover. For any [integer](../../../number-theory.md#integer) $u$, the point $\mathcal L^{u-a}c$ lies in $Y$, so some $0\leq n\leq D$ satisfies $\mathcal L^{u-a+n}c\in V$. The prescribed word therefore occurs at positions $[u+n,u+n+\ell-1]$, entirely inside $[u,u+D+\ell-1]$. Taking $M=D+\ell$ proves the bounded-gaps property for every interval of length at least $M$.

Conversely suppose $c$ is [uniformly recurrent](../../../dynamical-systems.md#uniform-recurrence). Every finite word from any [integer](../../../number-theory.md#integer) translate of $c$ occurs arbitrarily far to the right, so every such translate belongs to $Y$. Moreover, the property that every length-$M$ block contains a specified word of $c$ passes to every $z\in Y$: a finite block of $z$ is a limit of blocks of forward translates of $c$, and the finite discrete [alphabet](../../../information-theory.md#alphabet) forces eventual exact agreement on that block. Given $I=[a,b]\cap\mathbb Z$, look for its word inside $z([a,a+M-1])$. An occurrence starts at $a+n$ for some $n\geq0$, so $\mathcal L^n z$ agrees with $c$ on $I$. Taking $I=[-r,r]\cap\mathbb Z$ for arbitrarily large $r$ proves that $c$ belongs to the forward [orbit closure](../../../dynamical-systems.md#orbit-closure) of every $z\in Y$. That [closure](../../../topology.md#closure-topology) is a closed forward-invariant [subset](../../../set.md#subset) of $Y$, so it also contains every forward translate of $c$ and hence all of $Y$. Every forward [orbit](../../../dynamical-systems.md#orbit-dynamical-system) is therefore dense in $Y$, proving

$$
\boxed{c\text{ is a minimal point}\iff c\text{ is uniformly recurrent}.}
$$

The same conclusion holds if [orbit closure](../../../dynamical-systems.md#orbit-closure) is defined using all [integer](../../../number-theory.md#integer) iterates: the bounded-gaps condition makes the forward and two-sided closures equal.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The [dynamical proof of Hindman's theorem](../../../ramsey-theory.md#dynamical-proof-of-hindman-s-theorem) gives the following result. The [Hindman theorem](../../../ramsey-theory.md#hindman-theorem) asserts that every [finite coloring](../../../ramsey-theory.md#finite-coloring) of the [positive integers](../../../number-theory.md#positive-integer) admits an infinite strictly increasing [sequence](../../../real-analysis.md#sequence) $(a_i)$ for which all nonempty finite sums of distinct terms have one color. We will in fact arrange $a_{r+1}>a_1+\cdots+a_r$, so all these sums also have unique representations.

Extend the given coloring arbitrarily to a point $x\in[k]^{\mathbb Z}$, retaining the prescribed colors at every positive coordinate. Let $X$ be its forward [orbit closure](../../../dynamical-systems.md#orbit-closure) under the [left shift](../../../dynamical-systems.md#left-shift). The [product topology](../../../geometry-and-topology.md#product-topology) makes $X$ a [compact metric space](../../../topological-analysis.md#compact-metric-space), and the [left shift](../../../dynamical-systems.md#left-shift) is a [continuous map](../../../topology.md#continuous-map). There is a nonempty [minimal subsystem](../../../dynamical-systems.md#minimal-subsystem) $Y\subseteq X$: order the nonempty closed forward-invariant [subsets](../../../set.md#subset) by reverse inclusion, use [compactness](../../../topology.md#compact-space) and the [finite intersection property](../../../topology.md#finite-intersection-property) to intersect any chain, and apply the [Zorn lemma](../../../set-theory.md#zorn-s-lemma). Minimality also implies $\mathcal L(Y)=Y$. The result permitted in the question now supplies a [minimal point](../../../dynamical-systems.md#minimal-point) $y\in Y$ [proximal](../../../dynamical-systems.md#proximality) to $x$.

We need the [joint return lemma for a proximal minimal pair](../../../dynamical-systems.md#joint-return-lemma-for-a-proximal-minimal-pair), which we prove here. It suffices to consider an open [neighborhood](../../../topology.md#neighbourhood-mathematics) $U$ of $y$ in $X$. Choose an open [neighborhood](../../../topology.md#neighbourhood-mathematics) $V$ of $y$ with $\overline V\subseteq U$. Every forward [orbit](../../../dynamical-systems.md#orbit-dynamical-system) in $Y$ meets $V$, and a finite subcover of $\{\mathcal L^{-j}V:j\geq0\}$ on $Y$ supplies a bound $J$ on the needed return index. For a [compatible metric](../../../topological-analysis.md#compatible-metric) $d$, choose $\eta>0$ smaller than the distance from $\overline V$ to $X\setminus U$ when the latter is nonempty. By [uniform continuity](../../../topological-analysis.md#uniform-continuity) of the finitely many maps $\mathcal L^j$, $0\leq j\leq J$, some $\delta>0$ ensures

$$
d(z,z')<\delta\ \Longrightarrow
d(\mathcal L^jz,\mathcal L^jz')<\eta\quad(0\leq j\leq J).
$$

[Proximality](../../../dynamical-systems.md#proximality) supplies arbitrarily large $t$ with $d(\mathcal L^t x,\mathcal L^t y)<\delta$. To see that the times can be large under the definition using an infimum over $t\geq0$, either $x=y$, in which case this is automatic, or injectivity of the [left shift](../../../dynamical-systems.md#left-shift) makes every finite collection of distances strictly positive, so a sufficiently smaller [proximal](../../../dynamical-systems.md#proximality) distance occurs beyond that collection. Some $j\leq J$ has $\mathcal L^{t+j}y\in V$. Then $\mathcal L^{t+j}x\in U$ also. Hence arbitrarily large positive $n$ satisfy

$$
\mathcal L^n x\in U,\qquad \mathcal L^n y\in U.
$$

This uses the [minimal point](../../../dynamical-systems.md#minimal-point) property for bounded returns and [proximality](../../../dynamical-systems.md#proximality) for closeness; closeness alone would not guarantee a return near $y$.

Put $q=y(0)$. Inductively, let $F_r=\{0\}\cup\operatorname{FS}(a_1,\ldots,a_r)$, where $\operatorname{FS}$ denotes the [finite-sums set](../../../ramsey-theory.md#finite-sums-set), and maintain

$$
y(s)=q\quad(s\in F_r),\qquad x(s)=q\quad(s\in F_r\setminus\{0\}).
$$

The initial condition at $r=0$ is just $y(0)=q$; no condition on $x(0)$ is required. The [cylinder set](../../../geometry-and-topology.md#cylinder-set) $U_r=\{z:z(s)=q\text{ for every }s\in F_r\}$ is a [neighborhood](../../../topology.md#neighbourhood-mathematics) of $y$. Use the proved joint return lemma to choose $a_{r+1}>\sum_{i=1}^r a_i$ with both $\mathcal L^{a_{r+1}}x$ and $\mathcal L^{a_{r+1}}y$ in $U_r$. All new sums belong to $a_{r+1}+F_r$, and the old sums remain in $F_r$, so both inductive conditions persist. Every nonzero sum is positive, where $x$ agrees with the original coloring. Therefore

$$
\boxed{\chi(s)=q\quad\text{for every }s\in\operatorname{FS}(a_1,a_2,\ldots).}
$$

This proves the [Hindman theorem](../../../ramsey-theory.md#hindman-theorem) using only the permitted proximal-minimal existence result and the [compactness](../../../topology.md#compact-space) and return arguments supplied above.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Let $x(j)=1$ for every $j\in\mathbb Z$, and let $y$ differ from $x$ only at $j=0$, where $y(0)=2$. Under the [left shift](../../../dynamical-systems.md#left-shift), the unique defect of $\mathcal L^n y$ lies at coordinate $-n$. Every fixed finite coordinate set eventually avoids the defect, so

$$
\mathcal L^n x=x\longrightarrow x,\qquad \mathcal L^n y\longrightarrow x
$$

in the [product topology](../../../geometry-and-topology.md#product-topology). If a [metric](../../../topological-analysis.md#metric) $d$ induces this topology, convergence and the [triangle inequality](../../../topological-analysis.md#triangle-inequality) imply $d(\mathcal L^n x,\mathcal L^n y)\to0$. But [left shift](../../../dynamical-systems.md#left-shift) invariance would give

$$
d(\mathcal L^n x,\mathcal L^n y)=d(x,y)>0
$$

for every $n$, a contradiction. Thus **no [compatible metric](../../../topological-analysis.md#compatible-metric) invariant under the [left shift](../../../dynamical-systems.md#left-shift) exists**. The discrete [metric](../../../topological-analysis.md#metric) $\mathbf1_{\{x\ne y\}}$ is shift invariant, but it induces the [discrete topology](../../../topology.md#discrete-space) rather than the [product topology](../../../geometry-and-topology.md#product-topology); compatibility is the essential restriction.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
