<h1 id="14d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Substitute $y(x)=\sum_{j\geq0}c_jx^j$ into the [Legendre differential equation](../../../../../../legendre-differential-equation.md). Matching the coefficient of $x^j$ gives

$$
\boxed{c_{j+2}=\frac{j(j+1)-n(n+1)}{(j+2)(j+1)}c_j.}
$$

Choose the parity of $n$: start with nonzero $c_0$ for even $n$, or nonzero $c_1$ for odd $n$, and set the other parity to zero. The numerator is nonzero for every preceding index of that parity below $n$, so $c_n\ne0$, but at $j=n$ it vanishes. All higher coefficients are zero. This constructs a nonzero polynomial solution of degree exactly $n$.

Its value at $x=1$ cannot be zero. If it had a zero there of multiplicity $k\geq1$, write $y=(x-1)^kR$ with $R(1)\ne0$. The lowest-order term of $(1-x^2)y''-2xy'$ would be $-2k^2R(1)(x-1)^{k-1}$, whereas $n(n+1)y$ starts at order $k$. The differential equation could not hold. Hence the polynomial can be scaled to satisfy $P_n(1)=1$.

The resulting [Legendre polynomials](../../../../../../legendre-polynomial.md) begin

$$
\boxed{P_0(x)=1,\qquad P_1(x)=x,\qquad P_2(x)=\tfrac12(3x^2-1).}
$$

Each satisfies both the differential equation and the specified normalization.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [14D](../../14d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
