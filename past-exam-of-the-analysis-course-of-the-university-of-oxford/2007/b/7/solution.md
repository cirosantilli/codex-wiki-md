<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The classical [Fourier partial sums](../../../../fourier-partial-sum.md) are

$$
s_n^f(t)=\frac{a_0}2+\sum_{j=1}^n[a_j\cos jt+b_j\sin jt],\quad a_j=\frac1\pi\int_{-\pi}^\pi f(t)\cos jt\,dt,\quad b_j=\frac1\pi\int_{-\pi}^\pi f(t)\sin jt\,dt.
$$

Here $a_0=\pi^{-1}\int f$, and functions are extended periodically. One version of the [Dini test for Fourier series](../../../../dini-test-for-fourier-series.md) states that if one-sided limits $L_+,L_-$ at $t$ exist and

$$
\int_0^\delta\frac{|f(t+s)+f(t-s)-L_+-L_-|}{s}\,ds<\infty,
$$

then $s_n^f(t)\to(L_++L_-)/2$. A [step function](../../../../step-function.md) on a finite interval is constant on each side of any given point for sufficiently small distance, so its displayed numerator is zero there. [Dini test for Fourier series](../../../../dini-test-for-fourier-series.md) gives exactly the asserted midpoint of the two one-sided values, including at jumps.

Let $P_n=s_n$ on $L^2$. It is the [orthogonal projection](../../../../orthogonal-projection.md) onto the span of the displayed trigonometric functions through frequency $n$, hence $\|P_n\|\leq1$. For a step-function approximation $\psi$,

$$
\|P_nf-f\|_2\leq\|P_n(f-\psi)\|_2+\|P_n\psi-\psi\|_2+\|\psi-f\|_2\leq2\|f-\psi\|_2+\|P_n\psi-\psi\|_2.
$$

The [convergence on a dense set under a uniform operator bound](../../../../banach-steinhaus-convergence-theorem.md), here applied using the allowed convergence for $\psi$ and density of [step functions](../../../../step-function.md), proves **$P_nf\to f$ in $L^2$**. Consequently the union of these finite trigonometric spans is dense, which is precisely [completeness](../../../../completeness.md) of the [orthonormal system](../../../../orthonormal-sequence.md). It also proves Parseval's equality by passing to the limit in the Pythagorean projection identity.

For $f(t)=t^2$, oddness gives $b_j=0$, direct integration gives $a_0=2\pi^2/3$, and two integrations by parts give $a_j=4(-1)^j/j^2$. Thus

$$
\boxed{t^2=\frac{\pi^2}3+4\sum_{j\geq1}\frac{(-1)^j\cos jt}{j^2}.}
$$

[Dini test for Fourier series](../../../../dini-test-for-fourier-series.md) justifies this pointwise on the interval, or absolute coefficient summability gives its continuous extension after the $L^2$ identification. At zero it yields **$\sum_{j\geq1}(-1)^{j-1}/j^2=\pi^2/12$**. Parseval gives

$$
\frac{2\pi^5}5=\int_{-\pi}^\pi t^4dt=\frac\pi2\left(\frac{2\pi^2}3\right)^2+16\pi\sum_{j\geq1}\frac1{j^4}.
$$

Therefore **$\sum_{j\geq1}j^{-4}=\pi^4/90$**.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
