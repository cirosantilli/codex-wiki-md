<h1 id="19c/solution">Solution</h1>

↑ **Parent:** [19C](../19c.md)

Assume $L$ is linear, annihilates all [polynomials](../../../../../polynomial-split.md) of degree at most $k$, is defined on the truncated-power kernels and permits interchange with the remainder integral. For $k\geq1$, a convenient sufficient condition is that $L$ be a [bounded linear functional](../../../../../continuous-linear-functional.md) on $C[a,b]$; more general approximation functionals need the corresponding continuity/interchange property on their domain. Taylor's integral remainder gives

$$
f(x)=\sum_{j=0}^k\frac{f^{(j)}(a)}{j!}(x-a)^j
+\frac1{k!}\int_a^b(x-\theta)_+^k f^{(k+1)}(\theta)\,d\theta.
$$

Applying $L$, the [polynomial](../../../../../polynomial-split.md) terms vanish, and the [Peano kernel theorem](../../../../../peano-kernel-theorem.md) gives

$$
\boxed{L(f)=\frac1{k!}\int_a^bK(\theta)f^{(k+1)}(\theta)\,d\theta,\qquad
K(\theta)=L[(x-\theta)_+^k].}
$$

Here $t_+=\max(t,0)$. This is the printed raw-kernel convention; the normalized [Peano kernel](../../../../../peano-kernel.md) includes $1/k!$ inside its definition instead, and then has no factorial outside the integral. The interchange is justified by boundedness applied to the limit of Riemann sums of the continuous kernel-valued integrand. For a kernel with $k=0$, its discontinuity requires a function space/interchange assumption accommodating the step functions as well.

For the specified [Simpson's rule](../../../../../simpson-s-rule.md) error, direct evaluation on $1,x,x^2,x^3$ gives zero, so $k=3$. For $0\leq\theta\leq2$,

$$
K(\theta)=\frac{(2-\theta)^4}{4}
-\frac43(1-\theta)_+^3-\frac13(2-\theta)^3.
$$

Simplifying separately on the two halves gives

$$
\boxed{K(\theta)=\begin{cases}
-\theta^3(4-3\theta)/12,&0\leq\theta\leq1,\\
-(2-\theta)^3(3\theta-2)/12,&1\leq\theta\leq2.
\end{cases}}
$$

Both pieces are strictly negative in the open interval; they agree at the midpoint. Their integral is $-1/15$, as direct [polynomial](../../../../../polynomial-split.md) integration shows. Thus

$$
|L(f)|\leq\frac1{6}\int_0^2|K(\theta)|\,d\theta\,\|f^{(4)}\|_\infty
=\boxed{\frac1{90}\|f^{(4)}\|_\infty.}
$$

This is optimal, not merely an upper bound. For $f(x)=x^4/24$, the fourth [derivative](../../../../../derivative.md) is identically one and $L(f)=-1/90$, so **the minimum constant is $\rho=1/90$**.

## ↑ Ancestors (10)

1. [19C](../19c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
