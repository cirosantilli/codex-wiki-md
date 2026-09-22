<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $L_i=\lambda_i+k-i$, for $1\leq i\leq k$. These are distinct nonnegative integers with $L_1>\cdots>L_k$. Using the [falling factorial](../../../../../../falling-factorial.md), the matrix entry can be written

$$
\frac1{(\lambda_i-i+j)!}
=\frac{(L_i)_{k-j}}{L_i!}.
$$

When $k-j>L_i$, the falling factorial vanishes, agreeing with the stipulated convention for a negative factorial argument.

The column [polynomials](../../../../../../polynomial-split.md) $(X)_{k-1},(X)_{k-2},\ldots,(X)_0$ are monic of successive descending degrees. Subtracting lower-degree combinations of columns turns them into $X^{k-1},X^{k-2},\ldots,1$ without changing the [determinant](../../../../../../determinant.md). The [Vandermonde determinant](../../../../../../vandermonde-determinant.md) therefore gives

$$
\det\left(\frac1{(\lambda_i-i+j)!}\right)
=\frac{\prod_{i<j}(L_i-L_j)}{\prod_iL_i!}.
$$

The positive sign comes from reversing the usual increasing-degree Vandermonde columns at the same time as writing the differences as $L_i-L_j$.

We now match this denominator with the [hook-length formula](../../../../../../hook-length-formula.md). The [hook lengths](../../../../../../hook-length.md) in row $i$ are precisely

$$
\{1,2,\ldots,L_i\}\setminus\{L_i-L_r:r>i\}.
$$

To verify the claim, the first hook in the row has length $L_i$. As the column index passes from $j$ to $j+1$, its [hook length](../../../../../../hook-length.md) drops by $1$ plus the number of lower rows ending at column $j$. The skipped lengths are exactly $L_i-L_r$ for those rows: if $\lambda_r=j$, then $L_i-L_r=\lambda_i-j+r-i$. At the right-hand end, lower rows having the same length as row $i$ account for the missing smallest lengths by the same formula. This describes all omitted values, and the remaining count is $L_i-(k-i)=\lambda_i$.

Consequently

$$
\prod_{x\in\lambda}h(x)
=\prod_i\frac{L_i!}{\prod_{r>i}(L_i-L_r)}
=\frac{\prod_iL_i!}{\prod_{i<j}(L_i-L_j)}.
$$

Combining the two identities with the [hook-length formula](../../../../../../hook-length-formula.md) proves **the determinantal dimension formula**

$$
\boxed{f_\lambda=n!\det\left(\frac1{(\lambda_i-i+j)!}\right)}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
