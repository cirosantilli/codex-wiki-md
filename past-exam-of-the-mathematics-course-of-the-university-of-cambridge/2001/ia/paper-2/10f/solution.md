<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

For a [uniform random point in a disk](../../../../../uniform-random-point-in-a-disk.md), the event $R<x$ occupies a [disk](../../../../../disk-mathematics.md) of area $\pi x^2$ when $0<x<1$. Thus

$$
\boxed{F_R(x)=\begin{cases}0,&x\le0,\\x^2,&0<x<1,\\1,&x\ge1.\end{cases}}
$$

The radial [probability density function](../../../../../probability-density-function.md) is $f_R(r)=2r$ on $(0,1)$. Integrating gives

$$
\boxed{\mathbb ER=\int_0^1 2r^2\,dr=\frac23,\qquad
\mathbb ER^2=\frac12,\qquad\operatorname{Var}R=\frac1{18}.}
$$

Choose the polar angle $\Theta\in[0,2\pi)$. The Cartesian density is $1/\pi$ in the [disk](../../../../../disk-mathematics.md), and the [polar coordinates](../../../../../polar-coordinates.md) [Jacobian determinant](../../../../../jacobian-determinant.md) is $r$. Hence

$$
f_{R,\Theta}(r,\theta)=\frac r\pi=(2r)\frac1{2\pi}\quad(0<r<1,\ 0\le\theta<2\pi).
$$

The product support and product density prove that **$R$ and $\Theta$ are [independent](../../../../../independent-random-variables.md)**, with uniform angle.

Reflection symmetry gives $\mathbb EX=\mathbb EY=0$ and $\mathbb E(XY)=0$, so **$\operatorname{Cov}(X,Y)=0$**. They are nevertheless not [independent](../../../../../independent-random-variables.md). The events $X>3/4$ and $Y>3/4$ each have positive [probability](../../../../../probability.md), but their intersection is empty inside the [disk](../../../../../disk-mathematics.md), because it would require $X^2+Y^2>18/16>1$. [Independence](../../../../../independent-random-variables.md) would give a positive product [probability](../../../../../probability.md) for that intersection.

Except at the probability-zero center, $X/R=\cos\Theta$ and $Y/R=\sin\Theta$. Therefore

$$
\boxed{\mathbb E\frac XR+i\mathbb E\frac YR
=\mathbb E e^{i\Theta}=\frac1{2\pi}\int_0^{2\pi}e^{i\theta}\,d\theta=0,
\qquad\xi=\Theta\pmod{2\pi}.}
$$

An arbitrary definition at the center does not change these [expected values](../../../../../expected-value.md). This example distinguishes uncorrelated Cartesian coordinates from [independent](../../../../../independent-random-variables.md) [polar coordinates](../../../../../polar-coordinates.md).

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
