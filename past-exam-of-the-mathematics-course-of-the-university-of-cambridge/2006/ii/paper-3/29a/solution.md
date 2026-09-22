<h1 id="29a/solution">Solution</h1>

↑ **Parent:** [29A](../29a.md)

Let $H_t(x)=(4\pi t)^{-n/2}e^{-|x|^2/(4t)}$ be the [heat kernel](../../../../../heat-kernel.md), and write $P_tg=H_t*g$. The homogeneous solution is $u(t,x)=P_tg(x)$: differentiation verifies the [heat equation](../../../../../heat-equation.md), and the approximate-identity property recovers the smooth initial data.

The [Duhamel principle](../../../../../duhamel-s-principle.md) gives

$$
\boxed{v(t,x)=P_tg(x)+\int_0^tP_{t-s}f(s,\cdot)(x)\,ds.}
$$

Each source impulse at time $s$ evolves by the homogeneous heat flow for duration $t-s$. More formally, differentiating the time integral gives $f(t,x)+\int_0^t\Delta P_{t-s}f(s)(x)\,ds$. Subtracting its Laplacian leaves $f$. The integral tends to zero as $t\downarrow0$, since its absolute value is at most $t\sup_{s\le t}\|f(s)\|_\infty$. Thus the initial condition is also correct. Smoothness permits differentiation locally; standard cutoff or semigroup arguments justify it for bounded smooth data without global bounds on all derivatives.

For $n=4$ and time-independent Schwartz $f$, integrate the kernel in time. For $r>0$, $\int_0^t(4\pi s)^{-2}e^{-r^2/(4s)}ds=e^{-r^2/(4t)}/(4\pi^2r^2)$. Consequently

$$
\boxed{v(t,x)=P_tg(x)+\frac1{4\pi^2}\int_{\mathbb R^4}\frac{e^{-|x-y|^2/(4t)}}{|x-y|^2}f(y)\,dy.}
$$

The forcing term converges by dominated convergence to $W(x)=(4\pi^2|\cdot|^2)^{-1}*f$. Its singularity is locally integrable in four dimensions, and the Schwartz decay controls infinity. The supplied fundamental solution identity gives $-\Delta W=f$, first in distributions and then classically by regularity.

**The asserted large-time limit is not guaranteed for arbitrary bounded smooth $g$.** Take $f=0$ and $g(x)=(1+|x|^2)^i$, which is smooth and has modulus one. For a standard four-dimensional [Gaussian](../../../../../normal-distribution.md) $Z$,

$$
P_tg(0)=t^i\mathbb E[(t^{-1}+2|Z|^2)^i]\sim4^i\Gamma(2+i)t^i.
$$

Dominated convergence gives the asymptotic, and the gamma factor is nonzero. The phase $\log t$ rotates indefinitely, so there is no limit. This is an example of [heat evolution of bounded data need not converge at large times](../../../../../heat-evolution-of-bounded-data-need-not-converge-at-large-times.md).

Under the natural additional assumption $g\in C_0(\mathbb R^4)$, $P_tg\to0$: split the convolution into a large ball, whose heat-kernel mass tends to zero, and its complement, where $g$ is uniformly small. Then $w=W$ and $-\Delta w=f$. More generally, if $g(x)\to L$ at spatial infinity, the limit is $w=L+W$, satisfying the same equation. These are the intended qualified stationary-limit conclusions.

## ↑ Ancestors (10)

1. [29A](../29a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
