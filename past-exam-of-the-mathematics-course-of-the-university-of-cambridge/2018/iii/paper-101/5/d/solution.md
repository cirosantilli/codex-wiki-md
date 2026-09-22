<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take

$$
\boxed{D=\mathbb Z[\sqrt{-5}].}
$$

We justify that this is a [Dedekind domain](../../../../../../dedekind-domain.md). It is an [integral domain](../../../../../../integral-domain.md) inside the [number field](../../../../../../number-field.md) $K=\mathbb Q(\sqrt{-5})$. As an additive group it is free of rank two over $\mathbb Z$. The subgroup theorem for [finitely generated abelian groups](../../../../../../finitely-generated-abelian-group.md) says that every subgroup of such a group is finitely generated. Thus every [ideal](../../../../../../ideal.md) has finitely many additive generators, and those same elements generate it as a $D$-ideal. This proves that $D$ is [Noetherian](../../../../../../noetherian-ring.md).

We use the standard formula for the [ring of integers of a quadratic field](../../../../../../ring-of-integers-of-a-quadratic-field.md): for squarefree $d$, it is $\mathbb Z[(1+\sqrt d)/2]$ if $d\equiv1\pmod4$, and $\mathbb Z[\sqrt d]$ otherwise. Since $-5\equiv3\pmod4$, $D$ is the [ring of integers of a number field](../../../../../../ring-of-integers.md) $K$, meaning all elements of $K$ integral over $\mathbb Z$. We also use transitivity of [integral extensions](../../../../../../integral-extension.md). If an element of $K$ is integral over $D$, it is integral over $\mathbb Z$ because $D$ is integral over $\mathbb Z$, and therefore belongs to $D$. Thus $D$ is an [integrally closed domain](../../../../../../integrally-closed-domain.md).

Every nonzero [prime ideal](../../../../../../prime-ideal.md) $P$ is maximal. Indeed, choose $0\ne\alpha=a+b\sqrt{-5}\in P$. Multiplying by its [algebraic conjugate](../../../../../../conjugate-element-field-theory.md) puts the nonzero integer $N(\alpha)=a^2+5b^2$ in $P$. Hence the [integral domain](../../../../../../integral-domain.md) $D/P$ is a quotient of the finite [ring](../../../../../../ring.md) $D/N(\alpha)D$, and is finite. Every finite [integral domain](../../../../../../integral-domain.md) is a [field](../../../../../../field.md), since multiplication by a nonzero element is injective and therefore surjective. The element $2$ has no inverse in $D$, since $1/2\notin\mathbb Z[\sqrt{-5}]$, so $D$ is not a [field](../../../../../../field.md). Consequently $(0)$ is not maximal, and a [maximal ideal](../../../../../../maximal-ideal.md) above it is nonzero. Together with the preceding result, this gives [Krull dimension](../../../../../../krull-dimension.md) exactly one.

Finally, consider the [ideal](../../../../../../ideal.md)

$$
I=(2,1+\sqrt{-5}).
$$

Reduction modulo $2$ with $\sqrt{-5}\mapsto1$ identifies $D/I$ with $\mathbb F_2$, so the additive index $[D:I]$ is $2$. If $I$ were the [principal ideal](../../../../../../principal-ideal.md) $(a+b\sqrt{-5})$, multiplication by its nonzero generator would have integer matrix

$$
\begin{pmatrix}a&-5b\\b&a\end{pmatrix}
$$

in the basis $1,\sqrt{-5}$. The index of its image is the absolute determinant, so

$$
2=[D:I]=a^2+5b^2.
$$

There are no integer solutions: $b\ne0$ makes the right side at least $5$, while $b=0$ would require $a^2=2$. Thus $I$ is a [nonprincipal ideal in the integers adjoined a square root of minus five](../../../../../../nonprincipal-ideal-in-the-integers-adjoined-a-square-root-of-minus-five.md), and **$D$ is a Dedekind domain that is not a principal ideal domain**.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
