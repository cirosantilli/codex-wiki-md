<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [Freiman 2-isomorphism](../../../../../freiman-2-isomorphism.md) between subsets of [abelian groups](../../../../../abelian-group.md) is a [bijection](../../../../../bijection.md) $\phi$ such that

$$
a_1+a_2=a_3+a_4\iff\phi(a_1)+\phi(a_2)=\phi(a_3)+\phi(a_4).
$$

Both directions matter: an injective homomorphism on individual elements may still create new pair-sum relations. More generally a [Freiman s-isomorphism](../../../../../freiman-s-isomorphism.md) preserves equalities of sums of $s$ elements in both directions. For a nonempty [finite set](../../../../../finite-set.md), its [doubling constant](../../../../../doubling-constant.md) is $\sigma[A]=|A+A|/|A|$. A [Freiman 2-isomorphism](../../../../../freiman-2-isomorphism.md) preserves this constant, since $a+b\mapsto\phi(a)+\phi(b)$ is a well-defined [bijection](../../../../../bijection.md) of the two [sumsets](../../../../../sumset.md).

First let $A\subseteq\mathbb Z$ have $n$ elements and doubling at most $K$. The permitted [Plünnecke-Ruzsa inequality](../../../../../plunnecke-ruzsa-inequality.md) gives $|2A-2A|\leq K^4n$. We will obtain the [half-size prime cyclic Freiman model](../../../../../half-size-prime-cyclic-freiman-model.md) for every prime $p>4K^4n$. Choose an auxiliary prime $q>p$ larger than the absolute value of every member of $2A-2A$. Such a prime exists: for any [integer](../../../../../integer.md) bound $M$, every prime divisor of $M!+1$ exceeds $M$.

Choose $\lambda$ uniformly from the nonzero residues modulo $q$. For each nonzero $d\in2A-2A$, the residue $\lambda d$ is uniform among the nonzero residues. Put

$$
T=\{jp\pmod q:0<|jp|<q\}.
$$

There are at most $2(q-1)/p$ such residues, and therefore the [probability](../../../../../probability.md) that any of the nonzero differences is dilated into $T$ is at most

$$
|2A-2A|\frac{2q}{p(q-1)}\leq\frac{4K^4n}{p}<1.
$$

The first cardinal estimate is an upper bound even if some listed residues coincide; the slightly looser [probability](../../../../../probability.md) bound is convenient. Thus there exists $\lambda$ with no such bad difference.

For this $\lambda$, let $t_a\in\{0,\ldots,q-1\}$ represent $\lambda a$. Split these representatives into the two intervals $[0,(q-1)/2]$ and $[(q+1)/2,q-1]$. Take $A'$ from the more populated interval, so $|A'|\geq n/2$. For any four elements of $A'$, put $D=t_{a_1}+t_{a_2}-t_{a_3}-t_{a_4}$. Their common half-interval gives $|D|<q$, and

$$
D\equiv\lambda(a_1+a_2-a_3-a_4)\pmod q.
$$

If the original difference is zero, then $D$ is a multiple of $q$ of absolute value less than $q$, so $D=0$. If the original difference is nonzero, $D$ is nonzero, and it cannot be a multiple of $p$: otherwise its residue belongs to $T$, contrary to the choice of $\lambda$. Therefore $a\mapsto t_a\pmod p$ preserves pair-sum relations in both directions. It is injective as well, by applying the relation test to $a+a_0=b+a_0$ with any fixed $a_0\in A'$. Hence

$$
\boxed{|A'|\geq|A|/2,\quad A'\text{ has a Freiman 2-model in }\mathbb Z/p\mathbb Z\text{ for every }p>4K^4|A|.}
$$

This proves the stated polynomial bound, including the prescribed prime rather than just an unspecified cyclic modulus.

Now let $A\subseteq\mathbb F_2^\infty$. Finiteness of $A$ places it in some finite-dimensional coordinate space, so models exist. Choose a [Freiman 2-isomorphism](../../../../../freiman-2-isomorphism.md) $A\to C\subseteq\mathbb F_2^m$ with $m$ minimal. The [doubling constant](../../../../../doubling-constant.md) of $C$ is at most $K$.

If a nonzero $v$ did not belong to $4C$, projection onto $\mathbb F_2^m/\langle v\rangle$ would preserve all pair-sum relations in both directions: a new relation would have original difference $v$, whereas in [characteristic two](../../../../../characteristic-two.md) every such difference lies in $4C$. Projection is also injective on $C$, since $C+C\subseteq4C$ by adding any element of $C$ twice. This would give a model in dimension $m-1$, contradicting minimality. Consequently every nonzero vector belongs to $4C$; zero belongs as well, by adding one element four times. Thus $4C=\mathbb F_2^m$.

Using the [Plünnecke-Ruzsa inequality](../../../../../plunnecke-ruzsa-inequality.md) once more gives

$$
\boxed{2^m=|4C|\leq K^4|C|=K^4|A|.}
$$

This is the [minimal binary Freiman models have full fourfold sumset](../../../../../minimal-binary-freiman-models-have-full-fourfold-sumset.md) argument. It also covers a singleton, with $m=0$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
