<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $0\leq t\leq k\leq n$, define the [complete-intersection candidate families](../../../../../complete-intersection-candidate-family.md)

$$
\mathcal F_i=\{A\in[n]^{(k)}:|A\cap[t+2i]|\geq t+i\},\qquad 0\leq i\leq\min\{k-t,\lfloor(n-t)/2\rfloor\}.
$$

Each is a [t-intersecting family](../../../../../t-intersecting-family.md), since two members have at least $2(t+i)-(t+2i)=t$ common points in the distinguished block. The [cardinality](../../../../../cardinality.md) form of the [Ahlswede-Khachatrian theorem](../../../../../ahlswede-khachatrian-theorem.md) is

$$
\boxed{M(n,k,t)=\max_i\sum_{j=t+i}^{\min\{k,t+2i\}}\binom{t+2i}j\binom{n-t-2i}{k-j}=\max_i|\mathcal F_i|.}
$$

A [binomial coefficient](../../../../../binomial-coefficient.md) with lower argument outside its usual range is zero. For $t=0$, or $n\leq2k-t$, the answer is $\binom nk$; in the latter case every pair of $k$-sets already intersects in at least $t$ points. The displayed candidate formula also attains this value: its largest allowed index is at least $n-k$, so every $k$-set has enough points in that candidate's block. For $t=k$ the answer is one. We prove the remaining cases without assuming the complete intersection theorem as an auxiliary result.

We first record the $t=1$ case of the [Erdős-Ko-Rado theorem](../../../../../erdos-ko-rado-theorem.md). For $n\geq2k$, put the ground set in a [cyclic ordering](../../../../../cyclic-ordering.md). An [intersecting family](../../../../../intersecting-family.md) contains at most $k$ of its length-$k$ intervals. To see this, rotate a selected interval to end at position $n$. Intervals ending at $k,\ldots,n-k$ miss it. The other possible endpoints, except $n$, are paired as $j,j+n-k$, $1\leq j\leq k-1$, and the two intervals in each pair are disjoint. Thus at most $1+(k-1)=k$ intervals are selected. Averaging over all cyclic orders, each $k$-set has the same chance to occur among the $n$ intervals, yielding

$$
|\mathcal A|\frac n{\binom nk}\leq k,\qquad |\mathcal A|\leq\binom{n-1}{k-1}=|\mathcal F_0|.
$$

For $n<2k$ the whole layer works. This proves the $t=1$ case, including $n=2k$ without any uniqueness assertion.

We may now suppose $2\leq t<k$ and $n>2k-t$. If $n=2k-t+1$, [complementation of uniform intersecting families](../../../../../complementation-of-uniform-intersecting-families.md) changes the problem to an intersecting family of $(k-t+1)$-sets. The just-proved case gives $M(n,k,t)=\binom{n-1}{k-t}=\binom{n-1}k$. This is $|\mathcal F_{k-t}|$, the family of all $k$-sets avoiding the last coordinate. Hence it remains to treat $n\geq2k-t+2$.

Apply [coordinate shifts of a set family](../../../../../coordinate-shifts-of-a-set-family.md) with $i<j$. They preserve [cardinality](../../../../../cardinality.md) and t-intersection. The only way a moved member could lose an intersection point with an unmoved member is that the former moves $j$ to $i$ while the latter contains $j$ and avoids $i$. The latter's shifted partner must already belong to the original family, since otherwise it too would move; that partner would have had an intersection of size less than $t$ with the original moved member, a contradiction. If both members move, their intersection size is unchanged. Every nontrivial shift decreases the sum of all coordinates in all members, so repeated shifts terminate at a [left-compressed set family](../../../../../left-compressed-set-family.md). We can therefore choose a maximum family $\mathcal A$ [left-compressed](../../../../../left-compressed-set-family.md).

We prove the [small-support generating lemma for extremal intersecting families](../../../../../small-support-generating-lemma-for-extremal-intersecting-families.md), including the replacement argument responsible for the threshold. A [generating family for a uniform set family](../../../../../generating-family-for-a-uniform-set-family.md) is a family $\mathcal G$ of sets of size at most $k$ whose $k$-element supersets are exactly $\mathcal A$. Start with $\mathcal G=\mathcal A$. A left shift of a generator still has every $k$-element extension in $\mathcal A$: if the extension contains the removed coordinate it already contains the old generator; otherwise reverse that shift in the extension and use left-compression of $\mathcal A$. Taking all left shifts of generators, then deleting inclusion-redundant generators, therefore gives an [antichain](../../../../../antichain.md) of generators with the following property: every left shift of a generator contains a generator. This normalization never enlarges the support. Choose a normalized generating family whose largest support coordinate $m$ is as small as possible.

