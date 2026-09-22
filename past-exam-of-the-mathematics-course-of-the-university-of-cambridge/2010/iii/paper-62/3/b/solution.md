<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume $n\ge1$ and $\|p\|_{[-1,1]}\le1$. The given [Bernstein inequality for algebraic polynomials](../../../../../../bernstein-inequality-for-algebraic-polynomials.md) shows that $q=p'$ satisfies the nodal hypotheses of (a). Consequently, in the two endpoint regions $\cos(\pi/(2n))\le|x|\le1$, $|p'(x)|\le|T_n'(x)|$.

For $0<\theta<\pi$, the finite geometric identity

$$
\frac{\sin(n\theta)}{\sin\theta}=\sum_{r=0}^{n-1}e^{i(n-1-2r)\theta}
$$

bounds its absolute value by $n$. It follows that $|T_n'(\cos\theta)|\le n^2$, and the endpoint limit gives $T_n'(1)=n^2$. In the central interval, the [Bernstein inequality for algebraic polynomials](../../../../../../bernstein-inequality-for-algebraic-polynomials.md) gives

$$
|p'(x)|\le\frac{n}{\sqrt{1-x^2}}\le\frac{n}{\sin(\pi/(2n))}\le n^2,
$$

since $\sin t\ge2t/\pi$ on $[0,\pi/2]$. Combining the regions and rescaling proves the [Markov inequality for polynomial derivatives](../../../../../../markov-inequality-for-polynomial-derivatives.md):

$$
\boxed{\|p'\|_{[-1,1]}\le n^2\|p\|_{[-1,1]},\qquad T_n'(1)=n^2.}
$$

The [Chebyshev polynomial](../../../../../../chebyshev-polynomial.md) itself attains equality, so this constant is sharp. Constant [polynomials](../../../../../../polynomial-split.md) have zero [derivative](../../../../../../derivative.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
