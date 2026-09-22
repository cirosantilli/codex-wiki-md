<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

[Differentiability](../../../../../differentiability.md) at $(a,b)$ means that there is a [linear map](../../../../../linear-map.md) $L:\mathbb R^2\to\mathbb R$ such that

$$
f(a+h,b+k)-f(a,b)=L(h,k)+o(\sqrt{h^2+k^2}).
$$

Necessarily $L(h,k)=f_x(a,b)h+f_y(a,b)k$ when those [partial derivatives](../../../../../partial-derivative.md) exist. Under the stated assumptions, apply the one-variable [mean value theorem](../../../../../mean-value-theorem.md) separately to the two coordinate increments:

$$
f(a+h,b+k)-f(a,b)=h f_x(a+\theta h,b+k)+k f_y(a,b+\eta k),
$$

for some intermediate $\theta,\eta\in(0,1)$, omitting a term if its increment is zero. Existence of the [partial derivatives](../../../../../partial-derivative.md) in a neighborhood supplies the differentiability along each segment required for that theorem. Their [continuity](../../../../../continuous-function.md) at $(a,b)$ makes the difference from $f_x(a,b)h+f_y(a,b)k$ bounded by $(|h|+|k|)\varepsilon(h,k)$, where $\varepsilon(h,k)\to0$. Since $|h|+|k|\le\sqrt2\sqrt{h^2+k^2}$, this is the required little-o remainder and proves [Fréchet differentiability](../../../../../frechet-differentiability.md).

For the particular function, $f(h,0)=f(0,k)=0$, so the defining difference quotients give **$f_x(0,0)=f_y(0,0)=0$**. However $f(t,t)=1/2$ for every $t\ne0$. It is not continuous at the origin, and therefore **not differentiable there**. This illustrates why existence of [partial derivatives](../../../../../partial-derivative.md) alone is insufficient.

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
