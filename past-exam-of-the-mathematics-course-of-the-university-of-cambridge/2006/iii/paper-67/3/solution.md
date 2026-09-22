<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the periodic [modulus of continuity](../../../../../modulus-of-continuity.md)

$$
\omega(f,\delta)=\sup_{|h|\leq\delta}\sup_x|f(x+h)-f(x)|.
$$

Subdividing a displacement $t$ into at most $\lceil|t|/\delta\rceil$ steps of size at most $\delta$ proves the chaining inequality

$$
|f(x-t)-f(x)|\leq\left(1+\frac{|t|}{\delta}\right)\omega(f,\delta).
$$

For $|t|\leq\delta$, the sharper bound $\omega(f,\delta)$ holds directly.

Set $\delta=n^{-\alpha}$, where $0<\alpha<1$ and $n\geq1$. Positivity and unit normalized mass of the [Fejér kernel](../../../../../fejer-kernel.md) give

$$
|\sigma_n(f;x)-f(x)|\leq\frac1\pi\int_{-\pi}^{\pi}|f(x-t)-f(x)|F_n(t)\,dt.
$$

The portion $|t|\leq\delta$ is at most $\omega(f,\delta)$. For $0<|t|\leq\pi$, $\sin(|t|/2)\geq |t|/\pi$ and $|\sin(nt/2)|\leq1$, so

$$
F_n(t)\leq\frac{\pi^2}{2nt^2}.
$$

Apply this bound and the chaining inequality to the two tails:

$$
\begin{aligned}
\|\sigma_nf-f\|_\infty
&\leq\omega(f,\delta)\left[1+\frac\pi n\int_\delta^\pi\left(1+\frac t\delta\right)\frac{dt}{t^2}\right]\\
&=\omega(f,\delta)\left[1+\frac\pi n\left(\frac1\delta-\frac1\pi+\frac1\delta\log\frac\pi\delta\right)\right]\\
&\leq\omega(f,\delta)\left[1+\pi n^{\alpha-1}\bigl(1+\log\pi+\alpha\log n\bigr)\right].
\end{aligned}
$$

Let $\beta=1-\alpha>0$. Calculus gives $\sup_{u\geq1}u^{-\beta}\log u=1/(e\beta)$, attained at $u=e^{1/\beta}$, and $u^{-\beta}\leq1$. Thus a possible explicit constant for the [fractional-scale Fejér approximation bound](../../../../../fractional-scale-fejer-approximation-bound.md) is

$$
c_\alpha=1+\pi\left(1+\log\pi+\frac{\alpha}{e(1-\alpha)}\right),
\qquad\boxed{\|\sigma_nf-f\|_\infty\leq c_\alpha\omega(f,n^{-\alpha}).}
$$

The constant depends only on $\alpha$, not on $f$ or $n$. Since a continuous periodic [function](../../../../../function-split.md) is uniformly continuous, the right-hand side tends to zero. The logarithmic tail estimate is what permits every $\alpha<1$; a crude global-oscillation bound would not prove the whole requested range.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
