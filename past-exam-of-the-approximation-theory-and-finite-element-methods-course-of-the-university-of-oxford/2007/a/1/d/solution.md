<h1 id="a/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the [Fourier coefficients](../../../../../fourier-coefficient.md) as $c_k=(2\pi)^{-1}\int_{-\pi}^{\pi}u(t)e^{-ikt}dt$. The partial sum through frequencies $-n,\ldots,n$ is therefore a [convolution](../../../../../convolution.md) with

$$
D_n(\theta)=\sum_{k=-n}^ne^{ik\theta}
=\frac{\sin((n+1/2)\theta)}{\sin(\theta/2)}.
$$

The last expression follows by summing a finite [geometric series](../../../../../geometric-series.md), with its removable value $2n+1$ at zero. Periodicity and the evenness of $D_n$ give

$$
\boxed{s_n(x)=\frac1{2\pi}\int_{-\pi}^{\pi}
u(x+\theta)D_n(\theta)d\theta.}
$$

This also proves linearity and that the image lies in $F_n$. We use the continuous [periodic function](../../../../../periodic-function.md) space, consistent with the premise and the displayed maximum [norm](../../../../../norm.md).

The [convolution](../../../../../convolution.md) formula gives the upper bound

$$
\|S_nu\|_\infty\leq\frac{\|u\|_\infty}{2\pi}
\int_{-\pi}^{\pi}|D_n(\theta)|d\theta.
$$

To prove sharpness within continuous functions, take

$$
u_\epsilon(\theta)=\frac{D_n(\theta)}
{\sqrt{D_n(\theta)^2+\epsilon^2}}.
$$

It is continuous and periodic, with [norm](../../../../../norm.md) at most one. At $x=0$, dominated convergence gives $(S_nu_\epsilon)(0)\to(2\pi)^{-1}\int|D_n|$. Hence that upper bound is the actual [operator norm](../../../../../operator-norm.md). Evenness yields

$$
\boxed{\|S_n\|=\frac1\pi\int_0^\pi
\left|\frac{\sin((n+1/2)\theta)}{\sin(\theta/2)}\right|d\theta.}
$$

The approximating continuous signs avoid assuming that the discontinuous sign of the kernel belongs to the domain space.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
