# Newton polynomial

↑ **Parent:** [Divided difference](divided-difference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Newton_polynomial)

The [Newton polynomial](newton-polynomial.md) expresses the [interpolation polynomial](interpolation-polynomial.md) in products that successively vanish at all previously used [interpolation nodes](interpolation-node.md). With $y_i=f(x_i)$, the coefficients are [divided differences](divided-difference.md):

$$
p_n(x)=f(x_0)+\sum_{k=1}^nf[x_0,\ldots,x_k]
\prod_{i=0}^{k-1}(x-x_i).
$$

A triangular [divided difference](divided-difference.md) table computes all its coefficients using exactly $n(n+1)/2$ divisions. The [Newton polynomial](newton-polynomial.md) and the [Lagrange polynomial](lagrange-polynomial.md) have the same [polynomial degree](degree-of-a-polynomial.md) bound and the same nodal values, hence are equal by uniqueness of [polynomial interpolation](polynomial-interpolation.md).

For $f(0)=1$, $f(1)=2$, $f(2)=5$, the complete [divided difference](divided-difference.md) table is

$$
\begin{array}{c|r|r|r}
x_i&f[x_i]&f[x_i,x_{i+1}]&f[x_i,x_{i+1},x_{i+2}]\\\hline
0&1&1&1\\
1&2&3&\\
2&5&&
\end{array}
$$

The first [divided differences](divided-difference.md) are $1$ and $3$, and their [divided difference](divided-difference.md) is $(3-1)/(2-0)=1$. Reading the top entries gives

$$
p_2(x)=1+1(x-0)+1(x-0)(x-1)=1+x+x(x-1)=x^2+1.
$$

The initial term fits $(0,1)$; adding $x$ also fits $(1,2)$; adding $x(x-1)$ fits $(2,5)$ while leaving the first two data values unchanged. This is the practical beauty of the [Newton polynomial](newton-polynomial.md): each new correction respects all previous interpolation constraints.

If a new distinct [interpolation node](interpolation-node.md) $x_{n+1}$ with value $y_{n+1}$ arrives, append one term:

$$
p_{n+1}(x)=p_n(x)+c\prod_{i=0}^n(x-x_i),\qquad
c=\frac{y_{n+1}-p_n(x_{n+1})}{\prod_{i=0}^n(x_{n+1}-x_i)}.
$$

For example, appending $(3,11)$ to the three-point data gives $c=(11-10)/(3\cdot2\cdot1)=1/6$, hence $p_3(x)=x^2+1+x(x-1)(x-2)/6$. Changing the order of the [interpolation nodes](interpolation-node.md) changes the [Newton polynomial](newton-polynomial.md) coefficients and products, but not the final [interpolation polynomial](interpolation-polynomial.md) in exact arithmetic.

The products also permit nested evaluation analogous to [Horner's method](horner-s-method.md). If $a_k=f[x_0,\ldots,x_k]$, start with $b_n=a_n$ and work backwards by $b_k=a_k+(x-x_k)b_{k+1}$; the answer is $b_0$. The three-point example becomes $1+x[1+(x-1)]$, needing two multiplications for each evaluation. This organization is useful when adding observations incrementally or evaluating a stored [Newton polynomial](newton-polynomial.md) many times; the [Runge phenomenon](runge-s-phenomenon.md) still depends on the [interpolation nodes](interpolation-node.md) rather than on which representation is used.

To justify the update formula, its added [product](product-of-numbers.md) vanishes at every previous [interpolation node](interpolation-node.md). Choosing $c$ by the new residual forces agreement at $x_{n+1}$, so uniqueness of [polynomial interpolation](polynomial-interpolation.md) identifies the result. For $n\geq0$, $p_n$ has [polynomial degree](degree-of-a-polynomial.md) at most $n$, and the added [product](product-of-numbers.md) has [leading coefficient](leading-coefficient-of-a-polynomial.md) one. Thus the new [coefficient](coefficient.md) $c$ is exactly $f[x_0,\ldots,x_{n+1}]$. The initial state is $p_0(x)=f(x_0)$, with the [empty product](empty-product.md) interpreted as one.[NIST Digital Library of Mathematical Functions; §3.3(iv), equation 3.3.38 and the following new-point update paragraph](nist-digital-library-of-mathematical-functions/3-3-interpolation.md)

Appending $(4,57)$ to the four-point example in [divided difference table](divided-difference-table.md) leaves the [Newton polynomial](newton-polynomial.md) unchanged: $p_3(4)=57$, so the new fourth [divided difference](divided-difference.md) is zero. If the appended value is instead $58$, the new [coefficient](coefficient.md) is

$$
c=\frac{58-57}{(4+1)\cdot4\cdot(4-2)\cdot(4-3)}=\frac1{40},\qquad
p_4(x)=x^3-2x+1+\frac{(x+1)x(x-2)(x-3)}{40}.
$$

This [polynomial](polynomial-split.md) still takes values $2,1,5,22$ at the original [interpolation nodes](interpolation-node.md), and now takes value $58$ at $4$. A zero update is a valid completed step: adding another exact sample of the original [polynomial](polynomial-split.md) need not increase the [polynomial degree](degree-of-a-polynomial.md).

**Table of contents**

- [Node order in Newton interpolation](node-order-in-newton-interpolation.md)

## ↑ Ancestors (8)

1. [Divided difference](divided-difference.md)
2. [Polynomial interpolation](polynomial-interpolation.md)
3. [Interpolation](interpolation-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Divided difference](divided-difference.md)
- [Divided difference table](divided-difference-table.md)
- [Newton polynomial](newton-polynomial.md)
- [Node order in Newton interpolation](node-order-in-newton-interpolation.md)
- [Polynomial interpolation](polynomial-interpolation.md)
- [Symmetry of divided differences](symmetry-of-divided-differences.md)
