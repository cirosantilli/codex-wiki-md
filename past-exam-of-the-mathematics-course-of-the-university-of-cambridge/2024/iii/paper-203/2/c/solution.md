<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $z=x+iy$ with $|x|\leq1$ and $0<y\leq1$, the given [Reverse SLE derivative martingale](../../../../../../reverse-sle-derivative-martingale.md) starts from

$$
M_0=\left(1+\frac{x^2}{y^2}\right)^{4/\kappa}\leq C_0y^{-8/\kappa}.
$$

It is a nonnegative local martingale and therefore a [supermartingale](../../../../../../supermartingale.md). Since its second factor is at least one,

$$
\mathbb E|h_T'(x+iy)|^2\leq\mathbb E M_T\leq C_0y^{-8/\kappa}.
$$

Choose

$$
0<\alpha<\frac12\left(1-\frac8\kappa\right),
$$

which is possible exactly because $\kappa>8$. At height $y_n=2^{-n}$, take a horizontal grid of spacing comparable to $y_n$ in $[-1,1]$. The [Markov inequality](../../../../../../markov-inequality.md) gives, at each grid point,

$$
\mathbb P\bigl(|h_T'(z)|>y_n^{-1+\alpha}\bigr)\leq C y_n^{2-2\alpha-8/\kappa}.
$$

There are $O(y_n^{-1})$ grid points, so the probability that the bound fails anywhere on level $n$ is at most $Cy_n^{1-2\alpha-8/\kappa}$. These probabilities are summable. The [Borel-Cantelli lemmas](../../../../../../borel-cantelli-lemmas.md) therefore give an almost surely finite random constant controlling every sufficiently fine grid, and enlarging it handles the finitely many remaining levels.

Every point of the half-rectangle lies within a fixed hyperbolic distance of one of these grid points at comparable height. The [Koebe distortion theorem](../../../../../../koebe-distortion-theorem.md) compares the two derivatives by a universal factor. Hence an almost surely finite random $C$ satisfies

$$
|h_T'(x+iy)|\leq Cy^{-1+\alpha}
$$

for all $x\in[-1,1]$ and $0<y\leq1$. This proves the [Reverse SLE derivative bound above the space-filling threshold](../../../../../../reverse-sle-derivative-bound-above-the-space-filling-threshold.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
