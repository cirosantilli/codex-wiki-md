<h1 id="19d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Peano kernel theorem](../../../../../../peano-kernel-theorem.md) says that if a continuous linear error functional $L$ annihilates all polynomials of degree less than $r$ and permits the required interchange with integration, then for $f\in C^r[a,b]$,

$$
L(f)=\int_a^bK(\theta)f^{(r)}(\theta)\,d\theta,\qquad
K(\theta)=L\left[\frac{(x-\theta)_+^{r-1}}{(r-1)!}\right].
$$

It follows by applying $L$ to the integral-remainder [Taylor formula with integral remainder](../../../../../../taylor-formula-with-integral-remainder.md). Here choose $r=2$ and

$$
L(f)=f(1)-\frac13f(0)-f(2)+\frac13f(3).
$$

This functional annihilates constants and linear functions (indeed quadratics too), and its [Peano kernel](../../../../../../peano-kernel.md) is

$$
K(\theta)=(1-\theta)_+-(2-\theta)_++\frac13(3-\theta)_+
=\begin{cases}
-\theta/3,&0\leq\theta\leq1,\\
2\theta/3-1,&1\leq\theta\leq2,\\
1-\theta/3,&2\leq\theta\leq3.
\end{cases}
$$

Thus $\int_0^3|K|\,d\theta=1/2$ and $\max|K|=1/3$. The integral representation gives

$$
\boxed{\alpha_{\min}=\frac12,\qquad\beta_{\min}=\frac13.}
$$

For the first inequality, continuous functions $f''$ with $\|f''\|_\infty\leq1$ can approximate $\operatorname{sgn}K$ away from its zeros, making $L(f)$ arbitrarily close to $\int|K|$. Such derivatives integrate twice to admissible $C^2$ functions, proving no smaller $\alpha$ works. For the second, use continuous $f''$ of $L^1$ norm one concentrated near $\theta=1$ or $2$, where $|K|=1/3$, with the sign of $K$ there. This makes $|L(f)|$ approach $1/3$, proving optimality of $\beta$.

For $f=x^3$, $L(f)=2$, $\max|f''|=18$ and $\|f''\|_1=27$. Both right-hand bounds equal nine, so **both inequalities hold**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [19D](../../19d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
