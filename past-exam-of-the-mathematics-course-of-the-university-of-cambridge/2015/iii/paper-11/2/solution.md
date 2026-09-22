<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**The [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md).** For a [uniform set family](../../../../../uniform-set-family.md) $\mathcal F$ of $r$-sets, its [lower shadow](../../../../../lower-shadow.md) is

$$
\partial\mathcal F=\{D:|D|=r-1,\ D\subset F\text{ for some }F\in\mathcal F\}.
$$

If $\mathcal I_r(a)$ consists of the first $a$ $r$-sets in [colexicographic order](../../../../../colexicographic-order.md), then

$$
\boxed{|\partial\mathcal F|\geq|\partial\mathcal I_r(|\mathcal F|)|.}
$$

Here $B<A$ in [colexicographic order](../../../../../colexicographic-order.md) means that the largest element of the [symmetric difference](../../../../../symmetric-difference.md) $A\triangle B$ belongs to $A$. In terms of the unique greedy [binomial representation](../../../../../combinatorial-number-system.md)

$$
a=\binom{k_r}r+\binom{k_{r-1}}{r-1}+\cdots+\binom{k_s}s,
\qquad k_r>k_{r-1}>\cdots>k_s\geq s\geq1,
$$

the bound is

$$
\boxed{|\partial\mathcal F|\geq\binom{k_r}{r-1}+\binom{k_{r-1}}{r-2}+\cdots+\binom{k_s}{s-1}.}
$$

For $a=0$ the right side is zero. We prove both the minimizing assertion and this formula.

First, the [lower shadow](../../../../../lower-shadow.md) of a [colexicographic initial segment](../../../../../colexicographic-initial-segment.md) is a [colexicographic initial segment](../../../../../colexicographic-initial-segment.md). One way to check this is to extend an $(r-1)$-set $D$ by its least missing positive integer; this is its earliest $r$-set extension in [colexicographic order](../../../../../colexicographic-order.md). If $E<D$, the earliest extension of $E$ is no later than the earliest extension of $D$. To see the latter assertion, let $j=\max(D\triangle E)\in D$. If $E$ misses an integer below $j$, its least missing integer is below $j$, so its earliest extension is still earlier than the earliest extension of $D$. Otherwise $E$ contains every integer below $j$. Above $j$ the two sets agree, and their equal sizes force $D$ to contain $j$ and all but one integer below $j$. Adding that missing integer to $D$, or adding $j$ to $E$, gives the same earliest extension. Thus every set earlier than a member of the [lower shadow](../../../../../lower-shadow.md) is also in that [lower shadow](../../../../../lower-shadow.md).

We now prove the minimizing assertion by induction on the size $N$ of a finite ground set. The case $r=1$ is immediate: a nonempty [uniform set family](../../../../../uniform-set-family.md) of singletons has [lower shadow](../../../../../lower-shadow.md) $\{\varnothing\}$. The empty case and $r=N$ are also immediate. For a coordinate $i$, write the two sections of $\mathcal F$ as

$$
\mathcal F_0=\{A\in\mathcal F:i\notin A\},\qquad
\mathcal F_1=\{A\setminus\{i\}:A\in\mathcal F, i\in A\}.
$$

They are respectively $r$- and $(r-1)$-[uniform set families](../../../../../uniform-set-family.md) on $[N]\setminus\{i\}$. Perform a [colexicographic section compression](../../../../../colexicographic-section-compression.md): replace each section by the [colexicographic initial segment](../../../../../colexicographic-initial-segment.md) of the same size. The two sections of the [lower shadow](../../../../../lower-shadow.md) before this operation are

$$
\partial\mathcal F_0\cup\mathcal F_1,\qquad \partial\mathcal F_1.
$$

By the inductive hypothesis the individual [lower shadows](../../../../../lower-shadow.md) do not grow. After [colexicographic section compression](../../../../../colexicographic-section-compression.md), both families in the displayed union are [colexicographic initial segments](../../../../../colexicographic-initial-segment.md), so their union has the larger of their two sizes. This is no greater than the original union. Consequently [colexicographic section compression](../../../../../colexicographic-section-compression.md) preserves $|\mathcal F|$ and does not increase $|\partial\mathcal F|$. A section of size zero causes no difficulty; a section of $0$-sets is already compressed and its [lower shadow](../../../../../lower-shadow.md) is empty.

Repeat any [colexicographic section compression](../../../../../colexicographic-section-compression.md) that changes the family. The sum of the positions of its members in [colexicographic order](../../../../../colexicographic-order.md) strictly decreases, since restriction to either fixed-coordinate section preserves that order. Hence the process terminates at a family $\mathcal G$ all of whose sections are [colexicographic initial segments](../../../../../colexicographic-initial-segment.md).

There is only one possible obstruction to $\mathcal G$ itself being a [colexicographic initial segment](../../../../../colexicographic-initial-segment.md). Suppose $B<A$, $A\in\mathcal G$ and $B\notin\mathcal G$. No coordinate can belong to both $A,B$, or to neither: either possibility would contradict the compressed section at that coordinate. Thus $A,B$ partition $[N]$, and $N=2r$. Moreover, every such inversion must use this same complementary pair: any omitted set below $A$ equals $A^c=B$, and any included set above $B$ equals $B^c=A$. These observations also rule out an inversion completely before or after this pair. A set strictly between $B$ and $A$ would have to be both present, by comparison with $A$, and absent, by comparison with $B$. Therefore $B,A$ are consecutive in [colexicographic order](../../../../../colexicographic-order.md). Since $A$ contains $2r$ and $B$ does not, they must be