The generators themselves are [t-intersecting](../../../../../t-intersecting-family.md). Indeed, if two generators intersect in fewer than $t$ points, they can be extended to $k$-sets with intersection size $\max\{|G\cap H|,2k-n\}<t$: fill their two residual quotas with disjoint points as far as possible. This contradicts the defining property of the generated family. A generator containing $m$ has the [maximum-support generator fibre](../../../../../maximum-support-generator-fibre.md)

$$
\{A\in\mathcal A:A\cap[m]=G\},\qquad\text{size }\binom{n-m}{k-|G|},
$$

as its exclusively generated members. In fact, any extra coordinate $i<m$ in the prefix supplies a generator inside $G-\{m\}+\{i\}$, which avoids $m$ and also generates that member. An exact prefix $G$ contains no other generator by the [antichain](../../../../../antichain.md) property.

If two generators containing $m$ have intersection exactly $t$, they must have union $[m]$: any earlier coordinate missing from both permits shifting $m$ out of one generator and lowers their intersection below $t$. Thus [tight pairs of left-compressed generators](../../../../../tight-pairs-of-left-compressed-generators.md) have sizes summing to $m+t$. Write $\mathcal G_a$ for the generators of size $a$ containing $m$, and put $N=n-m$. Generators avoiding $m$ still meet a shortened generator in at least $t$ points, and shortened generators in classes $a,b$ still meet in at least $t$ unless $a+b=m+t$.

Suppose

$$
n>(k-t+1)\left(2+\frac{t-1}{r+1}\right),\qquad m>t+2r.
$$

We will contradict extremality or the minimality of $m$. If all the nonempty classes have $a\leq k-N$, no two of them can have sizes summing to $m+t$: for any partner of size at most $k$, their sum is at most $2k-N<m+t$, since $n>2k-t$. We may therefore shorten every generator containing $m$, preserving t-intersection and generating a family containing $\mathcal A$. By maximal [cardinality](../../../../../cardinality.md) it generates exactly $\mathcal A$, with support at most $m-1$, a contradiction. There must be a class with $a>k-N$.

If such a class has $2a\ne m+t$, put $b=m+t-a$. Remove classes $a,b$ and insert all shortened generators from class $a$, or instead all shortened generators from class $b$. Both replacements remain [t-intersecting](../../../../../t-intersecting-family.md). The first loses exactly $|\mathcal G_b|\binom N{k-b}$ exclusively generated members and gains at least $|\mathcal G_a|\binom N{k-a+1}$ new members with shortened exact prefixes and tails beyond $m$; the second gives the reversed comparison. If class $b$ is empty, the first gain is positive and contradicts extremality. Otherwise $a,b\leq k$ and $a,b>k-N$, so all four [binomial coefficients](../../../../../binomial-coefficient.md) are positive. If neither replacement increases [cardinality](../../../../../cardinality.md), multiplication of their two inequalities gives

$$
\binom N{k-a+1}\binom N{k-b+1}\leq\binom N{k-a}\binom N{k-b}.
$$

But the ratio of the left side to the right side is

$$
\frac{(N-k+a)(N-k+b)}{(k-a+1)(k-b+1)}>1.
$$

Indeed, using $a+b=m+t$, the numerator factors exceed the opposite denominator factors by $n+t-2k-1\geq1$. This contradiction excludes every noncentral class with positive fibre.

Consequently any class with $a>k-N$ is central: $m=t+2j$ and $a=t+j$ for an integer $j\geq r+1$. Shorten the central generators. Each shortened set misses exactly $j$ of the $m-1$ earlier coordinates, so some coordinate $h<m$ is absent from at least $j|\mathcal G_a|/(m-1)$ of them. Call that subfamily $\mathcal T$. Its members are [t-intersecting](../../../../../t-intersecting-family.md): a bad pair would have arisen from a tight pair whose union was $[m]$, whereas both shortened sets avoid $h$. They also meet all unchanged generators in at least $t$ points; a conflicting class would have to be the central class itself. Remove the entire central class and insert $\mathcal T$. The loss relative to the unaffected generators is exactly $|\mathcal G_a|\binom N{k-a}$. Each selected shortened prefix may be extended using the $N+1$ coordinates $m,\ldots,n$; these extensions are distinct and not generated by an unaffected generator, by the original [antichain](../../../../../antichain.md) property. The number restored or added is at least $|\mathcal T|\binom{N+1}{k-a+1}$. Their gain-to-loss ratio is therefore at least

$$
\frac j{m-1}\frac{N+1}{k-t-j+1}>1.
$$

