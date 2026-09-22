<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [covariant density presentation](../../../../../../covariant-density-presentation.md). An object of $\int F$ is $(c,x)$ with $x\in Fc$; an arrow $(c,x)\to(d,y)$ is $u:c\to d$ with $F(u)x=y$. For each such object the [Yoneda lemma](../../../../../../yoneda-lemma.md) gives a [natural transformation](../../../../../../natural-transformation.md) $\mathcal C(c,-)\to F$. An arrow $u$ induces $\mathcal C(d,-)\to\mathcal C(c,-)$ by precomposition, so these transformations form a cocone indexed by $(\int F)^{\mathrm{op}}$.

At $a$, send a representative $(c,x,v:c\to a)$ to $F(v)x$. Every $z\in Fa$ comes from $(a,z,1_a)$. If two representatives have the same value $z$, their arrows to $(a,z)$ in $\int F$ identify both with that same representative in the opposite-indexed colimit. Thus the map is bijective and natural, proving

$$
\boxed{F\cong\operatorname{colim}_{(c,x)\in(\int F)^{\mathrm{op}}}\mathcal C(c,-).}
$$

The index is small because $\mathcal C$ is small and every $Fc$ is a set. By (iii) it is a [filtered category](../../../../../../filtered-category.md). This proves (iv).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Section B](../../section-b.md)
4. [Paper 23](../../../paper-23-split.md)
5. [Iii](../../../split.md)
6. [2004](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)

## ← Incoming links (1)

- [Solution](../solution.md)
