<h1 id="12f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The zeros of $\cos(\pi/x)$ occur at

$$
x_k=\frac{2}{2k+1},\qquad k\in\mathbb Z.
$$

Let $g(x)=\cos(\pi/x)$. At these nonzero points,

$$
g(x_k)=0,\qquad
 g'(x_k)=\frac\pi{x_k^2}\sin\frac\pi{x_k}
=\frac{\pi(-1)^k}{x_k^2}\ne0.
$$

The definition of the [derivative](../../../../../../derivative.md) gives $g(x_k+h)=g'(x_k)h+o(|h|)$, hence

$$
|g(x_k+h)|=\frac\pi{x_k^2}|h|+o(|h|).
$$

The [sign function](../../../../../../sign-function.md) is constant sufficiently near the nonzero point $x_k$, and $(x_k+h)^2=x_k^2+O(h)$. As $f(x_k)=0$, multiplication yields

$$
f(x_k+h)=\pi\operatorname{sign}(x_k)|h|+o(|h|).
$$

Its right and left [one-sided derivatives](../../../../../../one-sided-derivative.md) are therefore $\pi\operatorname{sign}(x_k)$ and $-\pi\operatorname{sign}(x_k)$ respectively. They differ, so $f$ is not differentiable at any $x_k$. In particular, $x_k\to0$ as $k\to+\infty$, proving

$$
\boxed{\text{Every neighbourhood of }0\text{ contains points where }f'\text{ does not exist}.}
$$

The [absolute value at a simple zero](../../../../../../absolute-value-at-a-simple-zero.md) mechanism creates unequal [one-sided derivatives](../../../../../../one-sided-derivative.md). It also shows why the existence of $f'(0)$ alone does not imply [higher-order differentiability at a point](../../../../../../higher-order-differentiability-at-a-point.md) of order two.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
