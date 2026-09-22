<h1 id="6d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [general linear group](../../../../../../general-linear-group.md) $GL_2(\mathbb F_5)$ consists of invertible two-by-two matrices over the [finite field](../../../../../../finite-field.md) $\mathbb F_5$, under [matrix multiplication](../../../../../../matrix-multiplication.md). Such a matrix has two [linearly independent](../../../../../../linear-independence.md) columns. There are $5^2-1=24$ choices for a nonzero first column, and $5^2-5=20$ choices for a second column outside its one-dimensional span. Thus

$$
\boxed{|GL_2(\mathbb F_5)|=24\cdot20=480.}
$$

The [determinant](../../../../../../determinant.md) is a [group homomorphism](../../../../../../group-homomorphism.md)

$$
\det:GL_2(\mathbb F_5)\longrightarrow\mathbb F_5^\times,
$$

where $\mathbb F_5^\times=\{1,2,3,4\}$ is the multiplicative [group](../../../../../../group-split.md) of nonzero field elements. It is surjective because $\operatorname{diag}(t,1)$ has [determinant](../../../../../../determinant.md) $t$. Its [kernel of a group homomorphism](../../../../../../kernel-of-a-group-homomorphism.md) is $SL_2(\mathbb F_5)$. The [first isomorphism theorem](../../../../../../first-isomorphism-theorem.md) gives a quotient of order four, whence

$$
\boxed{|SL_2(\mathbb F_5)|=480/4=120.}
$$

The nonzero squares form the [subgroup](../../../../../../subgroup.md) $\{1,4\}$ of $\mathbb F_5^\times$. Its inverse image

$$
\boxed{H=\{M\in GL_2(\mathbb F_5):\det M\in\{1,4\}\}}
$$

is a [subgroup](../../../../../../subgroup.md) with index two. Indeed, composing the [determinant](../../../../../../determinant.md) with the quotient map to $\mathbb F_5^\times/\{1,4\}$ makes $H$ the kernel of a surjective [group homomorphism](../../../../../../group-homomorphism.md) to a group of order two. Thus $|H|=240$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6D](../../6d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
