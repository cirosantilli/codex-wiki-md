<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a [self-adjoint C-star element](../../../../../../hermitian-element-of-a-c-star-algebra.md) $h$, the [C-star identity](../../../../../../c-star-identity.md) gives $\|h^2\|=\|h\|^2$. If $x$ is a [normal C-star element](../../../../../../normal-element-of-a-c-star-algebra.md), then

$$
\|x^2\|^2=\|(x^*)^2x^2\|=\|(x^*x)^2\|=\|x^*x\|^2=\|x\|^4.
$$

All powers are [normal C-star elements](../../../../../../normal-element-of-a-c-star-algebra.md), so induction gives $\|x^{2^j}\|=\|x\|^{2^j}$. The general [spectral radius formula](../../../../../../spectral-radius-formula.md) now gives $r(x)=\|x\|$.

One can also see the needed growth estimate directly. For $R>r(x)$ the [resolvent Cauchy coefficient formula](../../../../../../resolvent-cauchy-coefficient-formula.md) gives

$$
x^m=\frac1{2\pi i}\int_{|z|=R}z^m(z1-x)^{-1}\,dz,\qquad\|x^m\|\le C_RR^{m+1}.
$$

The formula follows by the [Neumann series](../../../../../../neumann-series.md) on a larger circle and [contour deformation](../../../../../../contour-deformation.md) through the resolvent annulus. Put $m=2^j$, take $m$th roots and let $j\to\infty$ to get $\|x\|\le R$. Let $R\downarrow r(x)$; the reverse inequality already follows from the [norm](../../../../../../norm.md) bound on the [algebra spectrum](../../../../../../spectrum-of-an-element.md). Thus

$$
\boxed{r(x)=\|x\|}.
$$

This proves [spectral radius norm equality for normal elements](../../../../../../spectral-radius-norm-equality-for-normal-elements.md) from the [norm](../../../../../../norm.md) identity.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
