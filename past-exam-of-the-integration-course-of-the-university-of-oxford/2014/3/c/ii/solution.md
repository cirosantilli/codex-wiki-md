<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define the joint [function](../../../../../function-split.md) by an unambiguous piecewise prescription:

$$
H(x,y)=\begin{cases}(x-y)^{\beta-1}f(y),&0<y<x<1,\\0,&\text{otherwise in }(0,1)^2.\end{cases}
$$

It is nonnegative and [Lebesgue measurable](../../../../../lebesgue-measurable-set.md): on the open triangle the power factor is continuous and $f(y)$ is measurable for the [product sigma-algebra](../../../../../product-sigma-algebra.md), and the zero extension is measurable. This also resolves the diagonal singularity and avoids evaluating a noninteger power of a negative number outside the triangle. The source's inclusion of $y=x$ in its indicator [set](../../../../../set-split.md) changes only a [null set](../../../../../null-set.md); set the value there to zero.

The [function](../../../../../function-split.md) $g(x)=\int_0^1H(x,y)\,dy$ is measurable by [Tonelli's theorem](../../../../../tonelli-theorem.md). Apply that theorem to exchange the nonnegative [integrals](../../../../../integral-split.md), with infinity allowed until the estimate proves otherwise:

$$
\begin{aligned}
\int_0^1g(x)\,dx
&=\int_0^1f(y)\left(\int_y^1(x-y)^{\beta-1}\,dx\right)dy\\
&=\frac1\beta\int_0^1(1-y)^\beta f(y)\,dy\\
&\leq\frac1\beta\int_0^1f(y)\,dy<\infty.
\end{aligned}
$$

The inner [integral](../../../../../integral-split.md) is $(1-y)^\beta/\beta$ because $\beta>0$. The weight is at most one because $0<y<1$. Since $g\geq0$, this proves

$$
\boxed{\|g\|_1=\frac1\beta\int_0^1(1-y)^\beta f(y)\,dy
\leq\frac1\beta\|f\|_1,\qquad g\in L^1((0,1)).}
$$

In particular $g$ is finite [almost everywhere](../../../../../almost-everywhere.md); any exceptional infinite values may be replaced by zero to obtain an everywhere finite representative. This is the [L1 bound for a Volterra power-kernel integral](../../../../../l1-bound-for-a-volterra-power-kernel-integral.md).

An everywhere-finite conclusion would be stronger and can fail when $0<\beta<1$, even for integrable $f$. For example, put $x_0=1/2$ and $\gamma=(1+\beta)/2$, and take $f(y)=(x_0-y)^{-\gamma}$ for $0<y<x_0$ and zero otherwise. Since $\gamma<1$, $f$ is integrable. But

$$
g(x_0)=\int_0^{x_0}(x_0-y)^{\beta-1-\gamma}\,dy=\infty,
$$

because $\beta-1-\gamma=(\beta-3)/2<-1$. This does not contradict [Lebesgue integrability](../../../../../integrability.md), which requires finiteness only [almost everywhere](../../../../../almost-everywhere.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
