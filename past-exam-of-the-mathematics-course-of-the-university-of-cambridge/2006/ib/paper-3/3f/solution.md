<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The function is [Fréchet differentiable](../../../../../frechet-differentiability.md) at $(a,b)$ when there is a [linear map](../../../../../linear-map.md) $L:\mathbb R^2\to\mathbb R$ such that

$$
f(a+h,b+k)=f(a,b)+L(h,k)+r(h,k),\qquad
\lim_{(h,k)\to(0,0)}\frac{|r(h,k)|}{\sqrt{h^2+k^2}}=0.
$$

If it exists, $L(h,k)=f_x(a,b)h+f_y(a,b)k$, as is seen by taking increments along each coordinate axis.

To prove [differentiability from continuous partial derivatives](../../../../../differentiability-from-continuous-partial-derivatives.md), take a small rectangle in the given neighbourhood and split the increment along its sides. The one-variable [mean value theorem](../../../../../mean-value-theorem.md) gives

$$
\begin{aligned}
f(a+h,b+k)-f(a,b)
&=f(a+h,b+k)-f(a,b+k)+f(a,b+k)-f(a,b)\\
&=h f_x(a+\theta h,b+k)+k f_y(a,b+\eta k),
\end{aligned}
$$

for some $0<\theta,\eta<1$ when the corresponding increment is nonzero. If an increment is zero, its term is simply omitted. The required one-variable continuity follows from existence of the corresponding [partial derivative](../../../../../partial-derivative.md) on the segment. Subtracting $L(h,k)$ gives a remainder whose absolute value, by continuity of both [partial derivatives](../../../../../partial-derivative.md) at $(a,b)$, is at most

$$
\epsilon(|h|+|k|)\le\sqrt2\epsilon\sqrt{h^2+k^2}
$$

for sufficiently small increments. Since $\epsilon$ is arbitrary, the normalized remainder tends to zero. Thus **the function is differentiable at $(a,b)$**, with the displayed derivative.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
