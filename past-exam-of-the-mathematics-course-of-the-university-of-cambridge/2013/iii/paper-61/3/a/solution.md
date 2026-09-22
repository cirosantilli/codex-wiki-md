<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the strictly increasing local [spline knots](../../../../../../spline-knot.md) as $u_j=t_{i+j}$, $0\le j\le k$. The explicit formula for a [divided difference](../../../../../../divided-difference.md) gives

$$
M_i(t)=k\sum_{j=0}^k
\frac{(u_j-t)_+^{k-1}}
{\prod_{\ell\ne j}(u_j-u_\ell)}.
$$

Each summand is a [truncated power function](../../../../../../truncated-power-function.md) of $t$: it is a [polynomial](../../../../../../polynomial-split.md) on either side of its knot $u_j$, and for $k\ge2$ is globally $C^{k-2}$. Hence $M_i$ is a [piecewise polynomial function](../../../../../../piecewise-polynomial-function.md) of degree at most $k-1$, with these [spline knots](../../../../../../spline-knot.md) and at least this global smoothness.

For $t\ge u_k$, all summands vanish. For $t<u_0$, all knot values agree with those of the ordinary [polynomial](../../../../../../polynomial-split.md) $(s-t)^{k-1}$ in the divided-difference variable $s$. Its order-$k$ [divided difference](../../../../../../divided-difference.md) is zero, because its degree is less than $k$. Thus $M_i$ also vanishes to the left of $u_0$.

The closed support is exactly the indicated interval, rather than merely contained in it. For $u_0<t<u_1$, subtracting the omitted $j=0$ term from the zero divided difference of $(s-t)^{k-1}$ gives

$$
M_i(t)=\frac{k(t-u_0)^{k-1}}{\prod_{\ell=1}^k(u_\ell-u_0)}>0.
$$

For $u_{k-1}<t<u_k$, only the last truncated-power term survives, giving

$$
M_i(t)=\frac{k(u_k-t)^{k-1}}{\prod_{\ell=0}^{k-1}(u_k-u_\ell)}>0.
$$

There are therefore nonzero values arbitrarily close to either endpoint, proving

$$
\boxed{\operatorname{supp}M_i=[t_i,t_{i+k}],\qquad M_i\in C^{k-2}}.
$$

At each simple knot, the $(k-1)$st derivative has a nonzero jump from exactly one truncated-power summand, so this is also the exact global smoothness. For order $k=1$, the function is instead the normalized interval indicator; there is no assertion of classical continuity, and the notation $C^{k-2}$ is only the customary formal spline smoothness notation. This distinction is part of [simple-knot B-spline regularity](../../../../../../simple-knot-b-spline-regularity.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
