<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [descending chain condition](../../../../../../descending-chain-condition.md) on the finite intersections of [maximal right ideals](../../../../../../maximal-right-ideal.md). It gives a minimal such intersection $K=M_1\cap\cdots\cap M_r$. Intersecting $K$ with any other [maximal right ideal](../../../../../../maximal-right-ideal.md) cannot decrease it, by minimality. Thus $K$ lies in every [maximal right ideal](../../../../../../maximal-right-ideal.md), and $K=J(R)$. When $J(R)=0$, the diagonal map

$$
R_R\longrightarrow\bigoplus_{i=1}^rR/M_i,\qquad a\longmapsto(a+M_i)_i
$$

is injective, and each summand on the right is a [simple module](../../../../../../irreducible-module.md).

For completeness, a submodule $N$ of a finite direct sum of [simple modules](../../../../../../irreducible-module.md) is semisimple. Induct on the number of summands. For $S\oplus T$ with $S$ simple, $N\cap S$ is either $0$ or $S$. In the first case projection into $T$ identifies $N$ with a submodule of $T$, so induction applies. In the second case subtracting the $S$ coordinate shows $N=S\oplus(N\cap T)$, and induction again applies. This also shows finite [module length](../../../../../../length-of-a-module.md). Apply it to the image of the diagonal map to obtain

$$
\boxed{J(R)=0\text{ and }R\text{ right Artinian}\Longrightarrow R_R\text{ semisimple}.}
$$

This is the [semisimplicity of a right Artinian ring with zero radical](../../../../../../semisimplicity-of-a-right-artinian-ring-with-zero-radical.md). It does not assume right Noetherianity in order to prove it.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
