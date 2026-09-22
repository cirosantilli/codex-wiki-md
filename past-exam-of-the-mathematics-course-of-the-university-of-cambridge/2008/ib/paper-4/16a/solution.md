<h1 id="16a/solution">Solution</h1>

↑ **Parent:** [16A](../16a.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widetilde F(\omega)=\int_{\mathbb R}F(x)e^{-i\omega x}\,dx$. Reindexing the convergent [periodization of an integrable function](../../../../../periodization-of-an-integrable-function.md) gives $g(\tau+2\pi)=g(\tau)$; absolute integrability also ensures that the defining sum is absolutely convergent almost everywhere in a period. To calculate its [Fourier series](../../../../../fourier-series-split.md) coefficients, [uniform convergence](../../../../../uniform-convergence.md) permits passing the limit of the partial sums through the finite-interval integral. Changing variables $x=\tau+2\pi k$ and using $e^{2\pi ink}=1$ gives

$$
c_n=\frac1{2\pi}\int_0^{2\pi}g(\tau)e^{-in\tau}\,d\tau=\frac1{2\pi}\sum_{k\in\mathbb Z}\int_{2\pi k}^{2\pi(k+1)}F(x)e^{-inx}\,dx=\boxed{\frac{\widetilde F(n)}{2\pi}}.
$$

The sum of these integrals is absolutely convergent, bounded by $\int_{\mathbb R}|F|$, so the last rearrangement is justified. This proves the proposed Fourier expansion at the level of coefficients.

There is a genuine missing hypothesis in the pointwise assertion as printed. Take $F(x)=\mathbf1_{\{0\}}(x)$. It is absolutely integrable with integral zero, and its periodization has only finitely many nonzero terms on $[0,2\pi]$, so the series converges uniformly there. Yet $g(0)=1$ while $\widetilde F(n)=0$ for every $n$. Thus **the displayed pointwise identity does not follow from the stated assumptions**. Additional regularity ensuring Fourier convergence to the prescribed values of $g$, for example a continuous piecewise continuously differentiable periodization, makes the coefficient identity into the intended [Poisson summation formula](../../../../../poisson-summation-formula.md).

The particular function $F(x)=e^{-|x|}$ satisfies that stronger condition. Direct integration yields

$$
\widetilde F(\omega)=\frac1{1+i\omega}+\frac1{1-i\omega}=\frac2{1+\omega^2}.
$$

On $0\leq\tau\leq2\pi$, summing the two geometric tails gives $g(\tau)=\cosh(\tau-\pi)/\sinh\pi$, a continuous periodic function which is piecewise smooth. Its [Fourier series](../../../../../fourier-series-split.md) has absolutely summable coefficients and converges to $g$. At $\tau=0$,

$$
g(0)=1+2\sum_{k=1}^{\infty}e^{-2\pi k}=\frac{1+e^{-2\pi}}{1-e^{-2\pi}}=\coth\pi=\frac1\pi\sum_{n\in\mathbb Z}\frac1{1+n^2}.
$$

Consequently

$$
\boxed{\sum_{n=-\infty}^{\infty}\frac1{1+n^2}=\pi\coth\pi.}
$$

## ↑ Ancestors (10)

1. [16A](../16a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
