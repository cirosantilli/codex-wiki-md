<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Interpret the given velocity regularity in the stated [Sobolev space](../../../../../../sobolev-space-split.md) sense. Repeated [integration by parts](../../../../../../integration-by-parts.md), or the [Fourier transform of a derivative](../../../../../../fourier-transform-of-a-derivative.md) in distributions, gives

$$
 (2\pi i\xi)^{n+1}\widehat f_0(k,\xi)
 =\widehat{\partial_v^{n+1}f_0}(k,\xi).
$$

The usual one-dimensional [one-dimensional Sobolev representative](../../../../../../one-dimensional-sobolev-representative.md) or a smooth approximation justifies this identity without imposing extra decay of classical derivatives at specific boundary points. The transform of an integrable function has absolute value at most its $L^1$ [norm](../../../../../../norm.md). Therefore

$$
 |\widehat f_0(k,\xi)|\,|\xi|^{n+1}
 \leq\frac{\|\partial_v^{n+1}f_0\|_1}{(2\pi)^{n+1}}
 \leq\frac{\|f_0\|_{L_x^1W_v^{n+1,1}}}{(2\pi)^{n+1}}.
$$

Setting $\xi=kt$ and taking the supremum gives the required **uniform weighted bound**. The $k=0$ term on the left is zero; there is no division by that frequency in this argument.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
