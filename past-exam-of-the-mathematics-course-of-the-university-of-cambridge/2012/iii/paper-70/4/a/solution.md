<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual strictly increasing [spline knot sequence](../../../../../../spline-knot-sequence.md), and initially assume $k\ge2$. The explicit formula for the order-$k$ [divided difference](../../../../../../divided-difference.md) gives

$$
M_i(t)=k\sum_{j=i}^{i+k}\frac{(t_j-t)_+^{k-1}}{\prod_{\substack{\ell=i\\\ell\ne j}}^{i+k}(t_j-t_\ell)}.
$$

Each summand is a [truncated power function](../../../../../../truncated-power-function.md) in $t$, with its junction at $t_j$. It is a [piecewise polynomial function](../../../../../../piecewise-polynomial-function.md) of degree at most $k-1$ and has $k-2$ [continuous](../../../../../../continuous-function.md) [derivatives](../../../../../../derivative.md). Finite summation preserves these properties.

For $t\ge t_{i+k}$ all summands vanish. For $t\le t_i$, all [spline knot](../../../../../../spline-knot.md) data come from the [polynomial](../../../../../../polynomial-split.md) $u\mapsto(u-t)^{k-1}$. An order-$k$ [divided difference](../../../../../../divided-difference.md) annihilates a [polynomial](../../../../../../polynomial-split.md) of smaller degree, so $M_i(t)=0$ there too. Thus the [support](../../../../../../support.md) is contained in $[t_i,t_{i+k}]$.

On the last open [spline knot](../../../../../../spline-knot.md) interval only the $j=i+k$ term survives; it is a nonzero multiple of $(t_{i+k}-t)^{k-1}$. On the first open [spline knot](../../../../../../spline-knot.md) interval, compare the truncated [spline knot](../../../../../../spline-knot.md) data with the untruncated [polynomial](../../../../../../polynomial-split.md) data: only the $j=i$ value differs. Since the untruncated [divided difference](../../../../../../divided-difference.md) is zero, the result is a nonzero multiple of $(t_i-t)^{k-1}$. Consequently both outer pieces are nonzero, giving exact closed [support](../../../../../../support.md). The [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md) used below also proves positivity throughout the open [support](../../../../../../support.md). Therefore

$$
\boxed{M_i\in C^{k-2}(\mathbb R),\qquad\operatorname{supp}M_i=[t_i,t_{i+k}],\qquad\deg\text{ each piece}\le k-1.}
$$

This is [simple-knot B-spline regularity](../../../../../../simple-knot-b-spline-regularity.md). For $k=1$ the [B-splines](../../../../../../b-spline.md) are interval indicators; they are piecewise constant and need not be [continuous](../../../../../../continuous-function.md). The notation $C^{k-2}$ should then be read as no [continuity](../../../../../../continuous-function.md) requirement, not as a classical negative-order differentiability space.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
