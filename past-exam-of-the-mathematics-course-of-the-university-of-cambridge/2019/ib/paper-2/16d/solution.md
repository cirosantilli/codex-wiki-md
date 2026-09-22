<h1 id="16d/solution">Solution</h1>

↑ **Parent:** [16D](../16d.md)

Multiply the [Gegenbauer differential equation](../../../../../gegenbauer-differential-equation.md) by

$$
w(x)=(1-x^2)^{\alpha-1/2}.
$$

It becomes the [Sturm-Liouville form](../../../../../sturm-liouville-form.md)

$$
\frac d{dx}\left((1-x^2)^{\alpha+1/2}y'\right)
+n(n+2\alpha)w(x)y=0.
$$

For two polynomial solutions of degrees $m\ne n$, multiply their equations crosswise, subtract, and integrate over $(-1,1)$. The boundary term vanishes because $\alpha>0$ and $(1-x^2)^{\alpha+1/2}\to0$. Since the eigenvalues $n(n+2\alpha)$ are distinct,

$$
\boxed{\int_{-1}^1C_m^\alpha(x)C_n^\alpha(x)(1-x^2)^{\alpha-1/2}\,dx=0}.
$$

Thus $a=-1$, $b=1$, and the displayed function is the weight.

Every interior root is simple: a solution and its derivative cannot both vanish at an ordinary point of a second-order linear differential equation unless the solution is identically zero. Let $x_1,\ldots,x_k$ be all interior roots and put $q(x)=\prod_i(x-x_i)$. If $k<n$, then $q$ has degree below $n$, so [orthogonality](../../../../../orthogonal-polynomial.md) gives

$$
\int_{-1}^1C_n^\alpha(x)q(x)w(x)\,dx=0.
$$

But $C_n^\alpha/q$ has no zero and constant sign on $(-1,1)$, whence the integrand $q(x)^2(C_n^\alpha(x)/q(x))w(x)$ has one strict sign except at finitely many points. Its integral cannot vanish, a contradiction. Therefore $k=n$: all $n$ roots are real, simple, and lie in $(-1,1)$.

## ↑ Ancestors (10)

1. [16D](../16d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