The last inequality is equivalent, by multiplying out, to $n>(k-t+1)(2+(t-1)/j)$, which follows from $j\geq r+1$ and the assumed strict threshold. This finishes the [generator replacement proof of the small-support intersection lemma](../../../../../generator-replacement-proof-of-the-small-support-intersection-lemma.md):

$$
n>(k-t+1)\left(2+\frac{t-1}{r+1}\right)\quad\Longrightarrow\quad\mathcal G\subseteq\mathcal P([t+2r]).
$$

Reflection gives the analogous supporting suffix for a right-compressed optimum.

The second ingredient is the [compatibility bound for complementary generating families](../../../../../compatibility-bound-for-complementary-generating-families.md). Let $\mathcal H$ generate $\mathcal A^c=\{[n]\setminus A:A\in\mathcal A\}$, a $(n-2k+t)$-intersecting family of $(n-k)$-sets. For any $G\in\mathcal G$, $H\in\mathcal H$,

$$
|G\cup H|\geq n-k+t.
$$

If not, put their union in a set $T$ of size $n-k+t-1$, which is at least both $k$ and $n-k$. Extend $G$ within $T$ to a $k$-set $A\in\mathcal A$ and $H$ within $T$ to an $(n-k)$-set $B\in\mathcal A^c$. Then $B^c\in\mathcal A$, but $|A\cap B^c|=|A\cup B|-|B|\leq t-1$, a contradiction.

Set

$$
c=k-t+1,\qquad n_j=c\left(2+\frac{t-1}{j}\right)\ (j\geq1),\qquad n_0=\infty.
$$

First suppose $n_{r+1}<n<n_r$. These intervals cover the non-boundary parameters in our remaining range, with $0\leq r\leq k-t$. The support lemma gives generators on the prefix $[t+2r]$. Write $k'=n-k$, $t'=n-2k+t$ and $r'=k-t-r$. Direct rearrangement gives

$$
n>c\left(2+\frac{t'-1}{r'+1}\right),\qquad k'-t'+1=c.
$$

After multiplication by $r'+1=c-r$, the strict inequality becomes $c(t-1)+r(2c-n)>0$. For $r>0$ this is exactly $n<n_r$; for $r=0$ it is $c(t-1)>0$. Thus the reflected support lemma gives generators for $\mathcal A^c$ on a suffix of length $t'+2r'=n-t-2r$, disjoint from the prefix.

If every prefix generator has size at least $t+r$, then $\mathcal A\subseteq\mathcal F_r$. If every suffix generator has size at least $t'+r'=n-k-r$, every complemented member contains that many suffix points, and its original member has at least $t+r$ prefix points; again $\mathcal A\subseteq\mathcal F_r$. At least one of these alternatives holds: otherwise generators of sizes at most $t+r-1$ and $n-k-r-1$ would have union of size at most $n-k+t-2$, violating compatibility. Since $\mathcal F_r$ itself is [t-intersecting](../../../../../t-intersecting-family.md) and $\mathcal A$ is maximum,

$$
M(n,k,t)=|\mathcal F_r|\qquad(n_{r+1}<n<n_r).
$$

Finally suppose $n=n_{r+1}>2k-t+1$. The support lemma, now with index $r+1$, places $\mathcal G$ in $[t+2r+2]$. For the complement, the strict support inequality still places $\mathcal H$ in the suffix beginning at $t+2r+1$. These supports overlap in two coordinates, which is harmless for the union bound in compatibility. Either every $G$ has size at least $t+r+1$, placing $\mathcal A$ inside $\mathcal F_{r+1}$, or every $H$ has size at least $n-k-r$, placing $\mathcal A$ inside $\mathcal F_r$. If neither held, a pair of generators would have union of size at most $n-k+t-1$, again impossible.

The two candidate sizes agree at this boundary. In passing from $\mathcal F_r$ to $\mathcal F_{r+1}$, the gained sets have $t+r-1$ points in the old block and both new points; the lost sets have $t+r$ old-block points and neither new point. Their counts are

$$
\binom{t+2r}{t+r-1}\binom{n-t-2r-2}{k-t-r-1},\qquad\binom{t+2r}{t+r}\binom{n-t-2r-2}{k-t-r}.
$$

The ratio is one exactly when $(r+1)n=c(t+2r+1)$, that is, $n=n_{r+1}$. Therefore $M=|\mathcal F_r|=|\mathcal F_{r+1}|$ there. The full-level cases, the elementary $t=1$ proof, the complementary borderline case, and these strict-interval and boundary arguments establish the boxed [cardinality](../../../../../cardinality.md) theorem for every admissible parameter.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
