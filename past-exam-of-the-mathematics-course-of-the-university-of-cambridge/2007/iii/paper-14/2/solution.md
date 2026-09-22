<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Van der Waerden theorem](../../../../../van-der-waerden-theorem.md) says that for every pair of positive [integers](../../../../../integer.md) $r,k$ there is $W(r,k)$ such that every [finite colouring](../../../../../finite-coloring.md) of $[W(r,k)]=\{1,\ldots,W(r,k)\}$ using at most $r$ colours contains a [monochromatic](../../../../../monochromatic-set.md) [arithmetic progression](../../../../../arithmetic-progression.md) of length $k$ and positive [common difference](../../../../../common-difference.md). Consequently every [finite colouring](../../../../../finite-coloring.md) of $\mathbb N$ contains arbitrarily long [monochromatic](../../../../../monochromatic-set.md) [arithmetic progressions](../../../../../arithmetic-progression.md).

Here is a [colour-focusing proof of Van der Waerden theorem](../../../../../colour-focusing-proof-of-van-der-waerden-theorem.md). Induct on $k$, simultaneously for all $r$. For $k=1$, take $W(r,1)=1$. Suppose $W(R,k)$ exists for every number of colours $R$, and fix $r$. We will construct finite bounds $F_t$, $1\le t\le r$, with the following property: every [finite colouring](../../../../../finite-coloring.md) of $[F_t]$ using at most $r$ colours contains either a [monochromatic](../../../../../monochromatic-set.md) length-$(k+1)$ [arithmetic progression](../../../../../arithmetic-progression.md), or $t$ length-$k$ [arithmetic progressions](../../../../../arithmetic-progression.md) of pairwise distinct colours, all focused at the same point $f\in[F_t]$. Specifically, their terms are

$$
f-d_i,f-2d_i,\ldots,f-kd_i,\qquad d_i>0,\quad 1\le i\le t.
$$

“Focused” means that adjoining $f$ completes the corresponding length-$(k+1)$ [arithmetic progression](../../../../../arithmetic-progression.md) if $f$ has its colour.

For $t=1$, put $F_1=2W(r,k)$. Find a [monochromatic](../../../../../monochromatic-set.md) length-$k$ [arithmetic progression](../../../../../arithmetic-progression.md) in the first $W(r,k)$ points. Its next point is at most $2W(r,k)$ and supplies the focus. For $k=1$, give the selected singleton [common difference](../../../../../common-difference.md) $1$.

Suppose $F_t=N$ has been constructed. Set

$$
M=W(r^N,k),\qquad F_{t+1}=2NM.
$$

Divide $[2NM]$ into $2M$ consecutive blocks of length $N$. Colour the first $M$ block indices by their full [colour profiles](../../../../../colour-profile-of-a-finite-block.md), that is, the ordered list of their $N$ colours. There are at most $r^N$ profiles, so the induction hypothesis on $k$ gives equally profiled blocks with indices

$$
j_0,j_0+D,\ldots,j_0+(k-1)D.
$$

When $k=1$, choose $D=1$. Otherwise $D>0$ and $j_0+kD\le2M$, since the last selected block is at most $M$ and $D\le M$.

Assume the original [finite colouring](../../../../../finite-coloring.md) contains no [monochromatic](../../../../../monochromatic-set.md) length-$(k+1)$ [arithmetic progression](../../../../../arithmetic-progression.md). Applying the property of $F_t$ to the common profile gives $t$ focused length-$k$ [arithmetic progressions](../../../../../arithmetic-progression.md) at a position $f$, with [common differences](../../../../../common-difference.md) $d_i$ and distinct colours $q_i$. The colour $q$ of position $f$ differs from every $q_i$: otherwise the profile already contains a length-$(k+1)$ [monochromatic](../../../../../monochromatic-set.md) [arithmetic progression](../../../../../arithmetic-progression.md), and so does any selected block.

Put $j_*=j_0+kD$ and $F=N(j_*-1)+f$, a point in the original interval. For $1\le h\le k$, the point

$$
F-h(ND+d_i)=N(j_*-hD-1)+(f-hd_i)
$$

lies in a selected block at profile position $f-hd_i$, so has colour $q_i$. Similarly $F-hND$ has colour $q$. Thus $t+1$ length-$k$ [arithmetic progressions](../../../../../arithmetic-progression.md) of distinct colours focus at $F$. This proves the step in $t$. At $t=r$, the focus necessarily has the colour of one of the $r$ progressions, giving a [monochromatic](../../../../../monochromatic-set.md) length-$(k+1)$ [arithmetic progression](../../../../../arithmetic-progression.md). Hence $W(r,k+1)$ exists, completing the [mathematical induction](../../../../../mathematical-induction.md) and the proof of [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md).

