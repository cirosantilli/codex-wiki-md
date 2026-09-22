<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take the natural parameter range $1\leq t\leq r\leq n$ and admissible indices $0\leq i\leq r-t$. Larger indices give empty [set families](../../../../../set-family.md). Write $q=r-t+1$ and [set](../../../../../set-split.md) $n_0=\infty$ when discussing the first interval. For the nontrivial interval calculation, $t>1$ and $n>2r-t+1$; all prefixes used below then lie inside the ground [set](../../../../../set-split.md).

To compare consecutive [complete-intersection candidate families](../../../../../complete-intersection-candidate-family.md), put $a=t+2i$ and $b=t+i$. A [set](../../../../../set-split.md) in $\mathcal A_{i+1}\setminus\mathcal A_i$ has exactly $b-1$ points in $[a]$ and both of the next two points. A [set](../../../../../set-split.md) in $\mathcal A_i\setminus\mathcal A_{i+1}$ has exactly $b$ points in $[a]$ and neither next point. Therefore

$$
G_i=|\mathcal A_{i+1}\setminus\mathcal A_i|
=\binom{t+2i}{t+i-1}\binom{n-t-2i-2}{r-t-i-1},
$$



$$
L_i=|\mathcal A_i\setminus\mathcal A_{i+1}|
=\binom{t+2i}{t+i}\binom{n-t-2i-2}{r-t-i}.
$$

For $0\leq i<r-t$ these quantities are positive in the present range, and cancellation of [binomial coefficients](../../../../../binomial-coefficient.md) gives

$$
\frac{G_i}{L_i}
=\frac{(t+i)(r-t-i)}{(i+1)(n-r-i-1)}.
$$

The numerator minus the denominator is

$$
(i+1)(n_{i+1}-n),\qquad
n_{i+1}=q\left(2+\frac{t-1}{i+1}\right).
$$

Thus $|\mathcal A_{i+1}|$ is larger, equal or smaller than $|\mathcal A_i|$ according as $n$ is smaller, equal or larger than $n_{i+1}$. Since these thresholds decrease with the index, $n_{k+1}<n<n_k$ implies strict increase up to $\mathcal A_k$ and strict decrease thereafter:

$$
\boxed{\max_i|\mathcal A_i|=|\mathcal A_k|.}
$$

At an interior boundary $n=n_{k+1}$, the two consecutive maxima tie. The interval assertion concerns admissible $k$; taking $k>r-t$ would instead refer to an empty [set family](../../../../../set-family.md) and is not a valid interpretation.

The [Ahlswede-Khachatrian theorem](../../../../../ahlswede-khachatrian-theorem.md), in its [cardinality](../../../../../cardinality.md) form, states

$$
\boxed{M(n,r,t)=\max_{0\leq i\leq r-t}|\mathcal A_i|.}
$$

Here $\mathcal A_i$ is interpreted exactly by its intersection with $[t+2i]$, even if that prefix extends beyond $[n]$. Its size can always be written with $m_i=\min\{n,t+2i\}$ as

$$
|\mathcal A_i|=\sum_{j=t+i}^{r}\binom{m_i}{j}\binom{n-m_i}{r-j},
$$

where impossible [binomial coefficients](../../../../../binomial-coefficient.md) are zero. When $n\leq2r-t$, the whole level is $t$-intersecting and the formula gives $M=\binom nr$. The nontrivial case has $n>2r-t$.

First, each candidate is a [t-intersecting family](../../../../../t-intersecting-family.md): two members contain at least $2(t+i)-(t+2i)=t$ common points in the prefix. This proves the lower bound for $M$. We now prove the upper bound, using only the compression and generating-family facts expressly allowed in the question.

The first auxiliary fact is that the usual left [coordinate shifts of a set family](../../../../../coordinate-shifts-of-a-set-family.md) preserve [cardinality](../../../../../cardinality.md) and $t$-intersection. Iterating them produces a [left-compressed set family](../../../../../left-compressed-set-family.md) of the same size. The shift $S_{ab}$ with $a<b$ replaces $b$ by $a$ only when $b$ is present, $a$ is absent, and the replacement is not already in the [set family](../../../../../set-family.md). A [set family](../../../../../set-family.md) is left-compressed when it is fixed by every such shift. Right compression is the reflected notion.

For the second auxiliary fact, a [generating family for a uniform set family](../../../../../generating-family-for-a-uniform-set-family.md) $\mathcal G$ means a collection of [sets](../../../../../set-split.md) of size at most $r$ with

$$
\mathcal F=\{A\in[n]^{(r)}:G\subseteq A\text{ for some }G\in\mathcal G\}.
$$

The permitted [small-support generating lemma for extremal intersecting families](../../../../../small-support-generating-lemma-for-extremal-intersecting-families.md) is this precise statement: if $\mathcal F$ is a maximum-cardinality left-compressed $t$-intersecting [set family](../../../../../set-family.md), $n>2r-t$, and

$$
n>(r-t+1)\left(2+\frac{t-1}{j+1}\right)
\quad(j\geq0),
$$

then it has a generating [set family](../../../../../set-family.md) supported on $[t+2j]$. Reflection gives the same assertion for a right-compressed extremal [set family](../../../../../set-family.md), with the supporting interval at the right end. These two auxiliary results are being used as permitted lemmas; the extremal conclusion of the theorem is established in the remaining argument.

