<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

We take $\alpha,\beta>0$, as is necessary for the assertion. The nonvacuous cases have $0<\alpha\leq1/2$ and $0<\beta\leq1$. Put $n=|A|$ and

$$
K=\max_{b\in B}\frac{|A+bA|}{n}.
$$

We prove a lower bound for $K$ by transferring small [sumset](../../../../../sumset.md) growth through algebraic operations on the [scalars](../../../../../scalar.md). This gives a self-contained [polynomial skew-sumset expansion over a prime field](../../../../../polynomial-skew-sumset-expansion-over-a-prime-field.md) proof using the permitted [Ruzsa triangle inequality](../../../../../ruzsa-triangle-inequality.md), [Ruzsa covering lemma](../../../../../ruzsa-covering-lemma.md) and [Plünnecke-Ruzsa inequality](../../../../../plunnecke-ruzsa-inequality.md).

Since $|B|>1$, choose $b_0\in B\setminus\{0\}$. The bound $|b_0A+A|\leq K|b_0A|$ and the mixed-set [Plünnecke-Ruzsa inequality](../../../../../plunnecke-ruzsa-inequality.md) give

$$
|rA-sA|\leq K^{r+s}n\qquad(r,s\text{ nonnegative integers}).
$$

In particular $|A+A|\leq K^2n$ and $|3A-2A|\leq K^5n$. Here repeated-set sums such as $3A$ allow independent choices from each copy.

For a [scalar](../../../../../scalar.md) $t$, write $D(t)=|A+tA|/n$, and put $Q=A-A$ for the [difference set](../../../../../difference-set.md). The [Ruzsa covering lemma](../../../../../ruzsa-covering-lemma.md) gives $tA\subseteq T_t+Q$ with $|T_t|\leq D(t)$. Indeed choose a maximal family of disjoint translates $u+A$, with $u\in tA$; counting their union bounds the family size, and maximality forces every remaining translate to meet one of them.

For any $r,s$, the containments $A+(r+s)A\subseteq A+rA+sA$ and $A+rsA\subseteq rT_s+A+rQ$ give, after covering each copy of $rA,sA$,

$$
D(r+s)\leq K^5D(r)D(s),\qquad D(rs)\leq K^5D(r)^2D(s).
$$

For the second bound, specifically $rQ=rA-rA\subseteq T_r-T_r+2Q$, and $A+2Q=3A-2A$. The [Ruzsa triangle inequality](../../../../../ruzsa-triangle-inequality.md) also gives $|A-rA|\leq|A+A|\,|A+rA|/n$, so $D(-r)\leq K^2D(r)$. These are the [closure bounds for small skew-sumset scalars](../../../../../closure-bounds-for-small-skew-sumset-scalars.md).

We next prove a growth lemma for the [scalar](../../../../../scalar.md) sets. For $S\subseteq\mathbb F_p$ with $m=|S|\geq2$, let

$$
R=\left\{\frac{a-b}{c-d}:a,b,c,d\in S,\ c\ne d\right\}.
$$

If $R\ne\mathbb F_p$, then $R+1$ is not contained in $R$: otherwise equal [cardinality](../../../../../cardinality.md) would make $R$ invariant under addition of one, which generates the entire [prime field](../../../../../prime-field.md). Choose $r=1+(a-b)/(c-d)\notin R$. The map $(x,y)\mapsto x+ry$ on $S^2$ is injective. Indeed a collision with different second coordinates would express $r$ as a ratio of two differences from $S$, while equal second coordinates force equal first coordinates. Clearing the nonzero denominator puts its image inside

$$
(c-d)S+(c-d+a-b)S\subseteq3SS-3SS,
$$

so the latter set has at least $m^2$ elements. Here $SS$ is the [product set](../../../../../product-set.md), and $3SS-3SS$ denotes three independent product terms minus three others, not multiplication by the [scalar](../../../../../scalar.md) three.

If $R=\mathbb F_p$, let $E_t$ count the collisions $x_1+ty_1=x_2+ty_2$ with all four variables in $S$. Summing over $t$ gives

$$
\sum_{t\in\mathbb F_p}E_t=pm^2+m^3(m-1)\leq pm^2+m^4.
$$

