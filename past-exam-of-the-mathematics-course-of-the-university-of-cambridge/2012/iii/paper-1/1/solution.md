<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md), the operator associated with $x\in L$ is

$$
\operatorname{ad}_x(y)=[x,y].
$$

The [Jacobi identity](../../../../../jacobi-identity.md) gives $[\operatorname{ad}_x,\operatorname{ad}_y]=\operatorname{ad}_{[x,y]}$, so this really is a [Lie algebra representation](../../../../../lie-algebra-representation.md). Define the [lower central series of a Lie algebra](../../../../../lower-central-series-of-a-lie-algebra.md) by $L^1=L$ and $L^{r+1}=[L,L^r]$. A [nilpotent Lie algebra](../../../../../nilpotent-lie-algebra.md) is one for which $L^{c+1}=0$ for some integer $c$. If this holds, $\operatorname{ad}_x$ carries $L^r$ into $L^{r+1}$, and consequently $(\operatorname{ad}_x)^cL=0$. This proves one implication without any condition on the field.

For the converse, we prove the linear form of the [Engel theorem](../../../../../engel-s-theorem.md): if $A\subseteq\operatorname{End}(V)$ is a finite-dimensional [Lie algebra](../../../../../lie-algebra-split.md) consisting entirely of [nilpotent linear maps](../../../../../nilpotent-linear-map.md), with $V\ne0$ finite-dimensional, then there is a nonzero vector annihilated by all of $A$. This argument works over any field.

Induct on $\dim A$. The assertion is immediate when $A=0$. First observe that if $b^m=0$, then its [commutator](../../../../../commutator.md) action on $\operatorname{End}(V)$ is nilpotent, because

$$
(\operatorname{ad}_b)^r(T)=\sum_{j=0}^r(-1)^j\binom rj b^{r-j}Tb^j=0\qquad(r\ge2m-1).
$$

Let $B$ be a proper [Lie subalgebra](../../../../../lie-subalgebra.md) of $A$. The [commutator](../../../../../commutator.md) action of $B$ on $A/B$ therefore consists of [nilpotent linear maps](../../../../../nilpotent-linear-map.md). Its image has dimension at most $\dim B<\dim A$, so induction supplies a nonzero coset $a+B$ annihilated by $B$. Thus $[B,a]\subseteq B$, and the normalizer $N_A(B)=\{a\in A:[a,B]\subseteq B\}$ strictly contains $B$. This is the [Engel normalizer lemma](../../../../../engel-normalizer-lemma.md).

Choose $B$ maximal among proper [Lie subalgebras](../../../../../lie-subalgebra.md). Its normalizer must be $A$, so $B$ is a [Lie algebra ideal](../../../../../ideal-of-a-lie-algebra.md). Moreover $\dim(A/B)=1$: otherwise the inverse image of a one-dimensional subalgebra of $A/B$ would lie strictly between $B$ and $A$. By induction,

$$
W=\{v\in V:bv=0\text{ for all }b\in B\}\ne0.
$$

Since $B$ is an ideal, $W$ is $A$-invariant: $b(av)=a(bv)+[b,a]v=0$. Take $x\in A\setminus B$. Its restriction to $W$ is nilpotent and hence has a nonzero kernel. A nonzero vector in that kernel is annihilated by $B$ and $x$, and therefore by all of $A$. This completes the induction.

Apply this result successively to $V$, then its quotient by a common annihilated line, and so on. We obtain a complete flag $0=V_0\subset V_1\subset\cdots\subset V_n=V$ with $AV_i\subseteq V_{i-1}$. Equivalently every element of $A$ is strictly upper triangular in one common basis; any product of $n$ such operators is zero.

Now take $V=L$ and $A=\operatorname{ad}(L)$. The hypothesis supplies exactly the nilpotence needed above. Every iterated bracket of length $n+1$, where $n=\dim L$, is an application of $n$ adjoint operators and vanishes. These brackets span $L^{n+1}$, giving $L^{n+1}=0$. The zero algebra is already nilpotent. Thus **$L$ is nilpotent if and only if every $\operatorname{ad}_x$ is nilpotent**. The common flag is essential: separate nilpotence of unrelated operators would not imply that their mixed products vanish.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
