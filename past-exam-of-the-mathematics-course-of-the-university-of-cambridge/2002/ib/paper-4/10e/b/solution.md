<h1 id="10e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Continuity on the compact product of unit spheres bounds the [bilinear map](../../../../../../bilinear-map.md): there is $C$ such that $\|f(h,k)\|_3\le C\|h\|_1\|k\|_2$. This follows by scaling each nonzero vector to unit [norm](../../../../../../norm.md); if one factor space is zero, the map and the relevant assertion are trivial.

Bilinearity gives the exact expansion

$$
f(a+h,b+k)-f(a,b)=f(h,b)+f(a,k)+f(h,k).
$$

The proposed [derivative](../../../../../../derivative.md) $L(h,k)=f(h,b)+f(a,k)$ is linear and bounded, with $\|L(h,k)\|_3\le C(\|b\|_2\|h\|_1+\|a\|_1\|k\|_2)$. Set $\rho=(\|h\|_1^2+\|k\|_2^2)^{1/2}$. Its remainder obeys

$$
\frac{\|f(h,k)\|_3}{\rho}\le C\frac{\|h\|_1\|k\|_2}{\rho}\le\frac C2\rho\longrightarrow0.
$$

Thus the [derivative of a continuous bilinear map](../../../../../../derivative-of-a-continuous-bilinear-map.md) is the [Fréchet derivative](../../../../../../frechet-derivative.md)

$$
\boxed{Df(a,b)(h,k)=f(h,b)+f(a,k).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10E](../../10e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
