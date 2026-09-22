<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here $w$ is the [harmonic replacement](../../../../../../harmonic-replacement.md) of $u$ in $B_r=B(x_0,r)$, so $v=u-w\in H_0^1(B_r)$. Subtract the weak equations and test with $v$:

$$
\int_{B_r}|\nabla v|^2
=\frac12\int_{B_r}x_1^2u_{x_1}v_{x_1}+\int_{B_r}fv.
$$

Because $B_r\subset B(0,1)$, $|x_1|\leq1$. The [Sobolev inequality](../../../../../../sobolev-inequality.md) $\|v\|_6\leq C\|\nabla v\|_2$ and the [Holder inequality](../../../../../../holder-inequality.md) give

$$
\|\nabla v\|_2^2
\leq\frac12\|\nabla u\|_2\|\nabla v\|_2
+C\|f\|_{6/5}\|\nabla v\|_2.
$$

After division and squaring,

$$
\boxed{\int_{B_r}|\nabla v|^2
\leq C_1\int_{B_r}|\nabla u|^2
+C_2\left(\int_{B_r}|f|^{6/5}\right)^{5/3}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
