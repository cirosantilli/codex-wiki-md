<h1 id="14b/solution">Solution</h1>

↑ **Parent:** [14B](../14b.md)

Write $y=\sum_{k\ge0}c_kx^k$ with $c_0=1$. Substitution into the [ordinary differential equation](../../../../../ordinary-differential-equation.md) gives

$$
(k+1)^2c_{k+1}+(\lambda-k)c_k=0,\qquad c_k=\frac{\prod_{j=0}^{k-1}(j-\lambda)}{(k!)^2}.
$$

Unless the series terminates, its coefficient ratio is $O(1/k)$, so it converges for every finite $x$. A coefficient first vanishes exactly when $\lambda$ is a nonnegative integer $n$, and then $c_n=(-1)^n/n!\ne0$, $c_{n+1}=0$. Thus **$y$ is a [polynomial](../../../../../polynomial-split.md) precisely for $\lambda=n\in\{0,1,2,\ldots\}$**, in which case

$$
y_n(x)=\sum_{k=0}^n(-1)^k\binom nk\frac{x^k}{k!}
$$

is the normalized [Laguerre polynomial](../../../../../laguerre-polynomial.md).

Multiplying the differential equation by $e^{-x}$ gives $(xe^{-x}y_n')'+ne^{-x}y_n=0$. Multiply by $y_m$, subtract the equation with the indices exchanged, and integrate over $[0,\infty)$. The boundary term $xe^{-x}(y_my_n'-y_ny_m')$ vanishes both at zero and infinity. Therefore

$$
\boxed{\int_0^\infty e^{-x}y_m(x)y_n(x)\,dx=0\quad(m\ne n).}
$$

This is the weighted [orthogonality](../../../../../orthogonal-vectors.md) of the [Laguerre polynomials](../../../../../laguerre-polynomial.md).

Their leading coefficients show $\deg(y_my_n)=m+n$. Since $y_0,\ldots,y_{m+n}$ have distinct degrees, they form a basis of that [polynomial](../../../../../polynomial-split.md) space. Hence $y_my_n=\sum_{p=0}^{m+n}a_py_p$, and comparison of leading coefficients gives **$a_{m+n}=(m+n)!/(m!n!)\ne0$**. Likewise the degrees of $y_m$ and $y_my_n$ for $0\le m<n$ run through $0,\ldots,n-1$ and $n,\ldots,2n-1$, respectively. A nontrivial [linear combination](../../../../../linear-combination.md) cannot cancel its highest-degree term, so these $2n$ functions are [linearly independent](../../../../../linear-independence.md).

For $n=2$, this gives the basis $y_0,y_1,y_2,y_1y_2$ of the cubic [polynomial](../../../../../polynomial-split.md) space, establishing the specified expansion. Its weighted [integral](../../../../../integral.md) is $a_0$: $y_0=1$ integrates to one, $y_1$ and $y_2$ are orthogonal to $y_0$, and $y_1y_2$ integrates to zero. At the two roots $\alpha_1,\alpha_2$ of $y_2$, the expansion reduces to $f(\alpha_i)=a_0+a_1y_1(\alpha_i)$. Solving these two equations for $a_0$ gives

$$
\boxed{\int_0^\infty e^{-x}f(x)\,dx=w_1f(\alpha_1)+w_2f(\alpha_2),\quad w_1=\frac{y_1(\alpha_2)}{y_1(\alpha_2)-y_1(\alpha_1)},\quad w_2=\frac{-y_1(\alpha_1)}{y_1(\alpha_2)-y_1(\alpha_1)}.}
$$

For explicit verification, the recurrence gives $y_1=1-x$, $y_2=1-2x+x^2/2$. Thus $\alpha_1=2-\sqrt2$, $\alpha_2=2+\sqrt2$ are distinct positive roots and $w_1=(2+\sqrt2)/4$, $w_2=(2-\sqrt2)/4$. This is the two-node [Gauss-Laguerre quadrature](../../../../../gauss-laguerre-quadrature.md) rule, exact for every cubic.

## ↑ Ancestors (10)

1. [14B](../14b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
