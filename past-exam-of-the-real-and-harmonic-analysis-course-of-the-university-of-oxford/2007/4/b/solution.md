<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [summability kernel on the circle](../../../../summability-kernel-on-the-circle.md) is a sequence of continuous periodic functions with

$$
\int k_n\,dm=1,\qquad \sup_n\|k_n\|_1=C<\infty,\qquad\int_{\delta\leq|t|\leq\pi}|k_n(t)|\,dm(t)\longrightarrow0\quad(0<\delta<\pi).
$$

The frequently used stronger condition of uniform convergence to zero off each neighborhood of zero implies the last condition. For $f$ in a homogeneous [Banach space](../../../../banach-space-split.md),

$$
\|f*k_n-f\|_B\leq\int|k_n(s)|\|\tau_sf-f\|_B\,dm(s).
$$

Given $\varepsilon>0$, translation continuity bounds the difference inside a sufficiently small neighborhood by $\varepsilon$; its integral is at most $C\varepsilon$. Outside, use $2\|f\|_B$ and the vanishing tail condition. Hence $f*k_n\to f$ in $B$.

With the indexing needed in part (c), the [Fejér kernel](../../../../fejer-kernel.md) is

$$
K_n(t)=\frac1{n+1}\left|\sum_{r=0}^n e^{irt}\right|^2=\sum_{|j|\leq n}\left(1-\frac{|j|}{n+1}\right)e^{ijt},\qquad n\geq0.
$$

In particular $K_0=1$. The squared-modulus expression proves $K_n\geq0$, and its constant [Fourier coefficient](../../../../fourier-coefficient.md) proves $\int K_n\,dm=\|K_n\|_1=1$. The [geometric series](../../../../geometric-series.md) yields

$$
K_n(t)=\frac1{n+1}\frac{\sin^2((n+1)t/2)}{\sin^2(t/2)}\leq\frac1{(n+1)\sin^2(\delta/2)}\quad(\delta\leq|t|\leq\pi).
$$

Thus these are summability kernels. For $T_f:g\mapsto f*g$, part (a) gives $\|T_f\|\leq\|f\|_B$. Since $\|K_n\|_1=1$ and $T_fK_n\to f$ in $B$, the reverse bound follows:

$$
\boxed{\|T_f:L^1(\mathbb T)\to B\|=\|f\|_B.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../split.md)
5. [Real and harmonic analysis course of the University of Oxford](../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
