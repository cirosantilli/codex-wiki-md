<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

Fix $(x,y)\in U$ and a sufficiently small rectangle inside $U$. Its rectangular increment

$$
\Delta=f(x+h,y+k)-f(x+h,y)-f(x,y+k)+f(x,y)
$$

can be evaluated twice using the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md), giving

$$
\Delta=\int_x^{x+h}\int_y^{y+k}D_2D_1f(s,t)\,dt\,ds
=\int_y^{y+k}\int_x^{x+h}D_1D_2f(s,t)\,ds\,dt.
$$

Divide by $hk$ and let $h,k\to0$. Continuity of the [mixed partial derivatives](../../../../../mixed-partial-derivative.md) makes the two limits $D_2D_1f(x,y)$ and $D_1D_2f(x,y)$. **They are equal everywhere on $U$.**

Repeated interchange of adjacent [partial derivatives](../../../../../partial-derivative.md) reduces every order-$m$ [derivative](../../../../../derivative.md) of a smooth function to $D_1^jD_2^{m-j}f$, $0\leq j\leq m$. Hence there are at most $m+1$ distinct functions. This maximum is attained by $f(x,y)=e^{x+2y}$, whose listed [partial derivatives](../../../../../partial-derivative.md) are the distinct functions $2^{m-j}e^{x+2y}$. The answer is **$m+1$**, rather than the $2^m$ possible written orders.

For the supplied $f$, $f(t,t)=1/2$ for $t\ne0$, whereas $f(0,0)=0$. It is not even continuous at the origin, so **$f$ is neither differentiable nor infinitely differentiable there**.

For $g$, $|g(x,y)|\leq|xy|\leq(x^2+y^2)/2$. Thus $g(x,y)=o(\sqrt{x^2+y^2})$, proving [Fréchet differentiability](../../../../../frechet-differentiability.md) at the origin with [derivative](../../../../../derivative.md) zero. However,

$$
D_1g(0,y)=-y,\qquad D_2g(x,0)=x,
$$

including zero at the origin. Therefore $D_2D_1g(0,0)=-1$ and $D_1D_2g(0,0)=1$. **$g$ is differentiable but not infinitely differentiable at the origin**: it cannot have continuous second [partial derivatives](../../../../../partial-derivative.md) near that point.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
