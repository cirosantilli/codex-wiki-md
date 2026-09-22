<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Van der Waerden theorem.** Given [positive integers](../../../../../positive-integer.md) $r,k$, there is a finite $W(r,k)$ such that every [finite colouring](../../../../../finite-coloring.md) of $\{1,\ldots,W(r,k)\}$ with at most $r$ colours has a [monochromatic](../../../../../monochromatic-set.md) [arithmetic progression](../../../../../arithmetic-progression.md) of length $k$ and positive [common difference](../../../../../common-difference.md). In particular, every [finite colouring](../../../../../finite-coloring.md) of the [positive integers](../../../../../positive-integer.md) contains such progressions of every finite length.

Here is a [colour-focusing proof of Van der Waerden theorem](../../../../../colour-focusing-proof-of-van-der-waerden-theorem.md). We induct on $k$, simultaneously for all numbers of colours. The assertion for $k=1$ is immediate. Suppose $W(r,k)$ exists for every $r$, and fix $r$. We construct bounds $F_t$, for $1\le t\le r$, with this property: every colouring of $[F_t]$ either has a [monochromatic](../../../../../monochromatic-set.md) progression of length $k+1$, or has $t$ progressions of length $k$, of distinct colours, which share a next point $f\in[F_t]$. Write those progressions as

$$
f-hd_i,\qquad 1\le h\le k,\quad 1\le i\le t,
$$

with positive steps $d_i$ and all displayed points in $[F_t]$.

For $t=1$, put $L=W(r,k)$ and $F_1=2L$. A [monochromatic](../../../../../monochromatic-set.md) progression of length $k$ in $[L]$ has its next point in $[2L]$, since its step is at most $L$; for $k=1$ choose step $1$. This establishes the initial focusing property.

Suppose $F_t=N$ has been constructed. Put $M=W(r^N,k)$ and $F_{t+1}=2NM$. Divide the first $NM$ integers into $M$ consecutive blocks of size $N$. Colour a block by its full [colour profile](../../../../../colour-profile-of-a-finite-block.md), an $N$-tuple having at most $r^N$ possible values. The induction hypothesis on $k$ gives block indices

$$
j_0,j_0+D,\ldots,j_0+(k-1)D
$$

with the same [colour profile](../../../../../colour-profile-of-a-finite-block.md). For $k=1$ use any one block and $D=1$. Suppose that the whole interval has no [monochromatic](../../../../../monochromatic-set.md) progression of length $k+1$. Its repeated profile has $t$ focused length-$k$ progressions with positions $f-hd_i$ and distinct colours $q_i$. The colour $q$ of position $f$ differs from every $q_i$, since equality would complete a length-$(k+1)$ progression in the block.

Set $j_*=j_0+kD$ and $F=N(j_*-1)+f$. The index $j_*$ is at most $2M$, so this focus is in the full interval. For $1\le h\le k$, the point

$$
F-h(ND+d_i)=N(j_*-hD-1)+(f-hd_i)
$$

is in one of the chosen blocks and has colour $q_i$. Also $F-hND$ is at position $f$ in that block and has colour $q$. We have produced $t+1$ focused length-$k$ progressions of distinct colours. This proves the recursive focusing property. At $t=r$, the focus itself must have one of the $r$ colours, so one of the progressions extends to length $k+1$. Thus $W(r,k+1)=F_r$ is a valid bound, completing the [mathematical induction](../../../../../mathematical-induction.md) and the requested proof.

To obtain the equation criterion, we first prove the small strengthening of [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md) that we need. For any [positive integers](../../../../../positive-integer.md) $r,s,L$, there is a finite bound forcing a [monochromatic](../../../../../monochromatic-set.md) configuration

$$
\{sd,\ b,b+d,\ldots,b+(L-1)d\},\qquad b,d>0.
$$

