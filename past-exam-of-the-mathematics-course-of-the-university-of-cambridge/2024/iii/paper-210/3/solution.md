<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [cubic spline](../../../../../cubic-spline.md) with knots $x_1<\cdots<x_n$ is twice continuously differentiable and restricts to a polynomial of degree at most three between consecutive knots. It is a [natural cubic spline](../../../../../natural-cubic-spline.md) when it is linear outside $[x_1,x_n]$, equivalently when its second derivative vanishes at the two outer knots and on the exterior intervals.

Let $s$ be the natural cubic spline interpolating prescribed values and let $\widetilde g=s+h$ be any other interpolant in $S_2[a,b]$. Then $h(x_i)=0$. Piecewise [integration by parts](../../../../../integration-by-parts.md), using that $s''''=0$ between knots, $s''$ is continuous, $s''=0$ on the exterior intervals, and every jump of $s'''$ is multiplied by $h(x_i)=0$, gives

$$
\int_a^bs''(x)h''(x)\,dx=0.
$$

Consequently

$$
R(\widetilde g)=R(s)+R(h)\geq R(s).
$$

Equality forces $h''=0$ almost everywhere. Then $h$ is affine and its zeros at at least two distinct knots force $h=0$, proving uniqueness.

For the penalized problem, fix a vector $u=(u_1,\ldots,u_n)^T$ of fitted values. The preceding variational result says that its natural spline interpolant has the least roughness among all functions taking those values, and by assumption that roughness is $u^TKu$. The infinite-dimensional problem therefore reduces to

$$
\min_{u\in\mathbb R^n}
\{\lVert Y-u\rVert_2^2+\lambda u^TKu\}.
$$

Because $K$ is positive semidefinite, $I+\lambda K$ is positive definite. The unique fitted-value vector is

$$
\widehat u=A_\lambda Y,
\qquad
A_\lambda=(I+\lambda K)^{-1},
$$

and $\widehat g_\lambda$ is its unique natural cubic spline interpolant.

For [Leave-one-out cross-validation](../../../../../leave-one-out-cross-validation.md), let $\widehat g_{-i,\lambda}$ minimize

$$
\sum_{j\ne i}(Y_j-\widetilde g(x_j))^2+\lambda R(\widetilde g)
$$

and define

$$
\operatorname{CV}(\lambda)=\frac1n\sum_{i=1}^n
(Y_i-\widehat g_{-i,\lambda}(x_i))^2.
$$

If $u^{(-i)}_j=\widehat g_{-i,\lambda}(x_j)$, its normal equations say

$$
u^{(-i)}_j+\lambda(Ku^{(-i)})_j=Y_j\quad(j\ne i),
\qquad
(Ku^{(-i)})_i=0.
$$

Thus $u^{(-i)}=A_\lambda\widetilde Y^{(i)}$, where

$$
\widetilde Y^{(i)}_j=
\begin{cases}
Y_j,&j\ne i,\\
u^{(-i)}_i,&j=i.
\end{cases}
$$

Taking the $i$th coordinate and writing $\widehat u=A_\lambda Y$ gives

$$
u^{(-i)}_i
=\frac{\widehat u_i-(A_\lambda)_{ii}Y_i}
{1-(A_\lambda)_{ii}},
\qquad
Y_i-u^{(-i)}_i
=\frac{Y_i-\widehat u_i}{1-(A_\lambda)_{ii}}.
$$

Therefore one spline fit and the diagonal of its [smoothing matrix](../../../../../smoothing-matrix.md) give

$$
\boxed{\operatorname{CV}(\lambda)
=\frac1n\sum_{i=1}^n
\left(\frac{Y_i-\widehat u_i}
{1-(A_\lambda)_{ii}}\right)^2.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