$$
B=\{r,r+1,\ldots,2r-1\},\qquad A=\{1,2,\ldots,r-1,2r\}.
$$

Thus the exceptional family is $[2r-1]^{(r)}\setminus\{B\}\cup\{A\}$. For $r\geq2$, deleting $B$ leaves every $(r-1)$-set of $[2r-1]$ in the [lower shadow](../../../../../lower-shadow.md): each has $r$ extensions inside $[2r-1]$, so at least one remains. Its [lower shadow](../../../../../lower-shadow.md) therefore contains the [lower shadow](../../../../../lower-shadow.md) of the equally sized [colexicographic initial segment](../../../../../colexicographic-initial-segment.md) $[2r-1]^{(r)}$. The case $r=1$ was already handled. This proves the minimizing assertion in all cases.

Finally the greedy [binomial representation](../../../../../combinatorial-number-system.md) describes the successive blocks of a [colexicographic initial segment](../../../../../colexicographic-initial-segment.md). Its first block is $[k_r]^{(r)}$, and the remaining sets are obtained by adding $k_r+1$ to an initial segment of $(r-1)$-sets inside $[k_r]$. The [lower shadow](../../../../../lower-shadow.md) without $k_r+1$ has $\binom{k_r}{r-1}$ members; the [lower shadow](../../../../../lower-shadow.md) containing $k_r+1$ is the corresponding lower-rank [lower shadow](../../../../../lower-shadow.md). Repeating this decomposition proves the displayed [binomial coefficient](../../../../../binomial-coefficient.md) formula and completes the [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md) proof.

**The specified initial segment covers every $r$-set of $[m]$.** Assume $m\geq r+1$ and $r\geq1$, the nontrivial range. The last $r$-set of $[m]$ in [colexicographic order](../../../../../colexicographic-order.md) is

$$
R=\{m-r+1,\ldots,m\}.
$$

Its earliest $(r+1)$-set extension is $\{1\}\cup R$. Exactly $m-r-1$ sets of $[m]^{(r+1)}$ come after this extension: they are $\{x\}\cup R$ with $2\leq x\leq m-r$. Its position is therefore

$$
\binom m{r+1}-m+r+1.
$$

At the stated threshold, $R$ belongs to $\partial\mathcal I$. Since the [lower shadow](../../../../../lower-shadow.md) is a [colexicographic initial segment](../../../../../colexicographic-initial-segment.md),

$$
\boxed{[m]^{(r)}\subseteq\partial\mathcal I.}
$$

For $r=0$, the threshold is $1$ and a nonempty family of singletons has $\varnothing$ in its [lower shadow](../../../../../lower-shadow.md). If $m=r\geq1$, the threshold is again $1$; the first $(r+1)$-set is $[r+1]$, which contains $[r]^{(r)}$. If $m<r$, the desired inclusion is empty and automatic.

**The nonuniform bound.** Suppose first that $1\leq r\leq m$ and, contrapositively, that $|\mathcal B|\leq\binom mr-1$. Let $\mathcal J$ be the [colexicographic initial segment](../../../../../colexicographic-initial-segment.md) of $r$-sets of size $\binom mr-1$; this consists of $[m]^{(r)}$ with its last member $R$ removed. For each $j\geq r$, put $\mathcal A_j=\mathcal A\cap[n]^{(j)}$, and replace it by the equally sized [colexicographic initial segment](../../../../../colexicographic-initial-segment.md) $\mathcal I_j$.

Iterating the [Kruskal-Katona theorem](../../../../../kruskal-katona-theorem.md) shows that the [iterated lower shadow](../../../../../iterated-lower-shadow.md) down to size $r$ of $\mathcal I_j$ has no more members than the corresponding [iterated lower shadow](../../../../../iterated-lower-shadow.md) of $\mathcal A_j$. Indeed, at each step initial segments minimize the next [lower shadow](../../../../../lower-shadow.md), and its minimum size is increasing in the input size. The latter [iterated lower shadow](../../../../../iterated-lower-shadow.md) lies in $\mathcal B$. Therefore every $r$-subset of every member of $\mathcal I_j$ lies in $\mathcal J$.

For $j\geq r$, a $j$-set with this property must lie inside $[m]$: otherwise an $r$-subset containing an element larger than $m$ would lie outside $\mathcal J$. Among $j$-sets inside $[m]$, exactly those containing $R$ are forbidden. Hence

$$
|\mathcal A_j|=|\mathcal I_j|\leq
\binom mj-\binom{m-r}{j-r}\quad(r\leq j\leq m),
\qquad |\mathcal A_j|=0\quad(j>m).
$$

Adding these bounds proves the contrapositive. Thus **the strict threshold forces**

$$
\boxed{|\mathcal B|\geq\binom mr.}
$$

When $r=0$, the threshold merely says that $\mathcal A$ is nonempty, so $\mathcal B=\{\varnothing\}$. When $m<r$, the claimed lower bound is zero. The strict inequality is sharp: the family of all subsets of $[m]$ of size at least $r$ that do not contain $R$ attains the displayed sum and has exactly $\binom mr-1$ members in its size-$r$ [iterated lower shadow](../../../../../iterated-lower-shadow.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
