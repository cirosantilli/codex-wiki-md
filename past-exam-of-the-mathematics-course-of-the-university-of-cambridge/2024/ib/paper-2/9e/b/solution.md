<h1 id="9e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The coefficient condition says precisely that every nonconstant monomial has positive powers of both variables. Thus

$$
R=K+XYK[X,Y].
$$

If $c+XYf$ and $d+XYg$ lie in $R$, so do their sum and their product

$$
cd+XY(cg+df+XYfg),
$$

so $R$ is a subring of $K[X,Y]$.

For $n\geq1$, let

$$
I_n=(XY,XY^2,\ldots,XY^n)_R.
$$

Then $I_n\subseteq I_{n+1}$. The containment is strict because $XY^{n+1}\notin I_n$: multiplying a generator $XY^j$ by an element of $R$ produces either a [scalar](../../../../../../scalar.md) multiple of $XY^j$, or terms divisible by $X^2$. It cannot produce the monomial $XY^{n+1}$ when $j\leq n$. Hence

$$
I_1\subsetneq I_2\subsetneq I_3\subsetneq\cdots
$$

is a strictly increasing [ideal](../../../../../../ideal.md) chain. The [constant-plus-ideal non-Noetherian subring](../../../../../../constant-plus-ideal-non-noetherian-subring.md) therefore satisfies

$$
\boxed{R\text{ is not Noetherian}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9E](../../9e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
