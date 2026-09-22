<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $E[q^\infty]$ for the points killed by some power of $q$, rather than any notion of all points which are $q$-divisible. On the reduction kernel, formal multiplication is

$$
[q^m](t)=q^mt+O(t^2).
$$

Since $q\ne p$, its linear coefficient is a unit. Recursive inversion gives an integral inverse series, convergent on $p\mathbb Z_p$; equivalently the [Hensel lemma](../../../../../../hensel-s-lemma.md) gives a unique solution to $[q^m](t)=s$ for every $s\in p\mathbb Z_p$. Thus multiplication by $q^m$ is bijective on the kernel, proving that its $q$-primary torsion is zero. The reduction [group homomorphism](../../../../../../group-homomorphism.md) is therefore injective on $E(\mathbb Q_p)[q^\infty]$.

For surjectivity on this torsion, take a reduced point $\widetilde P$ killed by $q^m$. Lift it to $P\in E(\mathbb Q_p)$ using smooth reduction. Then $q^mP$ belongs to the kernel, so choose its unique kernel division point $R$ with $q^mR=q^mP$. The point $P-R$ is killed by $q^m$ and reduces to $\widetilde P$. This proves the [prime-to-p torsion lifts uniquely at good reduction](../../../../../../prime-to-p-torsion-lifts-uniquely-at-good-reduction.md) statement:

$$
\boxed{E(\mathbb Q_p)[q^\infty]\xrightarrow{\sim}\widetilde E(\mathbb F_p)[q^\infty].}
$$

The right side is a subgroup of a [finite group](../../../../../../finite-group.md). Thus the left side is finite and has exactly the requested order. No claim that the whole formal kernel is torsion-free at $p=2$ is needed.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
