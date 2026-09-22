<h1 id="22a/solution">Solution</h1>

↑ **Parent:** [22A](../22a.md)

Let $L(f)=\mathcal T[f]-f'(1/3)$. Direct substitution shows $L(1)=L(x)=L(x^2)=0$, so the functional annihilates all quadratic polynomials. Taylor's integral-remainder formula is

$$
f(x)=f(0)+xf'(0)+\frac{x^2}{2}f''(0)
+\int_0^1\frac{(x-t)_+^2}{2}f'''(t)\,dt.
$$

Applying $L$ and interchanging the finite evaluations and derivative with the continuous integral gives the [Peano kernel](../../../../../peano-kernel.md) representation $L(f)=\int_0^1K(t)f'''(t)dt$, where

$$
K(t)=\frac23(1/2-t)_+^2+\frac16(1-t)^2-(1/3-t)_+
=\begin{cases}
5t^2/6,&0\le t\le1/3,\\
5t^2/6-t+1/3,&1/3\le t\le1/2,\\
(1-t)^2/6,&1/2\le t\le1.
\end{cases}
$$

All three expressions are nonnegative; the middle quadratic has positive leading coefficient and discriminant $-1/9$. Therefore the best possible norm bound has constant $\int_0^1K(t)dt$. Evaluate that integral particularly simply by using $f(x)=x^3/6$, for which $f'''=1$:

$$
\int_0^1K(t)dt=L(x^3/6)=\frac1{12}-\frac1{18}=\frac1{36}.
$$

It follows that

$$
\boxed{|\mathcal T[f]-f'(1/3)|\le\frac1{36}\|f'''\|_\infty,\qquad c_{\min}=\frac1{36}.}
$$

The same cubic attains equality, so the constant is sharp, not merely sufficient. This is the [sharp Peano bound for an interior three-point first derivative](../../../../../sharp-peano-bound-for-an-interior-three-point-first-derivative.md).

## ↑ Ancestors (10)

1. [22A](../22a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
