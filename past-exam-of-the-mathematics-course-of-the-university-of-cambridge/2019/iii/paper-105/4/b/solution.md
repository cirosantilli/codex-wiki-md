<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $Lu=L_0u+(a^{ij}-A^{ij})D_{ij}u$, with repeated indices summed. The [triangle inequality](../../../../../../triangle-inequality.md) and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) over the $n^2$ coefficient pairs give

$$
\begin{aligned}
\|Lu\|_2
&\geq\|L_0u\|_2-\left\|\sum_{i,j}(a^{ij}-A^{ij})D_{ij}u\right\|_2\\
&\geq\theta\|D^2u\|_2-n\varepsilon\|D^2u\|_2.
\end{aligned}
$$

Choose

$$
\boxed{\varepsilon=\frac{\theta}{2n}.}
$$

Then the strict coefficient bound in the question implies

$$
\boxed{\frac\theta2\|D^2u\|_{L^2(B_r(x_0))}\leq\|Lu\|_{L^2(B_r(x_0))}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
