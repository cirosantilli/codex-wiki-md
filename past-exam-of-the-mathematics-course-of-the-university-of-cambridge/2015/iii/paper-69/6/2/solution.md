<h1 id="6/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the standard partition normalization of [B-splines](../../../../../../b-spline.md), not rescaling each spline to have supremum exactly one. Let $h_i=t_{i+k}-t_i>0$. Then $M_i=kN_i/h_i$. In the ordinary real [inner product](../../../../../../inner-product.md), the [mixed-normalization spline Gram matrix](../../../../../../mixed-normalization-spline-gram-matrix.md) is $G=D^{-1}H$, where $D=\operatorname{diag}(h_i/k)$ and $H_{ij}=(N_i,N_j)$. Since the $N_i$ form a basis, $H$ is positive definite; $D$ is invertible, so $G$ is invertible. The undeclared upper index $h$ in the printed matrix should be $n$.

We need the standard positivity and normalization properties with their justification. The [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md) is

$$
N_{i,k}(t)=\frac{t-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(t)+\frac{t_{i+k}-t}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(t),
$$

with zero-width terms interpreted as zero. It starts from nonnegative interval indicators. On each lower-order spline's support, its recurrence coefficients are nonnegative, so induction gives $N_i\geq0$. Extend the finite knots outside their endpoints to a full knot sequence. In the full sum, coefficients of each lower-order spline add to one, so the recurrence preserves [partition of unity](../../../../../../partition-of-unity.md). Our finite collection is a subset of nonnegative [B-splines](../../../../../../b-spline.md); therefore $\sum_{i=1}^nN_i(t)\leq1$ everywhere. The [Marsden identity](../../../../../../marsden-identity.md) gives equality on the basic knot interval.

The divided-difference definition also gives support in $[t_i,t_{i+k}]$: below the left endpoint the knot-data function is a [polynomial](../../../../../../polynomial-split.md) of degree $k-1$, whose order-$k$ [divided difference](../../../../../../divided-difference.md) vanishes; above the right endpoint the knot data vanish. Choose $a<t_i$ and $b>t_{i+k}$. Integrating in $t$ and then taking the [divided difference](../../../../../../divided-difference.md) in its knot variable gives

$$
\int M_i(t)\,dt
=k[t_i,\ldots,t_{i+k}]\left(\frac{(\cdot-a)^k}{k}\right)=1,
$$

because an order-$k$ [divided difference](../../../../../../divided-difference.md) of a monic degree-$k$ [polynomial](../../../../../../polynomial-split.md) is one. The support lies inside $[0,1]$, so $\int_0^1M_i=1$.

[Orthogonality](../../../../../../orthogonal-vectors.md) of $f-s^*$ to the spline space gives $Ga=r$, with $r_i=(M_i,f)$. Since $M_i\geq0$ and has unit integral, $|r_i|\leq\|f\|_\infty$. The induced matrix maximum norm is the absolute row-sum norm, so

$$
\|a\|_{\ell^\infty}\leq\|G^{-1}\|_{\ell^\infty}\|f\|_\infty,
\qquad
|s^*(t)|\leq\|a\|_{\ell^\infty}\sum_iN_i(t)\leq\|a\|_{\ell^\infty}.
$$

Taking the supremum over nonzero $f$ proves **the [maximum-norm bound for spline projection](../../../../../../maximum-norm-bound-for-spline-projection.md)**:

$$
\boxed{\|P_{\mathcal S}\|_\infty\leq\|G^{-1}\|_{\ell^\infty}.}
$$

The range is $\mathcal S$, so the printed phrase “onto $C[0,1]$” must mean into $C[0,1]$, and onto $\mathcal S$. Continuity of the range requires continuous [B-splines](../../../../../../b-spline.md), for example $k\geq2$ and internal multiplicities at most $k-1$. For order-one or discontinuous [B-splines](../../../../../../b-spline.md), the same bound is valid with codomain $L^\infty[0,1]$ rather than $C[0,1]$.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [6](../../6.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
