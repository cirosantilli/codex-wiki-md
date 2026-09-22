<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

The numbers $z_j$ are the nonzero [zeros of a function](../../../../../zero-of-a-function.md) $f$, repeated according to their [multiplicity](../../../../../multiplicity-mathematics.md). The displayed [Weierstrass factorization theorem](../../../../../weierstrass-factorization-theorem.md) formula uses genus-one [Weierstrass elementary factors](../../../../../weierstrass-elementary-factor.md) and a linear exponential factor; it applies under the corresponding growth assumptions, rather than to every arbitrary entire function.

Apply it to the [entire function](../../../../../entire-function.md) $g(z)=\sin(\pi z)/(\pi z)$, with its removable value $g(0)=1$. Its zeros are $\pm1,\pm2,\ldots$, each simple, and $g'(0)=0$ because $g$ is even. Pairing the factors at $n$ and $-n$ gives

$$
(1-z/n)e^{z/n}(1+z/n)e^{-z/n}=1-z^2/n^2,
$$

so

$$
\boxed{\frac{\sin(\pi z)}{\pi z}=\prod_{n=1}^{\infty}\left(1-\frac{z^2}{n^2}\right).}
$$

The product converges uniformly on compact subsets because $\sum n^{-2}<\infty$. Away from the integers its [logarithmic derivative](../../../../../logarithmic-derivative.md) can be taken term by term: the resulting series also converges locally uniformly, its terms being $O(n^{-2})$. Hence

$$
\pi\cot(\pi z)-\frac1z=\sum_{n=1}^{\infty}\frac{-2z/n^2}{1-z^2/n^2},\qquad
\boxed{\pi\cot(\pi z)=\frac1z+2\sum_{n=1}^{\infty}\frac{z}{z^2-n^2}.}
$$

This is an identity of [meromorphic functions](../../../../../meromorphic-function.md), understood away from their poles.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
