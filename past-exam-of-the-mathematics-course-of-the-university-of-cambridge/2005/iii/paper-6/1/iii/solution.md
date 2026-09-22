<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use $\mathbb T=\mathbb R/(2\pi\mathbb Z)$ and normalized measure $dt/(2\pi)$. The [Fourier partial sum](../../../../../../fourier-partial-sum.md) at zero is the real [linear functional](../../../../../../linear-functional.md)

$$
L_Nf=S_N(f,0)=\frac1{2\pi}\int_{-\pi}^{\pi}f(t)D_N(t)\,dt,
$$

where the [Dirichlet kernel](../../../../../../dirichlet-kernel.md) is

$$
D_N(t)=\sum_{j=-N}^Ne^{ijt}=\frac{\sin((N+\tfrac12)t)}{\sin(t/2)}.
$$

The quotient follows by summing the finite [geometric progression](../../../../../../geometric-progression.md), with its removable value $D_N(0)=2N+1$. It is a real [continuous](../../../../../../continuous-function.md) [periodic function](../../../../../../periodic-function.md). If

$$
\Lambda_N=\frac1{2\pi}\int_{-\pi}^{\pi}|D_N(t)|\,dt,
$$

then $|L_Nf|\leq\Lambda_N\|f\|_\infty$. This bound is its exact [operator norm](../../../../../../operator-norm.md) even on the real [continuous](../../../../../../continuous-function.md) functions. Indeed, for $\delta>0$ set

$$
f_{N,\delta}(t)=\frac{D_N(t)}{\sqrt{D_N(t)^2+\delta^2}}.
$$

It is real, [continuous](../../../../../../continuous-function.md) and periodic with [norm](../../../../../../norm.md) at most one, and

$$
L_Nf_{N,\delta}=\frac1{2\pi}\int_{-\pi}^{\pi}
\frac{D_N(t)^2}{\sqrt{D_N(t)^2+\delta^2}}\,dt\longrightarrow\Lambda_N
$$

by [dominated convergence](../../../../../../dominated-convergence-theorem.md). At zeros of the kernel the integrand is zero, and elsewhere its limit is $|D_N|$.

For $0<t\leq\pi$, $\sin(t/2)\leq t/2$. Using evenness and putting $v=(N+1/2)t$ gives

$$
\Lambda_N\geq\frac2\pi\int_0^{(N+1/2)\pi}\frac{|\sin v|}{v}\,dv
\geq\frac4{\pi^2}\sum_{j=1}^N\frac1j.
$$

For the last inequality, split into the first $N$ complete intervals $[(j-1)\pi,j\pi]$: their sine integrals are two and $1/v\geq1/(j\pi)$. The [harmonic sum](../../../../../../harmonic-sum.md) tends to infinity. This proves the [Dirichlet kernel harmonic lower bound](../../../../../../dirichlet-kernel-harmonic-lower-bound.md).

Choose $N$ with $\Lambda_N>K$, then choose $\delta$ sufficiently small that $L_Nf_{N,\delta}>K$. Thus

$$
\boxed{\|f_{N,\delta}\|_\infty\leq1,\qquad |S_N(f_{N,\delta},0)|>K.}
$$

This constructs [continuous](../../../../../../continuous-function.md) near-maximizers, rather than using the discontinuous sign of the kernel as the desired function.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
