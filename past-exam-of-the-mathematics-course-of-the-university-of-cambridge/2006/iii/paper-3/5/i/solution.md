<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an arbitrary [subgroup](../../../../../../subgroup.md) $A$, the full inverse image of its image is $AK$, not generally $A$. In fact, $\theta(g)\in\theta(A)$ exactly when $g=ak$ for some $a\in A,k\in K$. Since $K$ is normal, $AK$ is a [subgroup](../../../../../../subgroup.md). By the [subgroup correspondence for a surjective group homomorphism](../../../../../../subgroup-correspondence-for-a-surjective-group-homomorphism.md),

$$
[H:\theta(A)]=[G:AK].
$$

Multiplicativity of finite index gives

$$
[G:A]=[G:AK][AK:A].
$$

The map $k(K\cap A)\mapsto kA$ bijects the left [cosets](../../../../../../coset.md) of $K\cap A$ in $K$ with those of $A$ in $AK$, since $AK=KA$. Consequently

$$
\boxed{[H:\theta(A)]=\frac{i}{[K:K\cap A]}.}
$$

This need not equal $i$. For example, take $\theta:\mathbb Z\to\mathbb Z/2\mathbb Z$ to be reduction modulo $2$ and $A=3\mathbb Z$. Then $[G:A]=3$, but $\theta(A)=H$ has index one. If $A$ contains $K$, however, the denominator is one and

$$
\boxed{K\leq A\ \Longrightarrow\ [H:\theta(A)]=i.}
$$

For finite $i$, equality holds exactly when $K\leq A$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
