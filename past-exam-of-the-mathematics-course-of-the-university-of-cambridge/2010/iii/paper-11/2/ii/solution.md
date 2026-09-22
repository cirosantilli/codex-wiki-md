<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For this [Cartesian product](../../../../../../cartesian-product.md), the requested $U^2$ norm is the [box norm](../../../../../../box-norm.md), with complex conjugates:

$$
\boxed{\|f\|_{U^2}^4=\mathbb E_{x,x'\in X}\mathbb E_{y,y'\in Y}
f(x,y)\overline{f(x',y)}\overline{f(x,y')}f(x',y').}
$$

Equivalently it is $\mathbb E_{y,y'}|K(y,y')|^2$, where $K(y,y')=\mathbb E_xf(x,y)\overline{f(x,y')}$. This makes its nonnegativity explicit.

Apply the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) first in $x$:

$$
|\mathbb E_{x,y}f(x,y)u(x)v(y)|^2
\le\|u\|_2^2\,\mathbb E_{y,y'}v(y)\overline{v(y')}K(y,y').
$$

The right-hand expectation is nonnegative, since it came from $\mathbb E_x|\mathbb E_yf(x,y)v(y)|^2$. A second application in $(y,y')$ gives

$$
|\mathbb E_{x,y}fuv|^4
\le\|u\|_2^4\,
\mathbb E_{y,y'}|v(y)\overline{v(y')}|^2
\mathbb E_{y,y'}|K(y,y')|^2
=\|u\|_2^4\|v\|_2^4\|f\|_{U^2}^4.
$$

Taking fourth roots proves the [bilinear correlation bound for the box norm](../../../../../../bilinear-correlation-bound-for-the-box-norm.md)

$$
\boxed{|\mathbb E_{x,y}f(x,y)u(x)v(y)|\le\|f\|_{U^2}\|u\|_2\|v\|_2.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
