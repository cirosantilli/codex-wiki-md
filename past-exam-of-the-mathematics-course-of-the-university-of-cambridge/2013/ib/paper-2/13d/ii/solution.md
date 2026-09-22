<h1 id="13d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On the top side put $z=x+i\pi$, with $x$ running from $R$ to $-R$. Since $e^{i(x+i\pi)^2/\pi}=-e^{ix^2/\pi}e^{-2x}$ and $e^{-2(x+i\pi)}=e^{-2x}$, the reversed orientation cancels the minus sign. The two horizontal integrals therefore sum to

$$
\int_{-R}^R e^{ix^2/\pi}\left(\frac1{1+e^{-2x}}+\frac{e^{-2x}}{1+e^{-2x}}\right)dx
=\int_{-R}^R e^{ix^2/\pi}\,dx.
$$

If the vertical contributions vanish, the previous [residue theorem](../../../../../../residue-theorem.md) evaluation yields the [Fresnel integral](../../../../../../fresnel-integral.md)

$$
\boxed{\int_{-\infty}^{\infty}e^{ix^2/\pi}\,dx=\frac{\pi(1+i)}{\sqrt2}.}
$$

This also is an ordinary oscillatory [improper integral](../../../../../../improper-integral.md), not merely a symmetric principal value: [integration by parts](../../../../../../integration-by-parts.md), using $(e^{ix^2/\pi})'=(2ix/\pi)e^{ix^2/\pi}$, bounds either tail beginning at $R$ by a constant times $1/R$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [13D](../../13d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
