<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $1\leq t\leq r\leq n$, define the [complete-intersection candidate families](../../../../../complete-intersection-candidate-family.md)

$$
\mathcal A_i=\{A\in[n]^{(r)}:|A\cap[t+2i]|\geq t+i\},\qquad 0\leq i\leq\min\{r-t,\lfloor(n-t)/2\rfloor\}.
$$

Each is a [t-intersecting family](../../../../../t-intersecting-family.md), since two members have at least $2(t+i)-(t+2i)=t$ common points in the distinguished block. The [cardinality](../../../../../cardinality.md) form of the [Ahlswede-Khachatrian theorem](../../../../../ahlswede-khachatrian-theorem.md) is

$$
\boxed{M(n,r,t)=\max_i|\mathcal A_i|=\max_i\sum_{j=t+i}^{\min(r,t+2i)}\binom{t+2i}j\binom{n-t-2i}{r-j}.}
$$

A [binomial coefficient](../../../../../binomial-coefficient.md) is taken as zero if its lower argument is outside its usual range.

First reduce to [left-compressed set families](../../../../../left-compressed-set-family.md). One of the [coordinate shifts of a set family](../../../../../coordinate-shifts-of-a-set-family.md), $C_{ij}$ with $i<j$, replaces $j$ by $i$ only when the target set is absent. It preserves [cardinality](../../../../../cardinality.md) and the property of being [t-intersecting](../../../../../t-intersecting-family.md). To verify the latter, a pair of newly moved sets has the same intersection size as its old pair. If just one member moves and its intersection with a retained member decreases, the retained member contains $j$ and avoids $i$. Its own shifted partner must already have belonged to the old family, otherwise it would have moved too. The old moved member and that shifted partner have the same intersection size as the allegedly bad new pair, a contradiction. Repeating changing shifts terminates because the sum of all point labels strictly decreases.

A [generating family for a uniform set family](../../../../../generating-family-for-a-uniform-set-family.md) is a collection $\mathcal G$ of sets of size at most $r$ such that

$$
\mathcal F=\{A\in[n]^{(r)}:G\subseteq A\text{ for some }G\in\mathcal G\}.
$$

Use the following [small-support generating lemma for extremal intersecting families](../../../../../small-support-generating-lemma-for-extremal-intersecting-families.md), the auxiliary result permitted here. If $n>2r-t$, $j\geq0$, and

$$
n>(r-t+1)\left(2+\frac{t-1}{j+1}\right),
$$

then every maximum-[cardinality](../../../../../cardinality.md) [left-compressed set family](../../../../../left-compressed-set-family.md) that is [t-intersecting](../../../../../t-intersecting-family.md) has a generating family contained in $\mathcal P([t+2j])$. Reflection gives the corresponding right-end supporting interval for a right-compressed optimum. The inequality is strict.

The main ideas of the generating lemma are as follows. When $n=2r-t+1$, its hypothesis forces $t+2j\geq n$, making the support conclusion automatic. Otherwise $n\geq2r-t+2$. Choose inclusion-minimal compressed generators minimizing their furthest point $q$. Partition generators containing $q$ by size. A pair whose intersection would fall below $t$ on deleting $q$ must fill $[q]$ and have sizes summing to $q+t$. Compare the two replacements associated to those complementary size classes; counting their rank-$r$ extensions makes one replacement larger unless the sizes are equal. In that balanced case, put $q=t+2j+\delta$, where $\delta\geq2$ is even. Delete $q$ from generators avoiding a suitably chosen earlier point. Averaging supplies a proportion at least $(q-t)/(2(q-1))$. The ratio of the guaranteed gain to the loss is

$$
\frac{q-t}{2(q-1)}\frac{n-q+1}{r-(q+t)/2+1}.
$$

It exceeds one precisely when $n>(r-t+1)(2+(t-1)/(j+\delta/2))$, implied by the stated hypothesis. This contradicts maximal [cardinality](../../../../../cardinality.md); redundant generators are removed after each replacement. These extension counts explain both the support bound and its strict threshold.

We also need the [compatibility bound for complementary generating families](../../../../../compatibility-bound-for-complementary-generating-families.md), which has a short direct proof. Write $\overline{\mathcal F}=\{[n]\setminus A:A\in\mathcal F\}$. If $G$ generates $\mathcal F$ and $H$ generates $\overline{\mathcal F}$, then

$$
|G\cup H|\geq n-r+t.
$$

Otherwise contain their union in a set $T$ of size $n-r+t-1$. Under $n>2r-t$ this size is at least both $r$ and $n-r$. Extend $G,H$ inside $T$ to sets $A,B$ of those respective sizes. Then $A,B^c\in\mathcal F$, whereas $|A\cap B^c|=|A\cup B|-|B|\leq t-1$, a contradiction.

