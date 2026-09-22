<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The half-open translates $[-\pi,\pi)+2\pi k$ partition the real line. Exactly one summand is therefore nonzero in the periodization of $|f|^2$, giving $\sum_k|f(t+2\pi k)|^2=1$.

Choose the [Shannon scaling mask](../../../../../../shannon-scaling-mask.md) to be the $2\pi$-periodic extension of $\mathbf1_{[-\pi/2,\pi/2)}$. On the [support](../../../../../../support.md) of $f$, its product with $f$ is $\mathbf1_{[-\pi/2,\pi/2)}(t)=f(2t)$; outside that [support](../../../../../../support.md) both sides vanish. Thus the [scaling refinement equation](../../../../../../scaling-refinement-equation.md) holds in frequency. The [Fourier coefficients](../../../../../../fourier-coefficient.md) give its precise filter normalization:

$$
a_n=\frac1\pi\int_{-\pi/2}^{\pi/2}e^{int}\,dt
=\begin{cases}1,&n=0,\\\dfrac{2\sin(n\pi/2)}{\pi n},&n\ne0.\end{cases}
$$

These [coefficients](../../../../../../coefficient.md) are square summable, so the interpretation in part (b) applies.

The [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md) gives the [Shannon scaling function](../../../../../../shannon-scaling-function.md)

$$
\phi(x)=\frac1{2\pi}\int_{-\pi}^{\pi}e^{ixt}\,dt,
\qquad\boxed{\phi(x)=\frac{\sin(\pi x)}{\pi x}\ (x\ne0),\qquad\phi(0)=1.}
$$

This is the normalized [sinc function](../../../../../../sinc-function.md). Its [Fourier transform](../../../../../../fourier-transform.md) is taken in the [Plancherel theorem](../../../../../../plancherel-theorem.md) sense: the [Shannon scaling function](../../../../../../shannon-scaling-function.md) belongs to $L^2$ but not $L^1$, so its Fourier integral is not absolutely convergent. The inverse integral above is an ordinary integral because the rectangular transform belongs to $L^1$. The resulting refinement spaces are exactly the $L^2$ [functions](../../../../../../function-split.md) with [Fourier transform](../../../../../../fourier-transform.md) supported in $[-2^j\pi,2^j\pi]$; their union is [dense](../../../../../../dense-set.md) and their intersection is zero. Thus this example also gives a full [multiresolution analysis](../../../../../../multiresolution-analysis.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
