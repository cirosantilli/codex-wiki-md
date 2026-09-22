<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $n\geq1$, the [Bernstein polynomial](../../../../../bernstein-polynomial.md) is

$$
B_n(f;x)=\sum_{j=0}^nf(j/n)\binom njx^j(1-x)^{n-j}.
$$

The weights sum to one by the [binomial theorem](../../../../../binomial-theorem.md). Equivalently, if $K$ has the [binomial distribution](../../../../../binomial-distribution.md) with parameters $n,x$, then $B_n(f;x)=\mathbb E f(K/n)$. This interpretation makes the cancellation of apparent high-degree terms transparent.

For the [falling factorial](../../../../../falling-factorial.md) $u^{\underline r}=u(u-1)\cdots(u-r+1)$, with $u^{\underline0}=1$, direct cancellation in the binomial weights gives

$$
\begin{aligned}
\mathbb E K^{\underline r}
&=\sum_{j=r}^nj^{\underline r}\binom njx^j(1-x)^{n-j}\\
&=n^{\underline r}x^r\sum_{j=r}^n\binom{n-r}{j-r}x^{j-r}(1-x)^{n-j}
=n^{\underline r}x^r.
\end{aligned}
$$

The [polynomials](../../../../../polynomial-split.md) $u^{\underline0},\ldots,u^{\underline m}$ form a monic triangular [basis](../../../../../basis.md) of the degree-at-most-$m$ [polynomials](../../../../../polynomial-split.md). Hence $u^m=u^{\underline m}+\sum_{r<m}c_r u^{\underline r}$, and

$$
B_n(x^m;x)=\frac{n^{\underline m}}{n^m}x^m+\sum_{r<m}c_r\frac{n^{\underline r}}{n^m}x^r.
$$

For $m\leq n$, its [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) is $n^{\underline m}/n^m\ne0$. If $p$ has actual degree $m$ and [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) $a_m\ne0$, linearity shows that the [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) of $B_np$ is $a_mn^{\underline m}/n^m$; lower-degree terms cannot cancel it. Thus the [Bernstein polynomial degree preservation](../../../../../bernstein-polynomial-degree-preservation.md) property gives

$$
\boxed{\deg B_np=m\quad\text{whenever }\deg p=m\leq n.}
$$

This includes the requested $m<n$, and also explains why the property cannot simply be extended to $m>n$.

The same moments give $\mathbb EK=nx$ and $\mathbb EK^2=n(n-1)x^2+nx$. Therefore

$$
\boxed{B_n1=1,\qquad B_nx=x,\qquad B_n(x^2)=x^2+\frac{x(1-x)}n.}
$$

The first two approximation errors vanish identically, while

$$
\boxed{\|B_n(x^2)-x^2\|_\infty=\frac1{4n}\longrightarrow0.}
$$

All three convergences are consequently [uniform convergence](../../../../../uniform-convergence.md) on $[0,1]$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