This is the [Brauer progression theorem](../../../../../brauer-progression-theorem.md), and the following argument proves it from the theorem just established. Induct on $r$. One colour is immediate. Given a bound $M$ for $r-1$ colours with the same $s,L$, let $T=W(r,(L-1)M+1)$ and colour an interval at least as long as $\max(T,sMT)$. Find a [monochromatic](../../../../../monochromatic-set.md) progression $a,a+d,\ldots,a+(L-1)Md$ in $[T]$, of colour $q$; take $d=1$ if this progression has one term. If some $jsd$, $1\le j\le M$, has colour $q$, its first $L$ suitably spaced terms $a,a+jd,\ldots,a+(L-1)jd$ and the point $s(jd)$ give the configuration. Otherwise the colouring of the indices $1,\ldots,M$ obtained from $j\mapsto c(jsd)$ uses at most $r-1$ colours. The induction hypothesis supplies indices $se,b,b+e,\ldots,b+(L-1)e$ of one colour. Multiplication by $sd$ gives the desired configuration with step $esd$. This completes the strengthening without assuming any [Rado theorem](../../../../../rado-s-theorem.md).

Multiply the rational coefficients by a common positive denominator, so that all $a_i$ are nonzero [integers](../../../../../integer.md); this does not alter the equation or [partition regularity](../../../../../partition-regular-matrix.md). By definition, the row is [partition regular](../../../../../partition-regular-matrix.md) when every [finite colouring](../../../../../finite-coloring.md) admits positive [monochromatic](../../../../../monochromatic-set.md) $x_1,\ldots,x_n$ satisfying $\sum_i a_ix_i=0$. The variables need not be distinct.

For necessity, choose a [prime number](../../../../../prime-number.md) $p>\sum_i|a_i|$. Write each positive $x$ uniquely as $p^{v_p(x)}u$, with $p\nmid u$, and colour $x$ by $u\bmod p$. This is a [finite colouring](../../../../../finite-coloring.md) with $p-1$ colours. If a [monochromatic](../../../../../monochromatic-set.md) solution exists, let $v=\min_i v_p(x_i)$ and $I=\{i:v_p(x_i)=v\}$. Dividing the equation by $p^v$ and reducing modulo $p$ gives

$$
0\equiv u_0\sum_{i\in I}a_i\pmod p,
$$

where $u_0\ne0\pmod p$ is the common colour. Thus $\sum_{i\in I}a_i\equiv0\pmod p$. Its absolute value is strictly less than $p$, so $\sum_{i\in I}a_i=0$. The index set $I$ is nonempty. This proves the [leading-residue obstruction to partition regularity](../../../../../leading-residue-obstruction-to-partition-regularity.md).

Conversely, suppose $\sum_{i\in I}a_i=0$ for a nonempty $I$. If $I$ is all indices, taking every variable equal to any one positive integer already gives a [monochromatic](../../../../../monochromatic-set.md) solution. Otherwise fix $i_0\in I$, put $s=|a_{i_0}|$, $C=\sum_{j\notin I}a_j$, and define integer offsets

$$
\lambda_{i_0}=-\operatorname{sgn}(a_{i_0})C,\qquad
\lambda_i=0\quad(i\in I\setminus\{i_0\}).
$$

Let $u=\min_{i\in I}\lambda_i$ and choose $L=1+\max_{i\in I}\lambda_i-u$. The proved [Brauer progression theorem](../../../../../brauer-progression-theorem.md) gives a [monochromatic](../../../../../monochromatic-set.md) configuration consisting of $sd$ and a length-$L$ progression starting at $b$. Set

$$
x_i=b+(\lambda_i-u)d\quad(i\in I),\qquad x_j=sd\quad(j\notin I).
$$

All variables are positive and of one colour. Their weighted sum is

$$
\sum_i a_ix_i=(b-ud)\sum_{i\in I}a_i+d\sum_{i\in I}a_i\lambda_i+sdC
=0-sCd+sCd=0.
$$

This explicitly gives a [Brauer configuration for a one-row zero-sum equation](../../../../../brauer-configuration-for-a-one-row-zero-sum-equation.md). We conclude

$$
\boxed{(a_1,\ldots,a_n)\text{ is partition regular}\ \Longleftrightarrow\ \exists\varnothing\ne I\subseteq[n],\ \sum_{i\in I}a_i=0.}
$$

Both directions have been proved independently of the general [Rado theorem](../../../../../rado-s-theorem.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
