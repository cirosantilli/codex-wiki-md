<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the standard knot-domain convention in which the [spline](../../../../../spline-mathematics.md) space contains every [polynomial](../../../../../polynomial-split.md) of degree at most $k-1$ on $[a,b]$, with completed or clamped endpoint knots. The [De Boor–Fix functional](../../../../../de-boor-fix-spline-coefficient-functional.md) extracts a local [spline](../../../../../spline-mathematics.md) [coefficient](../../../../../coefficient.md), and its [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) extension is linear on continuous local data with the stated bound. Only that bound and [spline](../../../../../spline-mathematics.md) reproduction are needed here.

For $x$ in a knot cell $[t_j,t_{j+1}]$, [support and Gram bandwidth of B-splines](../../../../../support-and-gram-bandwidth-of-b-splines.md) implies that only indices

$$
j+1-k\le i\le j
$$

can contribute, restricted also to $1\le i\le n$. Every corresponding local [support](../../../../../support.md) $[t_i,t_{i+k}]$ lies inside

$$
J_j=[t_{j+1-k},t_{j+k}].
$$

Nonnegativity and [subpartition of unity for B-splines](../../../../../subpartition-of-unity-for-b-splines.md) therefore give

$$
|Qf(x)|\le\sum_i|\lambda_i(f)|N_i(x)
\le c_k\|f\|_{C(J_j)}\sum_iN_i(x)
\le c_k\|f\|_{C(J_j)}.
$$

Taking the supremum over the cell proves the local stability estimate for [spline quasi-interpolation](../../../../../spline-quasi-interpolation.md):

$$
\boxed{\|Qf\|_{C[t_j,t_{j+1}]}\le c_k\|f\|_{C[t_{j+1-k},t_{j+k}]}.}
$$

Endpoint limits follow by continuity for $k\ge2$; the order-one version uses the usual one-sided interval convention.

Let $h=\max_i|t_{i+1}-t_i|$ and $f\in C^k[a,b]$. Choose any point $y_j$ in the stencil and form its degree-$k-1$ [Taylor polynomial](../../../../../taylor-polynomial.md) $p_j$. The [Taylor theorem](../../../../../taylor-theorem.md) remainder gives

$$
\|f-p_j\|_{C(J_j)}\le\frac{\operatorname{diam}(J_j)^k}{k!}
\|f^{(k)}\|_{C(J_j)}
\le\frac{(2k-1)^kh^k}{k!}\|f^{(k)}\|_\infty.
$$

The [polynomial](../../../../../polynomial-split.md) is itself a [spline](../../../../../spline-mathematics.md), so $Qp_j=p_j$. By linearity and the local stability estimate,

$$
\|f-Qf\|_{C[t_j,t_{j+1}]}
\le\|f-p_j\|_{C[t_j,t_{j+1}]}+\|Q(f-p_j)\|_{C[t_j,t_{j+1}]}
\le(1+c_k)\|f-p_j\|_{C(J_j)}.
$$

Taking the maximum over cells yields

$$
\boxed{\|f-Qf\|_\infty\le
\frac{(1+c_k)(2k-1)^k}{k!}h^k\|f^{(k)}\|_\infty=O(h^k).}
$$

The constant depends only on $k$ and the supplied functional bound, not on mesh ratios or the number of knots.

The endpoint convention is essential to the global assertion. The domain can be the basic knot interval, with any needed exterior data extended smoothly, or the full approximation interval can use clamped endpoint knots. If one instead takes a finite, unclamped collection on the entire outer [support](../../../../../support.md) interval $[t_1,t_{n+k}]$, every order-$k\ge2$ [basis](../../../../../basis.md) function vanishes at $t_1$, so $Q1(t_1)=0$ and uniform approximation to the constant one there is impossible. This does not affect the local estimate; it explains the usual boundary completion implicit in the global [spline](../../../../../spline-mathematics.md) approximation statement.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