The first term comes from equal second coordinates, which force equal first coordinates. For unequal second coordinates, each quadruple determines exactly one [scalar](../../../../../scalar.md). Some $t$ consequently satisfies $E_t\leq m^2+m^4/p$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) on the representation counts gives

$$
|S+tS|\geq\frac{m^4}{E_t}\geq\frac{m^2}{1+m^2/p}\geq\tfrac12\min(p,m^2).
$$

Representing $t$ as a ratio from $R$ and clearing its denominator embeds a dilate of this [sumset](../../../../../sumset.md) in $2SS-2SS\subseteq3SS-3SS$, padding with the same product in the positive and negative sums. We have proved the [quadratic growth of a sixfold product difference set](../../../../../quadratic-growth-of-a-sixfold-product-difference-set.md) estimate

$$
\boxed{|3SS-3SS|\geq\tfrac12\min(p,|S|^2).}
$$

Starting from $S_0=B$, define $S_{j+1}=3S_jS_j-3S_jS_j$. Choose

$$
k=1+\left\lceil\log_2(1/\beta)\right\rceil.
$$

For $p\geq\max(4,2^{2/\beta})$, the growth lemma implies $|S_k|\geq p/2$. To see the constants explicitly, put $v_j=|S_j|/2$. Then $v_0\geq p^{\beta/2}$ and $v_{j+1}\geq\min(p/4,v_j^2)$. Induction gives $v_j\geq\min(p/4,p^{\beta2^{j-1}})$, and the chosen $k$ makes the exponent at least one.

Every $t\in S_0$ has $D(t)\leq K$. If $D(t)\leq K^{L_j}$ on $S_j$, the closure bounds show that each product has exponent at most $3L_j+5$, its negative at most $3L_j+7$, and a sum of six such terms has exponent at most $18L_j+67$. Thus, with

$$
L_0=1,\qquad L_{j+1}=18L_j+67,
$$

we have $|A+tA|\leq K^{L_k}n$ for every $t\in S_k$. The [integer](../../../../../integer.md) $L_k$ depends only on $\beta$.

Now apply the collision count to $A$ instead of $S$. Summing over all [scalars](../../../../../scalar.md) gives at most $pn^2+n^4$. Since $|S_k|\geq p/2$, some $t\in S_k$ has collision count at most $2n^2+2n^4/p$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) therefore gives

$$
K^{L_k}n\geq|A+tA|\geq\frac{n^2}{2+2n^2/p}\geq\frac14\min(n^2,p).
$$

It follows that

$$
K^{L_k}\geq\frac14\min(n,p/n)\geq\frac14p^\alpha.
$$

For $p\geq4^{2/\alpha}$ this gives $K\geq p^{\alpha/(2L_k)}\geq n^{\alpha/(2L_k)}$, proving the desired positive exponent for all sufficiently large primes.

For completeness, the same conclusion with a possibly smaller exponent holds for the remaining primes. Choose an [integer](../../../../../integer.md)

$$
P_0\geq\max(4,2^{2/\beta},4^{2/\alpha}),\qquad
c_{\alpha,\beta}=\min\left(\frac{\alpha}{2L_k},\frac{\log(1+1/P_0)}{\log P_0}\right)>0.
$$

If $p<P_0$, choose any nonzero $b\in B$. We have $1<n<p$. If $|A+bA|=n$, all its translates $A+u$ for $u\in bA$ would coincide. Two distinct such $u$ would make $A$ invariant under a nonzero [translation](../../../../../translation-geometry.md), forcing $A=\mathbb F_p$, a contradiction. Thus $|A+bA|\geq n+1\geq n^{1+c_{\alpha,\beta}}$ by the definition of the second exponent. Together with the large-prime case this proves

$$
\boxed{\exists b\in B:\ |A+bA|\geq|A|^{1+c_{\alpha,\beta}}.}
$$

Positivity of the parameters cannot be dropped: at $\alpha=0$, taking $A=\mathbb F_p$ prevents any expansion; at $\beta=0$, the allowed set $B=\{0\}$ prevents expansion of any proper $A$ with more than one element. No external sum-product theorem was invoked: the [scalar](../../../../../scalar.md) growth and transfer arguments were proved above.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
