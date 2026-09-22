# Rational interpolation linearization

↑ **Parent:** [Interpolation](interpolation-split.md)

For [rational interpolation](rational-interpolation.md) with $\deg q\leq m$ and a monic denominator $r(x)=x^\ell-\sum_{j=0}^{\ell-1}b_jx^j$, multiplying through gives the [linear system](system-of-linear-equations.md)

$$
\sum_{j=0}^{m}a_jx_i^j+f_i\sum_{j=0}^{\ell-1}b_jx_i^j=f_ix_i^\ell.
$$

These equations are equivalent to the fraction conditions only when all $r(x_i)$ are nonzero. If $f_i=x_i^{m+1}$ and $m+\ell=n$, the coefficient [matrix](matrix.md) is the [Vandermonde matrix](vandermonde-matrix.md) with rows $(1,x_i,\ldots,x_i^n)$, so distinct [interpolation nodes](interpolation-node.md) give a unique coefficient solution. More constructively, divide $W(x)=\prod_{i=0}^n(x-x_i)$ by $x^{m+1}$ as $W=x^{m+1}R+S$, $\deg S\leq m$. Then $r=R$, $q=-S$, since $x^{m+1}r-q$ is the unique monic degree-$n+1$ [polynomial](polynomial-split.md) vanishing at all the [interpolation nodes](interpolation-node.md). The quotient may vanish at a node, so unique solvability of this [linear system](system-of-linear-equations.md) does not prove existence of a [rational interpolant](rational-interpolant.md).

## ↑ Ancestors (6)

1. [Interpolation](interpolation-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2023/2/c/solution.md)
- [Rational interpolation](rational-interpolation.md)
