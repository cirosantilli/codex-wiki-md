<h1 id="20f/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

If the bounded [injective](../../../../../../injective-function.md) [Fourier transform](../../../../../../fourier-transform.md) $L^1\to C_0$ were surjective, the [open mapping theorem](../../../../../../open-mapping-theorem-functional-analysis.md) for [Banach spaces](../../../../../../banach-space-split.md) would make its inverse bounded, yielding $\|h\|_1\leq C\|\widehat h\|_\infty$. But the preceding $g_n$ have [uniform norm](../../../../../../supremum-norm.md) $2$, whereas $\|h_n\|_1$ diverges.

For a quantitative lower bound, on $0<x\leq1/4$ we have $\sin(2\pi x)\geq4x$. On each interval $I_j=[(j+1/12)/n,(j+5/12)/n]$, $|\sin(2\pi n x)|\geq1/2$. For $1\leq j\leq\lfloor n/8\rfloor$ these intervals lie below $1/4$ for large $n$, so

$$
 \|h_n\|_1\geq\frac2{\pi^2}\sum_j\int_{I_j}\frac{dx}{x}
 \geq\frac{2}{3\pi^2}\sum_{j=1}^{\lfloor n/8\rfloor}\frac1{j+5/12}\longrightarrow\infty.
$$

This contradicts boundedness of the inverse. Therefore **the [Fourier transform](../../../../../../fourier-transform.md) has proper dense image in $C_0(\mathbb R)$**.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [20F](../../20f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
