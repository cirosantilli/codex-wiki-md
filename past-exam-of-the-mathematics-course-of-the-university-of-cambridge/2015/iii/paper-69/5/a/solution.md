<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $g_t(y)=(y-t)_+^{k-1}$. Begin with distinct increasing knots so ordinary [polynomial interpolation](../../../../../../polynomial-interpolation.md) is unambiguous. The two interpolants agree at the $k-1$ common knots $t_{i+1},\ldots,t_{i+k-1}$. Their difference is consequently a scalar multiple of the monic [polynomial](../../../../../../polynomial-split.md) $\omega_i$ of degree $k-1$.

The leading coefficient of an interpolant is its highest [divided difference](../../../../../../divided-difference.md). Thus this scalar is

$$
[t_{i+1},\ldots,t_{i+k}]g_t-[t_i,\ldots,t_{i+k-1}]g_t
=(t_{i+k}-t_i)[t_i,\ldots,t_{i+k}]g_t=N_i(t).
$$

The equality is precisely the divided-difference recurrence. This proves **the [Lee interpolation identity](../../../../../../lee-interpolation-identity.md)**:

$$
\boxed{\ell_{i+1}(x,t)-\ell_i(x,t)=\omega_i(x)N_i(t).}
$$

For $k=1$ the common-knot product is empty; the same argument is a difference of constants. Interpret $(y-t)_+^0$ as $1_{y>t}$ to obtain the usual half-open order-one [B-splines](../../../../../../b-spline.md). Repeated knots use the standard confluent or limiting interpretation, where the interpolation data are defined.

Sum over $i=1,\ldots,n$. The right side telescopes to $\ell_{n+1}(x,t)-\ell_1(x,t)$. When $t_k<t<t_{n+1}$, the first interpolation nodes all lie below $t$, so $\ell_1=0$. The last interpolation nodes all lie above $t$, so $\ell_{n+1}$ interpolates the [polynomial](../../../../../../polynomial-split.md) $(x-t)^{k-1}$ of degree $k-1$ and equals it identically. Hence **the [Marsden identity](../../../../../../marsden-identity.md) follows**:

$$
\boxed{(x-t)^{k-1}=\sum_{i=1}^n\omega_i(x)N_i(t),\qquad t_k<t<t_{n+1}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
