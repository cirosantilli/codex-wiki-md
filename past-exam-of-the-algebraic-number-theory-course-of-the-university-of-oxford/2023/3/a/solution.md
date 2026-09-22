<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $d_K$ denote the [field discriminant](../../../../field-discriminant.md), and put $n=[K:\mathbb Q]\geq2$. Let $r_1$ be the number of real [field embeddings](../../../../field-embedding.md) and $r_2$ the number of conjugate pairs of nonreal [field embeddings](../../../../field-embedding.md), so $n=r_1+2r_2$. The [Minkowski bound for ideal classes](../../../../minkowski-s-bound.md) provides a nonzero [integral ideal](../../../../integral-ideal.md) $A$ satisfying

$$
1\leq N(A)\leq\left(\frac4\pi\right)^{r_2}\frac{n!}{n^n}\sqrt{|d_K|}.
$$

Rearranging gives the [Minkowski lower bound for a number-field discriminant](../../../../minkowski-lower-bound-for-a-number-field-discriminant.md)

$$
|d_K|\geq\left(\frac\pi4\right)^{2r_2}\left(\frac{n^n}{n!}\right)^2.
$$

Because $2r_2\leq n$ and $\pi/4<1$, this is at least

$$
\left(\frac\pi4\right)^n\left(\frac{n^n}{n!}\right)^2.
$$

Apply the [arithmetic-geometric mean inequality](../../../../arithmetic-geometric-mean-inequality.md) to $1,2,\ldots,n$:

$$
n!\leq\left(\frac{n+1}{2}\right)^n.
$$

It follows that

$$
|d_K|\geq\left(\frac{\pi n^2}{(n+1)^2}\right)^n
\geq\left(\frac{4\pi}{9}\right)^n>1,
$$

where $n/(n+1)\geq2/3$ for $n\geq2$ was used. Thus

$$
\boxed{|d_K|>1}.
$$

The source writes $|\Delta(K)^2|>1$. If $\Delta(K)$ denotes the embedding [determinant](../../../../determinant.md), its square is $d_K$; if it denotes the [field discriminant](../../../../field-discriminant.md), the displayed result also implies the stated inequality. The conclusion therefore does not depend on that notational convention.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic number theory course of the University of Oxford](../../../split.md)
5. [Algebraic number theory course of the University of Oxford](../../../../algebraic-number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