For the [partition regularity](../../../../../partition-regular-matrix.md) deduction we first prove a strengthened progression lemma, the [Brauer progression theorem](../../../../../brauer-progression-theorem.md): for positive $r,s,L$ with $L\ge2$, there is $B(r,s,L)$ such that every [finite colouring](../../../../../finite-coloring.md) of $[B(r,s,L)]$ using at most $r$ colours contains a [monochromatic set](../../../../../monochromatic-set.md)

$$
\{sd,a,a+d,\ldots,a+(L-1)d\},\qquad a,d>0.
$$

Induct on $r$. For $r=1$, take $B(1,s,L)=\max(s,L)$ and $a=d=1$. Given the result for $r-1$, put

$$
N=B(r-1,s,L),\qquad K=(L-1)N+1,\qquad W=W(r,K),\qquad B(r,s,L)=\max(W,sNW).
$$

[Van der Waerden theorem](../../../../../van-der-waerden-theorem.md) supplies a colour-$q$ [arithmetic progression](../../../../../arithmetic-progression.md) $a+j d_0$, $0\le j<K$, inside $[W]$. If some $sjd_0$, $1\le j\le N$, also has colour $q$, take $d=jd_0$ and use the $L$ terms $a,a+jd_0,\ldots,a+(L-1)jd_0$. They are in the progression because $(L-1)j\le K-1$.

Otherwise the [integers](../../../../../integer.md) $sjd_0$, $1\le j\le N$, use at most $r-1$ colours. Colour $j\in[N]$ by the colour of $sjd_0$ and apply the induction hypothesis. It supplies a [monochromatic set](../../../../../monochromatic-set.md) $\{se,b,b+e,\ldots,b+(L-1)e\}$. Multiplying by $sd_0$ gives the required configuration with $a=sd_0b$ and $d=sd_0e$: its distinguished member is $s^2d_0e=sd$. All of these points are at most $sNd_0\le sNW$, so the finite bound is valid. This proves the [Brauer progression theorem](../../../../../brauer-progression-theorem.md) using only the just-proved [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md).

A row is a [partition regular matrix](../../../../../partition-regular-matrix.md) over the positive [integers](../../../../../integer.md) if every [finite colouring](../../../../../finite-coloring.md) of $\mathbb N$ admits a positive vector $x$ whose coordinates have one colour and whose product with the row is zero. Coordinates may repeat. Since the coefficients are [rational numbers](../../../../../rational-number.md), multiplying them by a common positive denominator leaves the equation and every zero [subset](../../../../../subset.md) sum unchanged, so write the row as nonzero [integer](../../../../../integer.md) coefficients $b_1,\ldots,b_n$.

To prove necessity, suppose no nonempty [subset](../../../../../subset.md) of the $b_i$ sums to zero. Choose a [prime](../../../../../prime-number.md) $p>\sum_i|b_i|$ and use the [last nonzero digit coloring](../../../../../last-nonzero-digit-coloring.md)

$$
c(x)=p^{-v_p(x)}x\pmod p\ \in\mathbb F_p^{\times},
$$

where $v_p$ is the [P-adic valuation](../../../../../p-adic-valuation.md). If positive $x_i$ all had the same colour $u$ and satisfied $\sum_i b_ix_i=0$, let $m=\min_i v_p(x_i)$ and $I=\{i:v_p(x_i)=m\}$. After division by $p^m$ and reduction modulo $p$, the equation becomes

$$
u\sum_{i\in I}b_i=0\quad\text{in }\mathbb F_p.
$$

As $u\ne0$, this says $p\mid\sum_{i\in I}b_i$. The latter sum is nonzero and has absolute value at most $\sum_i|b_i|<p$, a contradiction. This explicitly proves the necessary obstruction without invoking a general [partition regularity](../../../../../partition-regular-matrix.md) criterion.

Conversely, suppose $\varnothing\ne I\subseteq\{1,\ldots,n\}$ and $\sum_{i\in I}b_i=0$. Select an index $j\in I$, and put

$$
S=\sum_{i\notin I}b_i,\qquad s=|b_j|,\qquad q=-\frac{sS}{b_j}\in\mathbb Z,\qquad u=\max(0,-q),\qquad L=\max(2,|q|+1).
$$

For any [finite colouring](../../../../../finite-coloring.md), the [Brauer progression theorem](../../../../../brauer-progression-theorem.md) gives one-coloured $\{sd,a,a+d,\ldots,a+(L-1)d\}$. The indices $u$ and $u+q$ both lie between $0$ and $L-1$. Define positive, same-coloured coordinates by

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

This also covers $I$ equal to the whole index [set](../../../../../set-split.md) and $q=0$. Reversing the clearing of denominators proves the exact criterion:

$$
\boxed{(a_1,\ldots,a_n)\text{ is partition regular}\quad\Longleftrightarrow\quad
\exists\varnothing\ne I\subseteq\{1,\ldots,n\}:\ \sum_{i\in I}a_i=0.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
