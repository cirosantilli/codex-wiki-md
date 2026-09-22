<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

By the [canonical colimit presentation of a presheaf](../../../../../../canonical-colimit-presentation-of-a-presheaf.md), write

$$
P=\operatorname{colim}_{(c,x)\in\int P}H_c
$$

with structure maps $\alpha_{c,x}:H_c\to P$. Since $P$ is a [0-presentable object](../../../../../../small-projective-object.md), the canonical map

$$
\operatorname{colim}_{(c,x)}\operatorname{Nat}(P,H_c)\longrightarrow\operatorname{Nat}(P,P)
$$

is bijective. Every element of a set-valued [colimit](../../../../../../colimit.md) has a representative in some component. In particular $1_P$ is the image of a transformation $s:P\to H_c$ for some $(c,x)$, so

$$
\alpha_{c,x}s=1_P.
$$

Thus $P$ is a retract of $H_c$. The [representable retract criterion](../../../../../../representable-retract-criterion.md) from part (c), using the assumed [equalisers](../../../../../../equaliser.md) in $\mathcal C$, now gives **$P$ is [representable](../../../../../../representable-functor.md)**. Only existence of the representative of $1_P$ is needed; no stronger uniqueness-of-factorization assertion about individual [colimit](../../../../../../colimit.md) injections has been assumed.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
