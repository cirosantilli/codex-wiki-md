<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

The [Fréchet derivative](../../../../../frechet-derivative.md) at $p=(x_0,y_0)$ is a [linear map](../../../../../linear-map.md) $L:\mathbb R^2\to\mathbb R$ for which

$$
 f(p+h)=f(p)+Lh+o(\|h\|)\quad(h\to0).
$$

This is [differentiability](../../../../../differentiability.md); if it holds, $L(h_1,h_2)=D_1f(p)h_1+D_2f(p)h_2$.

To prove the sufficient condition, take a rectangle about $p$ contained in the open domain. Split the increment along its coordinate directions:

$$
 f(x_0+h,y_0+k)-f(p)
 =[f(x_0+h,y_0+k)-f(x_0,y_0+k)]
 +[f(x_0,y_0+k)-f(p)].
$$

The one-variable [mean value theorem](../../../../../mean-value-theorem.md), applicable because the restrictions are differentiable, represents these two terms as

$$
 hD_1f(x_0+\theta h,y_0+k)+kD_2f(x_0,y_0+\phi k),\qquad0<\theta,\phi<1.
$$

The zero-increment cases are interpreted directly. Subtract $D_1f(p)h+D_2f(p)k$. By [continuity](../../../../../continuous-function.md) of both [partial derivatives](../../../../../partial-derivative.md) at $p$, the remainder is at most $\varepsilon(|h|+|k|)\leq\sqrt2\varepsilon\sqrt{h^2+k^2}$ once the increment is small. This is the required little-oh remainder and proves [differentiability](../../../../../differentiability.md).

The converse is false. Set $f(x,y)=x^2\sin(1/x)$ for $x\ne0$, and $f(0,y)=0$. At each point with $x=0$, its [Fréchet derivative](../../../../../frechet-derivative.md) is zero, since the function increment has magnitude at most $h^2=o(\sqrt{h^2+k^2})$. It is smooth away from this line. But

$$
 D_1f(x,y)=2x\sin(1/x)-\cos(1/x)\quad(x\ne0),\qquad D_1f(0,y)=0,
$$

is not continuous there. Thus a function can be differentiable everywhere while its [partial derivatives](../../../../../partial-derivative.md) are discontinuous.

For $h$, every point with $x\ne0$ is a smooth point. At the origin, $|h(x,y)|\leq|xy|\leq(x^2+y^2)/2$, so $h$ is differentiable with zero derivative. At $(0,y_0)$ with $y_0\ne0$, the putative first [partial derivative](../../../../../partial-derivative.md) would require the limit $y_0\sin(1/x)$, which does not exist. Consequently the exact set of differentiability is

$$
 \boxed{\{(x,y):x\ne0\}\ \cup\ \{(0,0)\}.}
$$

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
