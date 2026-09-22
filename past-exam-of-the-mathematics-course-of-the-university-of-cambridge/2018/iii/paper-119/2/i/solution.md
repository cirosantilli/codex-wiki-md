<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\lambda_A:GF(A)\to Z$ be the given [cocone under a diagram](../../../../../../cocone-under-a-diagram.md). For $B\in\mathcal D$, choose an object $(A,u:B\to FA)$ of the [comma category](../../../../../../comma-category.md) $(B\downarrow F)$ and define

$$
\bar\lambda_B=\lambda_A G(u):GB\to Z.
$$

Such a choice exists because $F$ is a [final functor](../../../../../../final-functor.md). If $a:A\to A'$ gives a morphism $(A,u)\to(A',u')$, so $F(a)u=u'$, the cocone relation gives

$$
\lambda_{A'}G(u')=\lambda_{A'}GF(a)G(u)=\lambda_AG(u).
$$

The [connected category](../../../../../../connected-category.md) condition makes the result independent of the choice along any zigzag.

For $v:B\to B'$, choose $(A,u:B'\to FA)$; then $(A,uv)$ is available for $B$, giving $\bar\lambda_B=\bar\lambda_{B'}G(v)$. Thus the maps form a [cocone under a diagram](../../../../../../cocone-under-a-diagram.md) on $G$. Choosing $(A,1_{FA})$ shows that restriction recovers $\lambda_A$. Any extension must satisfy $\bar\lambda_B=\bar\lambda_{FA}G(u)=\lambda_AG(u)$, proving uniqueness. This is [cocone extension along a final functor](../../../../../../cocone-extension-along-a-final-functor.md).

If $GF$ has a [colimit](../../../../../../colimit.md), extend its universal cocone in this way. Every cocone on $G$ restricts to one on $GF$, factors uniquely through that colimit, and then agrees with its extension by uniqueness. Hence the same vertex is a colimit of $G$. In particular,

$$
\boxed{\operatorname{colim}_{\mathcal D}G\cong\operatorname{colim}_{\mathcal C}GF,}
$$

and existence of all $\mathcal C$-shaped colimits in $\mathcal E$ implies existence of all $\mathcal D$-shaped colimits.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
