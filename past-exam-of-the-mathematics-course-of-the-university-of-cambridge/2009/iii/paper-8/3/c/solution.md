<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For every real $s$, the elementary weight estimate

$$
\langle m\rangle^s\leq C_s\langle m-l\rangle^{|s|}\langle l\rangle^s
$$

follows from $\langle x+y\rangle\leq\sqrt2\langle x\rangle\langle y\rangle$, using the reverse rearrangement for negative $s$. If $a$ is smooth its [Fourier coefficients](../../../../../../fourier-coefficient.md) decay faster than every power, so $c_j=\langle j\rangle^{|s|}|\widehat a(j)|$ is summable. The Fourier convolution formula and [Young convolution inequality](../../../../../../young-s-convolution-inequality.md) give

$$
\|au\|_s\leq C_s\|c\|_{\ell^1}\|u\|_s.
$$

Initially this holds for trigonometric polynomials, and density extends it to every $u\in H_s$, agreeing with distributional multiplication. Hence smooth multiplication preserves every order.

If $s>n/2$, the stronger estimate $\langle m\rangle^s\leq C_s(\langle l\rangle^s+\langle m-l\rangle^s)$ gives

$$
\|uv\|_s\leq C_s\left(\|u\|_s\|\widehat v\|_{\ell^1}+\|\widehat u\|_{\ell^1}\|v\|_s\right)
\leq C'_s\|u\|_s\|v\|_s,
$$

using the summability estimate from part (b) with $k=0$. Approximation extends the product, and the continuous embedding identifies it with the pointwise product. Completeness from part (a), this estimate and the constant unit make **$H_s$ a commutative [Sobolev algebra](../../../../../../sobolev-algebra.md) for $s>n/2$**. Rescaling the norm by $C'_s$ if necessary gives an equivalent strictly submultiplicative Banach-algebra norm.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
