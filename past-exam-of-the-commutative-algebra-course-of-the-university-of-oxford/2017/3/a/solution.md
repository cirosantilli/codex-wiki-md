<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Krull dimension](../../../../krull-dimension.md) of a [commutative ring](../../../../commutative-ring.md) $R$ is

$$
\boxed{\dim R=\sup\{d:\text{there exist prime ideals }P_0\subsetneq P_1\subsetneq\cdots\subsetneq P_d\}.}
$$

The length of a [prime chain](../../../../prime-chain.md) counts strict inclusions, rather than the number of [prime ideals](../../../../prime-ideal.md).

Let $R$ be a [principal ideal domain](../../../../principal-ideal-domain.md) that is not a [field](../../../../field.md). We first show that every nonzero [prime ideal](../../../../prime-ideal.md) is a [maximal ideal](../../../../maximal-ideal.md). Write such a [prime ideal](../../../../prime-ideal.md) as $P=(p)$ with $p\ne0$, and suppose $P\subseteq(a)$. Then $p=ab$ for some $b\in R$. Since $ab\in P$, either $a\in P$, in which case $(a)=P$, or $b\in P$. In the second case $b=pc$ for some $c$, and $p=apc$ gives $1=ac$ by [multiplicative cancellation in an integral domain](../../../../multiplicative-cancellation-in-an-integral-domain.md). Thus $(a)=R$. This proves maximality.

Since $R$ is an [integral domain](../../../../integral-domain.md), $(0)$ is a [prime ideal](../../../../prime-ideal.md), and every other [prime ideal](../../../../prime-ideal.md) is maximal. Consequently every [prime chain](../../../../prime-chain.md) has length at most one. For the opposite inequality, choose a nonzero [nonunit](../../../../nonunit.md) $a$, which exists because $R$ is not a [field](../../../../field.md). The proper [principal ideal](../../../../principal-ideal.md) $(a)$ is contained in a [maximal ideal](../../../../maximal-ideal.md) $\mathfrak m$; existence follows from [Zorn's lemma](../../../../zorn-s-lemma.md) applied to the proper [ideals](../../../../ideal.md) containing $(a)$. A [maximal ideal](../../../../maximal-ideal.md) is a [prime ideal](../../../../prime-ideal.md), since its [quotient ring](../../../../quotient-ring.md) is a [field](../../../../field.md). Therefore $(0)\subsetneq\mathfrak m$ is a [prime chain](../../../../prime-chain.md) of length one. Thus the [Krull dimension of a principal ideal domain](../../../../krull-dimension-of-a-principal-ideal-domain.md) that is not a [field](../../../../field.md) is

$$
\boxed{\dim R=1.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
