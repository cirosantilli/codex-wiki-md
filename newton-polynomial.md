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

## ↑ Ancestors (8)

1. [Divided difference](divided-difference.md)
2. [Polynomial interpolation](polynomial-interpolation.md)
3. [Interpolation](interpolation.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Divided difference](divided-difference.md)
- [Newton polynomial](newton-polynomial.md)
- [Polynomial interpolation](polynomial-interpolation.md)
