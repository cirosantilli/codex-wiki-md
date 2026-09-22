<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Strengthened Van der Waerden theorem](../../../../../../strengthened-van-der-waerden-theorem.md) says that every finite coloring contains, for each prescribed $m$, a monochromatic set

$$
\{d,a,a+d,\ldots,a+(m-1)d\}.
$$

We prove the finite form by induction on the number $k$ of colors. The case $k=1$ is immediate. Let $n$ work for $m$ and $k-1$ colors, and apply the ordinary [Van der Waerden theorem](../../../../../../van-der-waerden-theorem.md) to obtain a monochromatic progression

$$
a,a+d,\ldots,a+n(m-1)d.
$$

If one of $d,2d,\ldots,nd$ has the progression's color, say $rd$, then

$$
rd,a,a+rd,\ldots,a+(m-1)rd
$$

works. Otherwise $d,2d,\ldots,nd$ use at most $k-1$ colors. By the induction hypothesis their indices contain $b,b+r,\ldots,b+(m-1)r$ together with $r$ in one color. Multiplying by $d$ yields

$$
rd,bd,(b+r)d,\ldots,(b+(m-1)r)d,
$$

which is the required progression together with its [common difference](../../../../../../common-difference.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
