<h1 id="23k/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Poisson thinning theorem](../../../../../../poisson-thinning-theorem.md), or its multinomial marking version, makes the bin counts at time $n$ independent Poisson variables with mean $n/n=1$. Independence is more than is needed for the following [union bound](../../../../../../boole-s-inequality.md). Fix $\epsilon>0$ and put $x_n=(1+\epsilon)\log n/\log\log n$. Then

$$
\mathbb P(M_n\geq x_n)\leq n\exp(x_n-x_n\log x_n).
$$

Since

$$
\log x_n=\log\log n-\log\log\log n+\log(1+\epsilon),
$$

the logarithm of the upper bound is $-\epsilon\log n+o(\log n)\to-\infty$. Thus **$\boxed{\mathbb P(M_n\geq x_n)\to0}$**. The estimate handles the noninteger threshold directly, since the supplied Poisson tail bound holds for real $x$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [23K](../../23k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