The easy parameter ranges can now be disposed of. If $n\leq2r-t$, every two $r$-sets intersect in at least $t$ points, and $M(n,r,t)=\binom nr$. This is a candidate value too: choose $i=n-r$, for which the minimum possible intersection with $[t+2i]$ is exactly $t+i$. If $t=1$ and $n\geq2r$, Question 1 gives $M(n,r,1)=\binom{n-1}{r-1}=|\mathcal A_0|$. If $n=2r-t+1$, [complementation of uniform intersecting families](../../../../../complementation-of-uniform-intersecting-families.md) turns the problem into an [intersecting family](../../../../../intersecting-family.md) of rank $n-r=r-t+1$, on a ground set of size at least twice that rank. Question 1 then gives

$$
M(n,r,t)\leq\binom{n-1}{r-t}=\binom{n-1}r=|\mathcal A_{r-t}|,
$$

with equality from that candidate, the family of all $r$-sets avoiding the last point.

It remains to treat $t>1$ and $n>2r-t+1$. Put $R=r-t+1$ and

$$
N_0=\infty,\qquad N_j=R\left(2+\frac{t-1}{j}\right)\quad(j\geq1).
$$

Since $N_R=2r-t+1$, there is $0\leq k\leq R-1$ with $N_{k+1}\leq n<N_k$. Take a maximum [left-compressed set family](../../../../../left-compressed-set-family.md) $\mathcal F$. Its complement family is right-compressed and has parameters

$$
r'=n-r,\qquad t'=n-2r+t,\qquad r'-t'+1=R.
$$

It is maximum for those parameters, since complementation is a [cardinality](../../../../../cardinality.md)-preserving bijection between the two intersection problems. Put $\ell=r-t-k=R-1-k$. The strict inequality $n<N_k$ implies

$$
n>R\left(2+\frac{t'-1}{\ell+1}\right).
$$

For $k>0$, multiplying out reduces this to $nk<R(2k+t-1)$, exactly $n<N_k$; for $k=0$ it reduces to $t>1$. The reflected generating lemma therefore gives generators $\mathcal H$ for $\overline{\mathcal F}$ supported on

$$
Y=[t+2k+1,n].
$$

First suppose $N_{k+1}<n<N_k$. The original generating lemma supplies generators $\mathcal G$ supported on $X=[t+2k]$. If every $G\in\mathcal G$ has size at least $t+k$, then $\mathcal F\subseteq\mathcal A_k$. The same conclusion follows if every $H\in\mathcal H$ has size at least $n-r-k$: every complement member then has at least that many points in $Y$, forcing each original member to have at least $t+k$ points in $X$. If neither condition holds, choose $|G|\leq t+k-1$ and $|H|\leq n-r-k-1$. Then

$$
|G\cup H|\leq n-r+t-2,
$$

contradicting the proved compatibility bound. Thus $M(n,r,t)\leq|\mathcal A_k|$, and the candidate itself attains equality.

Now suppose $n=N_{k+1}$. The earlier exceptional case excludes $k=R-1$. Since $t>1$, $n>N_{k+2}$, so the original generating lemma gives $\mathcal G$ supported on $[t+2k+2]$, while the same dual argument still gives $\mathcal H$ supported on $Y=[t+2k+1,n]$. If all $G$ have size at least $t+k+1$, then $\mathcal F\subseteq\mathcal A_{k+1}$. If all $H$ have size at least $n-r-k$, then $\mathcal F\subseteq\mathcal A_k$. Otherwise a pair with $|G|\leq t+k$ and $|H|\leq n-r-k-1$ violates compatibility. Hence

$$
M(n,r,t)\leq\max\{|\mathcal A_k|,|\mathcal A_{k+1}|\}.
$$

Both candidates are available, so this proves the maximum formula also at the boundaries.

For completeness, their equality and the maximizing intervals follow from a direct count, with no appeal to the theorem. Moving from $\mathcal A_i$ to $\mathcal A_{i+1}$ adds sets containing both new coordinates and exactly $t+i-1$ old block points, and loses sets containing neither new coordinate and exactly $t+i$ old block points. Thus

$$
\begin{aligned}
|\mathcal A_{i+1}|-|\mathcal A_i|={}&\binom{t+2i}{t+i-1}\binom{n-t-2i-2}{r-t-i-1}\\
&-\binom{t+2i}{t+i}\binom{n-t-2i-2}{r-t-i}.
\end{aligned}
$$

In the nontrivial range, the gain-to-loss ratio is $\frac{(t+i)(r-t-i)}{(i+1)(n-r-i-1)}$. It exceeds, equals or falls below one according as $n$ is below, equal to or above $N_{i+1}$. Since the thresholds decrease with $i$ when $t>1$, the largest candidate is $\mathcal A_k$ in each strict interval and the consecutive candidates tie at $n=N_{k+1}$. This completes the proof of the [cardinality](../../../../../cardinality.md) theorem in every parameter range.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
