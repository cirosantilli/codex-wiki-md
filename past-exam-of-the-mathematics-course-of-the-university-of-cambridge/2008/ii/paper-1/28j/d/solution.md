<h1 id="28j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $\phi=\Phi'$ for the standard [normal density](../../../../../../normal-density.md). Differentiating the [Black-Scholes formula](../../../../../../black-scholes-formula.md) and using $S_0\phi(d_1)=Ke^{-rT}\phi(d_2)$ gives

$$
\frac{\partial C}{\partial\sigma}
=S_0\phi(d_1)\left(\frac{\partial d_1}{\partial\sigma}-\frac{\partial d_2}{\partial\sigma}\right)
=\boxed{S_0\sqrt T\,\phi(d_1)>0}.
$$

The last equality follows by differentiating $d_1-d_2=\sigma\sqrt T$. This derivative is the option's [vega](../../../../../../option-vega.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [28J](../../28j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
