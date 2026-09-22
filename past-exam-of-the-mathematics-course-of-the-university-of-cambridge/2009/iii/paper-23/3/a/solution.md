<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $H_c=\mathcal C(-,c)$. The [category of elements](../../../../../../category-of-elements.md) $\int P$ of a [categorical presheaf](../../../../../../presheaf-category-theory.md) $P$ has objects $(c,x)$ with $x\in P(c)$; a [morphism](../../../../../../morphism.md) $(c,x)\to(d,y)$ is $u:c\to d$ satisfying $P(u)y=x$. It is a [small category](../../../../../../small-category.md) because $\mathcal C$ is small and each $P(c)$ is a [set](../../../../../../set-split.md). Consider the diagram sending $(c,x)$ to $H_c$ and $u$ to the [natural transformation](../../../../../../natural-transformation.md) given by postcomposition with $u$.

There is a canonical cocone $\alpha_{c,x}:H_c\to P$ with

$$
(\alpha_{c,x})_a(v)=P(v)x\qquad(v:a\to c).
$$

Functoriality makes it a [natural transformation](../../../../../../natural-transformation.md), and the equation $P(u)y=x$ makes these transformations a cocone.

To prove its [universal property](../../../../../../universal-property.md), let $Q$ be any [categorical presheaf](../../../../../../presheaf-category-theory.md) with a compatible cocone $\beta_{c,x}:H_c\to Q$. Define

$$
t_c(x)=(\beta_{c,x})_c(1_c).
$$

For $u:c\to d$ and $y\in P(d)$, compatibility with the arrow $(c,P(u)y)\to(d,y)$ gives

$$
t_c(P(u)y)=(\beta_{d,y})_c(u)=Q(u)(\beta_{d,y})_d(1_d)=Q(u)t_d(y).
$$

Thus $t:P\to Q$ is natural. [Naturality](../../../../../../naturality.md) of each $\beta_{c,x}$ shows $t\alpha_{c,x}=\beta_{c,x}$. Conversely any transformation with these equations must have the displayed values $t_c(x)$, so it is unique. We have proved the [canonical colimit presentation of a presheaf](../../../../../../canonical-colimit-presentation-of-a-presheaf.md):

$$
\boxed{P\cong\operatorname{colim}_{(c,x)\in\int P}H_c.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