Choose a maximum left-compressed [set family](../../../../../set-family.md) $\mathcal F$. Its complement [set family](../../../../../set-family.md)

$$
\mathcal F^*=\{[n]\setminus A:A\in\mathcal F\}
$$

is right-compressed, has uniformity $r'=n-r$ and intersection parameter $t'=n-2r+t$, and is extremal for those parameters. Indeed

$$
|([n]\setminus A)\cap([n]\setminus B)|=n-2r+|A\cap B|,
$$

so complementation gives a cardinality-preserving bijection between the two classes of intersecting [set families](../../../../../set-family.md). Notice that $r'-t'+1=q$ too.

We need a compatibility observation, which we prove. If $G$ generates $\mathcal F$ and $H$ generates $\mathcal F^*$, then

$$
\boxed{|G\cup H|\geq n-r+t.}
$$

Otherwise extend $G\cup H$ to a [set](../../../../../set-split.md) $T$ of size $n-r+t-1$. This size is at least both $r$ and $n-r$ because $n\geq2r-t+1$ and $t\geq1$. Choose an $r$-set $A\subseteq T$ containing $G$, and an $(n-r)$-set $B\subseteq T$ containing $H$. Their generating properties imply $A,[n]\setminus B\in\mathcal F$, but

$$
|A\cap([n]\setminus B)|=|A\cup B|-|B|
\leq(n-r+t-1)-(n-r)=t-1,
$$

a contradiction. This [compatibility bound for complementary generating families](../../../../../compatibility-bound-for-complementary-generating-families.md) is the link between the two compression directions.

Suppose first that $t>1$ and $n>2r-t+1$ lies strictly between $n_{k+1}$ and $n_k$. Put $m=t+2k$ and $h=r-t-k$. The small-support lemma gives generators $\mathcal G$ for $\mathcal F$ supported on $[m]$. It also gives generators $\mathcal H$ for $\mathcal F^*$ supported on $[m+1,n]$. For completeness, the dual inequality required here is

$$
n>q\left(2+\frac{t'-1}{h+1}\right).
$$

Writing $D=n-2q$, it is equivalent to $kD<q(t-1)$, exactly the upper interval inequality $n<n_k$; for $k=0$ it follows from $t>1$. The dual support length is $t'+2h=n-m$.

Either every $G\in\mathcal G$ has $|G|\geq t+k$, or every $H\in\mathcal H$ has $|H|\geq n-r-k$. If neither assertion held, a pair of smaller generators would have union size at most

$$
(t+k-1)+(n-r-k-1)=n-r+t-2,
$$

contradicting the compatibility bound. In the first alternative, every member of $\mathcal F$ has at least $t+k$ points in $[m]$, so $\mathcal F\subseteq\mathcal A_k$. In the second alternative, each complement has at least $n-r-k$ points in $[m+1,n]$, leaving its original [set](../../../../../set-split.md) with at most $r-t-k$ points there; again $\mathcal F\subseteq\mathcal A_k$. Therefore $M\leq|\mathcal A_k|$, proving the theorem in every strict interval.

At an interior boundary $n=n_{k+1}$, with $0\leq k\leq r-t-1$, apply the small-support lemma at index $k+1$ to the original [set family](../../../../../set-family.md), since $n>n_{k+2}$. Its generators are supported on $[t+2k+2]$. The dual generators are still supported on $[t+2k+1,n]$, by the same dual calculation with $h=r-t-k$. Either all original generators have size at least $t+k+1$, or all dual generators have size at least $n-r-k$: failure of both would give union size at most $n-r+t-1$, again impossible. The first alternative places $\mathcal F$ inside $\mathcal A_{k+1}$, and the second places it inside $\mathcal A_k$. The comparison already proved gives $|\mathcal A_k|=|\mathcal A_{k+1}|$, so the common size is $M$.

It remains to cover the endpoint cases, not to assume them implicitly. For $t=1$ and $n>2r$, the small-support lemma with $j=0$ puts an extremal left-compressed [set family](../../../../../set-family.md)'s generators inside $\{1\}$. Its members must all contain one, giving $M\leq\binom{n-1}{r-1}$, attained by $\mathcal A_0$. For $t=1$, $n=2r$, at most one member of each complementary pair can occur, so $M\leq\tfrac12\binom{2r}{r}=\binom{2r-1}{r-1}$, again attained by $\mathcal A_0$. If $n<2r$, the whole level is intersecting.

For $t>1$ and $n=2r-t+1$, complementation changes the problem into a one-intersection problem with uniformity $q=r-t+1$. Since $n=2q+t-1>2q$, the preceding case gives

$$
M(n,r,t)=\binom{n-1}{q-1}=\binom{n-1}{r},
$$

attained by $\mathcal A_{r-t}$, the [set family](../../../../../set-family.md) of $r$-sets avoiding the final point. For $n\leq2r-t$, every two $r$-sets meet in at least $2r-n\geq t$, so $M=\binom nr$ and $\mathcal A_{r-t}$ is the whole level. Finally, $t=r$ gives $M=1$ directly. These cases, the strict intervals and their boundaries cover all $1\leq t\leq r\leq n$, completing the proof of the stated maximum formula.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
