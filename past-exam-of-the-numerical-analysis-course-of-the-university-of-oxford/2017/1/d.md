<h1 id="1/d">d</h1>

↑ **Parent:** [1](../1.md)

Read the differential order $dx\,dy$ literally: take [quadrature nodes](../../../quadrature-node.md) $X=(c,(c+d)/2,d)$ in $x$ and $Y=(a,(a+b)/2,b)$ in $y$. Applying [Simpson's rule](../../../simpson-s-rule.md) first in $x$ and then in $y$ multiplies the one-dimensional [quadrature weights](../../../quadrature-weight.md). With $s=(1,4,1)$, this [tensor-product quadrature](../../../tensor-product-quadrature.md) is

$$
Q(g)=\frac{(b-a)(d-c)}{36}\sum_{i=0}^2\sum_{j=0}^2s_i s_jg(X_i,Y_j).
$$

Equivalently, the nine sampled [function](../../../function-split.md) values have the [quadrature weight](../../../quadrature-weight.md) array

$$
\frac{(b-a)(d-c)}{36}
\begin{pmatrix}1&4&1\\4&16&4\\1&4&1\end{pmatrix},
$$

with rows indexed by the $x$ [quadrature nodes](../../../quadrature-node.md) and columns by the $y$ [quadrature nodes](../../../quadrature-node.md). The [quadrature weights](../../../quadrature-weight.md) sum to the [rectangle](../../../rectangle.md)'s area. If the intended coordinate assignment is instead $x\in[a,b]$, $y\in[c,d]$, exchange $X$ and $Y$ in the formula. Both conventions give the same calculation on the unit square used below.

For the [separable integrand](../../../separable-integrand.md), [tensor-product quadrature](../../../tensor-product-quadrature.md) factors into two one-dimensional applications of [Simpson's rule](../../../simpson-s-rule.md):

$$
Q_x\bigl(x(1-x)\bigr)=\frac16\left[0+4\cdot\frac14+0\right]=\frac16,
\qquad
Q_y(y^q)=\frac{1+4\,2^{-q}}6,
$$

so

$$
\boxed{Q(g)=\frac{1+2^{2-q}}{36}.}
$$

The exact [double integral](../../../double-integral.md), evaluated by [Fubini's theorem](../../../fubini-s-theorem.md) and the [power rule for integration](../../../power-rule-for-integration.md), is

$$
I(g)=\left(\int_0^1x(1-x)\,dx\right)\left(\int_0^1y^q\,dy\right)
=\frac{1}{6(q+1)}.
$$

The $x$ factor is always integrated exactly. All [quadrature error](../../../quadrature-error.md) therefore comes from applying [Simpson's rule](../../../simpson-s-rule.md) to the $y$ factor.

**Table of contents**

- [i](d/i.md)
  - [Solution](d/i/solution.md)
- [ii](d/ii.md)
  - [Solution](d/ii/solution.md)
- [iii](d/iii.md)
  - [Solution](d/iii/solution.md)

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2017](../../2017-split.md)
3. [Past exam of the numerical analysis course of the University of Oxford](../../split.md)
4. [Numerical analysis course of the University of Oxford](../../../numerical-analysis-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
