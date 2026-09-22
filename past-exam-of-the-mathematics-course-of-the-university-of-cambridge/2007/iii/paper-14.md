# Paper 14

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper14.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper14.pdf)

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
  - [Solution](#2/solution)
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

## 1

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Let $c:\mathbb N\to\{1,\ldots,r\}$ be the given [finite colouring](../../../ramsey-theory.md#finite-coloring), with $\mathbb N=\{1,2,\ldots\}$. Give each unordered pair $\{a,b\}$ the colour $c(a+b)$. The infinite [Ramsey theorem for r-sets](../../../ramsey-theory.md#ramsey-s-theorem), in its two-element case, gives an infinite [homogeneous set for a colouring](../../../ramsey-theory.md#homogeneous-set-for-a-colouring) $X$. Enumerate it as $x_1<x_2<\cdots$. Every distinct-index sum $x_i+x_j$ has the common pair colour, so

$$
\boxed{\{x_i+x_j:i\ne j\}\text{ is monochromatic}.}
$$

This application of the infinite [Ramsey theorem for r-sets](../../../ramsey-theory.md#ramsey-s-theorem) uses only unordered pairs.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For the [finite colouring](../../../ramsey-theory.md#finite-coloring) $c$, colour each unordered pair $\{a,b\}$, written with $a<b$, by $c(a+2b)$. The infinite [Ramsey theorem for r-sets](../../../ramsey-theory.md#ramsey-s-theorem) again gives an infinite [homogeneous set for a colouring](../../../ramsey-theory.md#homogeneous-set-for-a-colouring). If its increasing enumeration is $x_1<x_2<\cdots$, then

$$
\boxed{\{x_i+2x_j:i<j\}\text{ is monochromatic}.}
$$

The ordering in this pair colouring is essential: it assigns the coefficient $2$ to the larger member.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Use the [alternating dyadic colouring excludes symmetric weighted pair sums](../../../real-analysis.md#alternating-dyadic-colouring-excludes-symmetric-weighted-pair-sums) construction:

$$
\boxed{c(n)=\lfloor\log_2 n\rfloor\pmod2.}
$$

Thus consecutive [dyadic intervals](../../../real-analysis.md#dyadic-interval) $[2^k,2^{k+1})$ have opposite colours. Suppose an increasing infinite [sequence](../../../real-analysis.md#sequence) $X=(x_j)$ had all its distinct-index weighted sums in one [colour class](../../../ramsey-theory.md#colour-class). [Set](../../../set.md) $\delta(y)=2^{\lfloor\log_2 y\rfloor+1}-y$, the distance to the next strictly larger power of $2$.

If $\delta$ is unbounded on $X$, fix a term $x$ and choose a later term $y>2x$ with $\delta(y)>2x$. Put $L=2^{\lfloor\log_2 y\rfloor}$, so $y=2L-\delta(y)$. Then

$$
L\le y+2x<2L,\qquad 2L\le2y+x=4L-2\delta(y)+x<4L.
$$

These two weighted sums lie in adjacent [dyadic intervals](../../../real-analysis.md#dyadic-interval) and therefore have opposite colours.

If $\delta$ is bounded by $D$ on $X$, choose a term $x>2D$ and a later term $y>2x$. With the same $L$, we have

$$
2L<y+2x=2L-\delta(y)+2x<4L,
\qquad
4L<2y+x=4L-2\delta(y)+x<8L.
$$

For the upper bounds, $y+2x<2y<4L$ and $2y+x<\tfrac52y<5L<8L$. These weighted sums also lie in adjacent [dyadic intervals](../../../real-analysis.md#dyadic-interval). In both cases they are $x_i+2x_j$ and $x_j+2x_i$ for two distinct indices, contradicting the common [colour class](../../../ramsey-theory.md#colour-class). Hence **the symmetric distinct-index conclusion is false**, even for this two-colour [finite colouring](../../../ramsey-theory.md#finite-coloring).

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Every [ultrafilter](../../../set-theory.md#ultrafilter) contains exactly one cell of any finite [set partition](../../../combinatorics.md#set-partition). Indeed, two disjoint cells cannot both belong to a proper [filter](../../../set-theory.md#filter-set-theory), while if none belonged to the [ultrafilter](../../../set-theory.md#ultrafilter), all their complements would belong to it and their finite [intersection](../../../set.md#set-intersection) would be empty.

Apply this property to the two [colour classes](../../../ramsey-theory.md#colour-class) in (iii). One belongs to any proposed [ultrafilter](../../../set-theory.md#ultrafilter), but neither contains a symmetric weighted-pair configuration from an increasing infinite [sequence](../../../real-analysis.md#sequence). This contradicts the proposed property of every member. Therefore **no such [ultrafilter](../../../set-theory.md#ultrafilter) exists**.

## 2

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

[Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem) says that for every pair of positive [integers](../../../number-theory.md#integer) $r,k$ there is $W(r,k)$ such that every [finite colouring](../../../ramsey-theory.md#finite-coloring) of $[W(r,k)]=\{1,\ldots,W(r,k)\}$ using at most $r$ colours contains a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [arithmetic progression](../../../arithmetic.md#arithmetic-progression) of length $k$ and positive [common difference](../../../arithmetic.md#common-difference). Consequently every [finite colouring](../../../ramsey-theory.md#finite-coloring) of $\mathbb N$ contains arbitrarily long [monochromatic](../../../ramsey-theory.md#monochromatic-set) [arithmetic progressions](../../../arithmetic.md#arithmetic-progression).

Here is a [colour-focusing proof of Van der Waerden theorem](../../../ramsey-theory.md#colour-focusing-proof-of-van-der-waerden-theorem). Induct on $k$, simultaneously for all $r$. For $k=1$, take $W(r,1)=1$. Suppose $W(R,k)$ exists for every number of colours $R$, and fix $r$. We will construct finite bounds $F_t$, $1\le t\le r$, with the following property: every [finite colouring](../../../ramsey-theory.md#finite-coloring) of $[F_t]$ using at most $r$ colours contains either a [monochromatic](../../../ramsey-theory.md#monochromatic-set) length-$(k+1)$ [arithmetic progression](../../../arithmetic.md#arithmetic-progression), or $t$ length-$k$ [arithmetic progressions](../../../arithmetic.md#arithmetic-progression) of pairwise distinct colours, all focused at the same point $f\in[F_t]$. Specifically, their terms are

$$
f-d_i,f-2d_i,\ldots,f-kd_i,\qquad d_i>0,\quad 1\le i\le t.
$$

“Focused” means that adjoining $f$ completes the corresponding length-$(k+1)$ [arithmetic progression](../../../arithmetic.md#arithmetic-progression) if $f$ has its colour.

For $t=1$, put $F_1=2W(r,k)$. Find a [monochromatic](../../../ramsey-theory.md#monochromatic-set) length-$k$ [arithmetic progression](../../../arithmetic.md#arithmetic-progression) in the first $W(r,k)$ points. Its next point is at most $2W(r,k)$ and supplies the focus. For $k=1$, give the selected singleton [common difference](../../../arithmetic.md#common-difference) $1$.

Suppose $F_t=N$ has been constructed. Set

$$
M=W(r^N,k),\qquad F_{t+1}=2NM.
$$

Divide $[2NM]$ into $2M$ consecutive blocks of length $N$. Colour the first $M$ block indices by their full [colour profiles](../../../ramsey-theory.md#colour-profile-of-a-finite-block), that is, the ordered list of their $N$ colours. There are at most $r^N$ profiles, so the induction hypothesis on $k$ gives equally profiled blocks with indices

$$
j_0,j_0+D,\ldots,j_0+(k-1)D.
$$

When $k=1$, choose $D=1$. Otherwise $D>0$ and $j_0+kD\le2M$, since the last selected block is at most $M$ and $D\le M$.

Assume the original [finite colouring](../../../ramsey-theory.md#finite-coloring) contains no [monochromatic](../../../ramsey-theory.md#monochromatic-set) length-$(k+1)$ [arithmetic progression](../../../arithmetic.md#arithmetic-progression). Applying the property of $F_t$ to the common profile gives $t$ focused length-$k$ [arithmetic progressions](../../../arithmetic.md#arithmetic-progression) at a position $f$, with [common differences](../../../arithmetic.md#common-difference) $d_i$ and distinct colours $q_i$. The colour $q$ of position $f$ differs from every $q_i$: otherwise the profile already contains a length-$(k+1)$ [monochromatic](../../../ramsey-theory.md#monochromatic-set) [arithmetic progression](../../../arithmetic.md#arithmetic-progression), and so does any selected block.

Put $j_*=j_0+kD$ and $F=N(j_*-1)+f$, a point in the original interval. For $1\le h\le k$, the point

$$
F-h(ND+d_i)=N(j_*-hD-1)+(f-hd_i)
$$

lies in a selected block at profile position $f-hd_i$, so has colour $q_i$. Similarly $F-hND$ has colour $q$. Thus $t+1$ length-$k$ [arithmetic progressions](../../../arithmetic.md#arithmetic-progression) of distinct colours focus at $F$. This proves the step in $t$. At $t=r$, the focus necessarily has the colour of one of the $r$ progressions, giving a [monochromatic](../../../ramsey-theory.md#monochromatic-set) length-$(k+1)$ [arithmetic progression](../../../arithmetic.md#arithmetic-progression). Hence $W(r,k+1)$ exists, completing the [mathematical induction](../../../foundations-of-mathematics.md#mathematical-induction) and the proof of [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem).

For the [partition regularity](../../../ramsey-theory.md#partition-regular-matrix) deduction we first prove a strengthened progression lemma, the [Brauer progression theorem](../../../ramsey-theory.md#brauer-progression-theorem): for positive $r,s,L$ with $L\ge2$, there is $B(r,s,L)$ such that every [finite colouring](../../../ramsey-theory.md#finite-coloring) of $[B(r,s,L)]$ using at most $r$ colours contains a [monochromatic set](../../../ramsey-theory.md#monochromatic-set)

$$
\{sd,a,a+d,\ldots,a+(L-1)d\},\qquad a,d>0.
$$

Induct on $r$. For $r=1$, take $B(1,s,L)=\max(s,L)$ and $a=d=1$. Given the result for $r-1$, put

$$
N=B(r-1,s,L),\qquad K=(L-1)N+1,\qquad W=W(r,K),\qquad B(r,s,L)=\max(W,sNW).
$$

[Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem) supplies a colour-$q$ [arithmetic progression](../../../arithmetic.md#arithmetic-progression) $a+j d_0$, $0\le j<K$, inside $[W]$. If some $sjd_0$, $1\le j\le N$, also has colour $q$, take $d=jd_0$ and use the $L$ terms $a,a+jd_0,\ldots,a+(L-1)jd_0$. They are in the progression because $(L-1)j\le K-1$.

Otherwise the [integers](../../../number-theory.md#integer) $sjd_0$, $1\le j\le N$, use at most $r-1$ colours. Colour $j\in[N]$ by the colour of $sjd_0$ and apply the induction hypothesis. It supplies a [monochromatic set](../../../ramsey-theory.md#monochromatic-set) $\{se,b,b+e,\ldots,b+(L-1)e\}$. Multiplying by $sd_0$ gives the required configuration with $a=sd_0b$ and $d=sd_0e$: its distinguished member is $s^2d_0e=sd$. All of these points are at most $sNd_0\le sNW$, so the finite bound is valid. This proves the [Brauer progression theorem](../../../ramsey-theory.md#brauer-progression-theorem) using only the just-proved [Van der Waerden theorem](../../../ramsey-theory.md#van-der-waerden-theorem).

A row is a [partition regular matrix](../../../ramsey-theory.md#partition-regular-matrix) over the positive [integers](../../../number-theory.md#integer) if every [finite colouring](../../../ramsey-theory.md#finite-coloring) of $\mathbb N$ admits a positive vector $x$ whose coordinates have one colour and whose product with the row is zero. Coordinates may repeat. Since the coefficients are [rational numbers](../../../number-theory.md#rational-number), multiplying them by a common positive denominator leaves the equation and every zero [subset](../../../set.md#subset) sum unchanged, so write the row as nonzero [integer](../../../number-theory.md#integer) coefficients $b_1,\ldots,b_n$.

To prove necessity, suppose no nonempty [subset](../../../set.md#subset) of the $b_i$ sums to zero. Choose a [prime](../../../number-theory.md#prime-number) $p>\sum_i|b_i|$ and use the [last nonzero digit coloring](../../../ramsey-theory.md#last-nonzero-digit-coloring)

$$
c(x)=p^{-v_p(x)}x\pmod p\ \in\mathbb F_p^{\times},
$$

where $v_p$ is the [P-adic valuation](../../../number-theory.md#p-adic-valuation). If positive $x_i$ all had the same colour $u$ and satisfied $\sum_i b_ix_i=0$, let $m=\min_i v_p(x_i)$ and $I=\{i:v_p(x_i)=m\}$. After division by $p^m$ and reduction modulo $p$, the equation becomes

$$
u\sum_{i\in I}b_i=0\quad\text{in }\mathbb F_p.
$$

As $u\ne0$, this says $p\mid\sum_{i\in I}b_i$. The latter sum is nonzero and has absolute value at most $\sum_i|b_i|<p$, a contradiction. This explicitly proves the necessary obstruction without invoking a general [partition regularity](../../../ramsey-theory.md#partition-regular-matrix) criterion.

Conversely, suppose $\varnothing\ne I\subseteq\{1,\ldots,n\}$ and $\sum_{i\in I}b_i=0$. Select an index $j\in I$, and put

$$
S=\sum_{i\notin I}b_i,\qquad s=|b_j|,\qquad q=-\frac{sS}{b_j}\in\mathbb Z,\qquad u=\max(0,-q),\qquad L=\max(2,|q|+1).
$$

For any [finite colouring](../../../ramsey-theory.md#finite-coloring), the [Brauer progression theorem](../../../ramsey-theory.md#brauer-progression-theorem) gives one-coloured $\{sd,a,a+d,\ldots,a+(L-1)d\}$. The indices $u$ and $u+q$ both lie between $0$ and $L-1$. Define positive, same-coloured coordinates by

$$
x_i=\begin{cases}
sd,&i\notin I,\\
a+ud,&i\in I\setminus\{j\},\\
a+(u+q)d,&i=j.
\end{cases}
$$

Then

$$
\sum_i b_ix_i=(a+ud)\sum_{i\in I}b_i+d(b_jq+sS)=0.
$$

This also covers $I$ equal to the whole index [set](../../../set.md) and $q=0$. Reversing the clearing of denominators proves the exact criterion:

$$
\boxed{(a_1,\ldots,a_n)\text{ is partition regular}\quad\Longleftrightarrow\quad
\exists\varnothing\ne I\subseteq\{1,\ldots,n\}:\ \sum_{i\in I}a_i=0.}
$$

## 3

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

An [ultrafilter](../../../set-theory.md#ultrafilter) on $\mathbb N=\{1,2,\ldots\}$ is a family $p\subseteq\mathcal P(\mathbb N)$ satisfying the proper [filter](../../../set-theory.md#filter-set-theory) axioms: $\mathbb N\in p$, $\varnothing\notin p$, [closure](../../../topology.md#closure-topology) under finite [intersections](../../../set.md#set-intersection), and upward [closure](../../../topology.md#closure-topology) under inclusion. In addition, for every $A\subseteq\mathbb N$, exactly one of $A$ and $A^c$ belongs to $p$. Equivalently, an [ultrafilter](../../../set-theory.md#ultrafilter) is a maximal proper [filter](../../../set-theory.md#filter-set-theory). The [principal ultrafilter](../../../set-theory.md#principal-ultrafilter) at $n$ consists of all [subsets](../../../set.md#subset) containing $n$; an [ultrafilter](../../../set-theory.md#ultrafilter) not of this form is a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter).

To prove existence, start with the [cofinite filter](../../../set-theory.md#cofinite-filter) and order the proper [filters](../../../set-theory.md#filter-set-theory) containing it by inclusion. The [union](../../../set.md#set-union) of a chain is still a proper [filter](../../../set-theory.md#filter-set-theory): finitely many of its members lie in one [filter](../../../set-theory.md#filter-set-theory) of the chain, and no constituent contains the empty [set](../../../set.md). Thus [Zorn lemma](../../../set-theory.md#zorn-s-lemma) supplies a maximal such [filter](../../../set-theory.md#filter-set-theory) $p$. If $A\notin p$, adjoining $A$ cannot generate a proper [filter](../../../set-theory.md#filter-set-theory); otherwise maximality fails. Consequently some $B\in p$ has $B\cap A=\varnothing$, so $A^c\in p$ by upward [closure](../../../topology.md#closure-topology). This proves the [ultrafilter](../../../set-theory.md#ultrafilter) alternative. No finite $A$ can belong to $p$, because $A^c$ is [cofinite](../../../set-theory.md#cofinite-set) and already belongs to $p$. In particular $p$ contains no singleton and is a **[nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter)**. The same argument, starting from any proper [filter](../../../set-theory.md#filter-set-theory), proves the [ultrafilter lemma](../../../set-theory.md#ultrafilter-lemma) used below.

Define $\beta\mathbb N$ to be the [set](../../../set.md) of all [ultrafilters](../../../set-theory.md#ultrafilter) on $\mathbb N$, with basic [open sets](../../../topology.md#open-set)

$$
\widehat A=\{p\in\beta\mathbb N:A\in p\},\qquad A\subseteq\mathbb N.
$$

They form a [topological basis](../../../topology.md#basis-of-a-topology) because $\widehat{\mathbb N}=\beta\mathbb N$ and $\widehat A\cap\widehat B=\widehat{A\cap B}$. Moreover $(\widehat A)^c=\widehat{A^c}$, so they are [clopen sets](../../../topology.md#clopen-set). This is the [compact Hausdorff topology on ultrafilters](../../../set-theory.md#compact-hausdorff-topology-on-ultrafilters). If $p\ne q$, some $A$ belongs to $p$ but not $q$, and then $\widehat A$ and $\widehat{A^c}$ are disjoint open [neighbourhoods](../../../topology.md#neighbourhood-mathematics) of the two points. Thus $\beta\mathbb N$ is [Hausdorff](../../../topology.md#hausdorff-space).

For [compactness](../../../topology.md#compact-space), take an [open cover](../../../topology.md#open-cover) and refine it by basic [open sets](../../../topology.md#open-set) $\widehat{A_\lambda}$. If no finite subfamily covers, then for every finite collection of indices the [intersection](../../../set.md#set-intersection) $\bigcap A_\lambda^c$ is nonempty. Indeed, if that [intersection](../../../set.md#set-intersection) were empty, the corresponding $A_\lambda$ would cover $\mathbb N$, and every [ultrafilter](../../../set-theory.md#ultrafilter) would contain at least one of them by the finite [ultrafilter](../../../set-theory.md#ultrafilter) alternative. The complements therefore have the [finite intersection property](../../../topology.md#finite-intersection-property) and generate a proper [filter](../../../set-theory.md#filter-set-theory). Extend it to an [ultrafilter](../../../set-theory.md#ultrafilter) $q$ by the proved [ultrafilter lemma](../../../set-theory.md#ultrafilter-lemma). Then $A_\lambda^c\in q$ for every $\lambda$, so $q$ belongs to none of the covering $\widehat{A_\lambda}$, a contradiction. A finite basic subcover lies inside a finite subcover of the original cover. Hence

$$
\boxed{\beta\mathbb N\text{ is compact and Hausdorff}.}
$$

The map $n\mapsto p_n$, where $p_n$ is the [principal ultrafilter](../../../set-theory.md#principal-ultrafilter) at $n$, identifies the discrete natural numbers with a [dense subset](../../../topology.md#dense-set): any nonempty $\widehat A$ has $A\ne\varnothing$ and contains $p_n$ for $n\in A$.

[Hindman theorem](../../../ramsey-theory.md#hindman-theorem) states that every [finite colouring](../../../ramsey-theory.md#finite-coloring) of the positive [integers](../../../number-theory.md#integer) admits an increasing [sequence](../../../real-analysis.md#sequence) $x_1<x_2<\cdots$ whose [finite-sums set](../../../ramsey-theory.md#finite-sums-set)

$$
FS(x_1,x_2,\ldots)=\left\{\sum_{i\in F}x_i:\varnothing\ne F\subseteq\mathbb N\text{ finite}\right\}
$$

is [monochromatic](../../../ramsey-theory.md#monochromatic-set). We now give the [Idempotent-ultrafilter proof of Hindman's theorem](../../../ramsey-theory.md#idempotent-ultrafilter-proof-of-hindman-s-theorem). For $A\subseteq\mathbb N$, write $A-x=\{y\in\mathbb N:x+y\in A\}$. The addition on $\beta\mathbb N$ is defined by

$$
A\in p+q\quad\Longleftrightarrow\quad\{x\in\mathbb N:A-x\in q\}\in p.
$$

Take an [idempotent ultrafilter on the natural numbers](../../../set-theory.md#idempotent-ultrafilter-on-the-natural-numbers) $p$, whose existence is allowed, so $p+p=p$. It is a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter): addition of principal points is $p_m+p_n=p_{m+n}$, whereas no positive [integer](../../../number-theory.md#integer) satisfies $2m=m$.

Exactly one [colour class](../../../ramsey-theory.md#colour-class) $A$ belongs to $p$. Define

$$
A^*=A\cap\{x:A-x\in p\}.
$$

By idempotence, $A^*\in p$. The [idempotent-ultrafilter star-set lemma](../../../set-theory.md#idempotent-ultrafilter-star-set-lemma) needed for the recursion is that $A^*-x\in p$ whenever $x\in A^*$. To prove it, put $D=A-x\in p$. Idempotence again gives

$$
D^*=D\cap\{y:D-y\in p\}\in p.
$$

For $y\in D^*$, we have $x+y\in A$ and $A-(x+y)=D-y\in p$, hence $x+y\in A^*$. Thus $D^*\subseteq A^*-x$, proving the lemma by upward [closure](../../../topology.md#closure-topology).

Choose $x_1\in A^*$. Suppose $F_n=FS(x_1,\ldots,x_n)\subseteq A^*$ has been constructed. Every factor of

$$
A^*\cap\bigcap_{s\in F_n}(A^*-s)\cap\left\{z:z>\sum_{i=1}^nx_i\right\}
$$

belongs to $p$: the translate factors do by the just-proved lemma, and the last factor does because it is [cofinite](../../../set-theory.md#cofinite-set) and $p$ is a [nonprincipal ultrafilter](../../../set-theory.md#nonprincipal-ultrafilter). The finite [intersection](../../../set.md#set-intersection) is therefore nonempty. Choose $x_{n+1}$ in it. Then $x_{n+1}$ and every $s+x_{n+1}$ with $s\in F_n$ lie in $A^*$, so $F_{n+1}\subseteq A^*$. This constructs a strictly increasing [sequence](../../../real-analysis.md#sequence), indeed $x_{n+1}>\sum_{i\le n}x_i$, and proves [Hindman theorem](../../../ramsey-theory.md#hindman-theorem).

Finally apply [Hindman theorem](../../../ramsey-theory.md#hindman-theorem) to obtain a [monochromatic](../../../ramsey-theory.md#monochromatic-set) [finite-sums set](../../../ramsey-theory.md#finite-sums-set) $FS(y_1,y_2,\ldots)$. We construct a [divisibility chain inside a finite-sums set](../../../ramsey-theory.md#divisibility-chain-inside-a-finite-sums-set) using disjoint successive blocks of indices. Start with $x_1=y_1$. If $x_i=m$, take $2m$ unused terms after all indices used so far, and split them into two groups of $m$ consecutive terms. In each group its $m+1$ [partial sums](../../../real-analysis.md#partial-sum), including $0$, contain two in the same [congruence class](../../../number-theory.md#congruence-class) modulo $m$ by the [pigeonhole principle](../../../algebra.md#pigeonhole-principle). Their difference is a nonempty consecutive sum divisible by $m$, and positivity makes it at least $m$. Let $x_{i+1}$ be the sum of these two selected sums. Then $m\mid x_{i+1}$ and $x_{i+1}\ge2m>m$.

The index [set](../../../set.md) defining $x_{i+1}$ lies strictly after all previous index [sets](../../../set.md). Discard the other terms in these two groups before continuing. Because the chosen index [sets](../../../set.md) are disjoint, every finite sum of distinct $x_i$ is a finite sum of distinct $y_j$, retaining the same colour. Therefore

$$
\boxed{x_1<x_2<\cdots,\qquad x_i\mid x_{i+1}\ \text{for every }i,\qquad FS(x_1,x_2,\ldots)\text{ is monochromatic}.}
$$

## 4

↑ **Parent:** [Paper 14](paper-14.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Write $[M]^\omega$ for the [set](../../../set.md) of all infinite [subsets](../../../set.md#subset) of $M$. A family $Y\subseteq[\mathbb N]^\omega$ is a [Ramsey family in the homogeneous-cone sense](../../../ramsey-theory.md#ramsey-family-in-the-homogeneous-cone-sense) if there is an infinite $M$ such that either $[M]^\omega\subseteq Y$ or $[M]^\omega\cap Y=\varnothing$. Thus membership in $Y$ is constant on an infinite homogeneous cone. We will prove the stronger version for open families: such a cone exists inside every prescribed infinite ground [set](../../../set.md), as in the definition of a [Ramsey set of infinite subsets](../../../ramsey-theory.md#ramsey-set-of-infinite-subsets).

The symbols in the question refer to the [ordinary topology on infinite subsets](../../../ramsey-theory.md#ordinary-topology-on-infinite-subsets) $\tau$ and the [Ellentuck topology](../../../ramsey-theory.md#ellentuck-topology) $*$. For a [finite set](../../../set.md#finite-set) $s$, let

$$
[s]=\{X\in[\mathbb N]^\omega:s\text{ is the initial segment of }X\}.
$$

These [sets](../../../set.md) form a [topological basis](../../../topology.md#basis-of-a-topology) for $\tau$, equivalently the [subspace topology](../../../topology.md#subspace-topology) inherited from the [product topology](../../../geometry-and-topology.md#product-topology) on $\{0,1\}^{\mathbb N}$. For an infinite $A$ with $\max s<\min A$, the [sets](../../../set.md)

$$
[s,A]=\{s\cup B:B\in[A]^\omega\}
$$

form a [topological basis](../../../topology.md#basis-of-a-topology) for $*$; take $\max\varnothing=0$. In particular $[s]=[s,\{n:n>\max s\}]$, so $*$ is finer than $\tau$.

For a non-Ramsey example use the [finite-symmetric-difference parity colouring](../../../ramsey-theory.md#finite-symmetric-difference-parity-colouring). On $[\mathbb N]^\omega$, define the [equivalence relation](../../../set-theory.md#equivalence-relation) $X\sim Z$ if their [symmetric difference](../../../set.md#symmetric-difference) $X\mathbin\triangle Z$ is finite. By the [axiom of choice](../../../set-theory.md#axiom-of-choice), select a representative $R$ in every [equivalence class](../../../set-theory.md#equivalence-class). Give $X$ the colour

$$
c(X)=|X\mathbin\triangle R_X|\pmod2,
$$

where $R_X$ is its class representative. Deleting one point stays in the same class and toggles the parity. Thus for every infinite $M$, the [sets](../../../set.md) $M$ and $M\setminus\{\min M\}$ are both in $[M]^\omega$ but have opposite colours. Either [colour class](../../../ramsey-theory.md#colour-class), regarded as a family $Y$, is therefore **not Ramsey**.

Now let $U$ be $\tau$-open. We prove that for every infinite $A_0$ there is an infinite $C\subseteq A_0$ with $[C]^\omega\subseteq U$ or $[C]^\omega\cap U=\varnothing$. The proof uses [acceptance and rejection of finite stems](../../../ramsey-theory.md#acceptance-and-rejection-of-finite-stems), which we define explicitly. For a [finite stem](../../../ramsey-theory.md#finite-stem-of-an-infinite-subset) $s$ and an infinite tail $A$ above $\max s$, say that $A$ accepts $s$ if $[s,A]\subseteq U$, and rejects $s$ if no infinite [subset](../../../set.md#subset) of $A$ accepts $s$. Both properties persist on taking infinite [subsets](../../../set.md#subset). Every tail has an infinite [subset](../../../set.md#subset) that decides $s$: take an accepting [subset](../../../set.md#subset) if one exists, and otherwise it already rejects $s$.

First thin $A_0$ to decide the empty stem. Then construct $b_1<b_2<\cdots$ and nested infinite tails. At step $n$, choose $b_n$ from the current tail, discard its points at most $b_n$, and successively thin what remains to decide every stem $s\subseteq\{b_1,\ldots,b_n\}$. There are only finitely many such stems, so an infinite tail remains. Let $B=\{b_1,b_2,\ldots\}$ and write $B/s=\{b\in B:b>\max s\}$. For every finite $s\subseteq B$, the tail $B/s$ decides $s$, since it lies in the tail obtained at the stage when the largest point of $s$ was selected. The empty stem is also decided. This is [deciding all finite stems by fusion](../../../ramsey-theory.md#deciding-all-finite-stems-by-fusion).

If $B$ accepts the empty stem, then $[B]^\omega\subseteq U$, as required. Otherwise $B$ rejects it. We need the [finitely many accepting extensions of a rejected stem](../../../ramsey-theory.md#finitely-many-accepting-extensions-of-a-rejected-stem) observation. Suppose a tail $B/s$ rejects $s$. Only finitely many $a\in B/s$ can have $B/a$ accepting $s\cup\{a\}$. Indeed, if infinitely many such $a$ formed a [set](../../../set.md) $D$, every member of $[s,D]$ would have some first new point $a$ and all later points in $B/a$, hence would lie in $U$. This would make $D$ an accepting [subset](../../../set.md#subset) of $B/s$, contradicting rejection.

Choose $c_1<c_2<\cdots$ in $B$ recursively so that for every finite $s\subseteq\{c_1,\ldots,c_n\}$, the tail $B/s$ rejects $s$. The empty stem satisfies this initially. At the next step, each of the finitely many previous stems has only finitely many accepting one-point extensions by the observation. Choose $c_{n+1}$ larger than all previous points and outside all those finite exceptional [sets](../../../set.md). The first fusion ensured that the tail for every new stem decides it; since it does not accept it, it rejects it. This maintains the recursion.

Put $C=\{c_1,c_2,\ldots\}$. If some $X\in[C]^\omega$ belonged to $U$, ordinary openness would give a finite initial segment $s$ of $X$ with $[s]\subseteq U$. In particular $[s,C/s]\subseteq U$. But $C/s$ is an infinite [subset](../../../set.md#subset) of $B/s$, which rejects $s$, a contradiction. Hence $[C]^\omega\cap U=\varnothing$. We have proved

$$
\boxed{\text{Every }\tau\text{-open family is Ramsey, even inside every infinite ground set}.}
$$

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Take the [cone on an infinite coinfinite ground set](../../../ramsey-theory.md#cone-on-an-infinite-coinfinite-ground-set)

$$
\boxed{E=[2\mathbb N]^\omega.}
$$

It is $*$-open because $E=[\varnothing,2\mathbb N]$ is a basic [open set](../../../topology.md#open-set) of the [Ellentuck topology](../../../ramsey-theory.md#ellentuck-topology). It is not $\tau$-open: if $X\in E$, every ordinary basic [neighbourhood](../../../topology.md#neighbourhood-mathematics) $[s]$ of $X$ contains an infinite extension of $s$ having an odd point larger than $\max s$. That extension is outside $E$. Therefore no point of $E$ has an ordinary open [neighbourhood](../../../topology.md#neighbourhood-mathematics) contained in $E$.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The same [cone on an infinite coinfinite ground set](../../../ramsey-theory.md#cone-on-an-infinite-coinfinite-ground-set) works:

$$
\boxed{E=[2\mathbb N]^\omega.}
$$

It is $\tau$-closed: a [set](../../../set.md) outside $E$ has an odd point, and the ordinary [neighbourhood](../../../topology.md#neighbourhood-mathematics) given by its initial segment through that point remains outside $E$. Its $\tau$-[interior](../../../topology.md#interior-topology) is empty, since every ordinary basic [open set](../../../topology.md#open-set) admits an extension having an odd point. Hence its ordinary [closure](../../../topology.md#closure-topology) equals itself and has empty [interior](../../../topology.md#interior-topology), proving that it is a $\tau$-[nowhere dense set](../../../topological-analysis.md#nowhere-dense-set).

In the [Ellentuck topology](../../../ramsey-theory.md#ellentuck-topology), however, $E$ is itself a nonempty [open set](../../../topology.md#open-set). Its $*$-[closure](../../../topology.md#closure-topology) therefore has nonempty $*$-[interior](../../../topology.md#interior-topology), so $E$ is **not $*$-nowhere dense**.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Let

$$
\boxed{D=\{X\subseteq\mathbb N:X\text{ is cofinite}\}.}
$$

This is the [dense countable family of cofinite infinite subsets](../../../ramsey-theory.md#dense-countable-family-of-cofinite-infinite-subsets). Every ordinary basic [open set](../../../topology.md#open-set) $[s]$ contains the [cofinite set](../../../set-theory.md#cofinite-set) $s\cup\{n:n>\max s\}$. Thus $D$ is $\tau$-dense: its ordinary [closure](../../../topology.md#closure-topology) is the whole space, so it is **not $\tau$-nowhere dense**.

It is $*$-closed. Indeed, for an infinite noncofinite $X$, the [Ellentuck topology](../../../ramsey-theory.md#ellentuck-topology) [neighbourhood](../../../topology.md#neighbourhood-mathematics) $[\varnothing,X]$ contains only noncofinite [sets](../../../set.md), because every [subset](../../../set.md#subset) of $X$ misses the infinite [complement](../../../set.md#complement-of-a-set) of $X$. This [neighbourhood](../../../topology.md#neighbourhood-mathematics) is disjoint from $D$.

Finally every nonempty basic $*$-[open set](../../../topology.md#open-set) $[s,A]$ contains a smaller basic $*$-[open set](../../../topology.md#open-set) disjoint from $D$: enumerate $A$ and let $B$ consist of every second point. Then $A\setminus B$ is infinite, and $[s,B]\subseteq[s,A]$ contains no [cofinite set](../../../set-theory.md#cofinite-set). In particular $D$ has empty $*$-[interior](../../../topology.md#interior-topology). As it is already $*$-closed, its $*$-[closure](../../../topology.md#closure-topology) has empty $*$-[interior](../../../topology.md#interior-topology), proving that it is **$*$-nowhere dense**.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
