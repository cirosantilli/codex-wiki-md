<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $T=\epsilon t$ and use the [method of multiple scales](../../../../../../method-of-multiple-scales.md):

$$
y=y_0(t,T)+\epsilon y_1(t,T)+\cdots,\qquad
y_0=a(T)\cos(t/2)+b(T)\sin(t/2).
$$

Since $\omega^2=1/4+k\epsilon+O(\epsilon^2)$, the first correction satisfies

$$
(\partial_t^2+1/4)y_1=-2\partial_t\partial_Ty_0-(k+\cos t)y_0.
$$

The resonant cosine and sine coefficients must vanish to avoid [secular terms](../../../../../../secular-term.md). Using the product-to-sum formulas gives

$$
\boxed{a_T=(k-1/2)b,\qquad b_T=-(k+1/2)a.}
$$

The remaining forcing has [frequency](../../../../../../frequency.md) $3/2$ and permits the bounded particular correction $y_1=(a/4)\cos(3t/2)+(b/4)\sin(3t/2)$. The two slow [amplitudes](../../../../../../wave-amplitude.md) carry the two arbitrary constants of the original equation.

For an explicit general leading solution, put

$$
M=\begin{pmatrix}0&k-1/2\\-(k+1/2)&0\end{pmatrix},\qquad
\lambda^2=1/4-k^2,\qquad M^2=\lambda^2I.
$$

The [matrix exponential](../../../../../../matrix-exponential.md) gives

$$
\begin{pmatrix}a(T)\\b(T)\end{pmatrix}
=\left[\cosh(\lambda T)I+\frac{\sinh(\lambda T)}{\lambda}M\right]
\begin{pmatrix}a(0)\\b(0)\end{pmatrix},
\qquad
\boxed{y(t)=a(\epsilon t)\cos(t/2)+b(\epsilon t)\sin(t/2)+O(\epsilon).}
$$

The error is uniform on bounded intervals of $T$, for bounded initial data. When $\lambda$ is imaginary this expression uses ordinary sine and cosine; at $\lambda=0$ its continuous limit is $I+TM$.

The [primary instability tongue of a weak Mathieu oscillator](../../../../../../primary-instability-tongue-of-a-weak-mathieu-oscillator.md) has a positive slow [eigenvalue](../../../../../../eigenvalue.md) precisely when

$$
\boxed{-\frac12<k<\frac12,\qquad
\text{growth rate}=\epsilon\sqrt{\frac14-k^2}+O(\epsilon^2).}
$$

These are the leading edges, rather than an exact finite-$\epsilon$ interval. At the leading endpoints the [amplitude](../../../../../../wave-amplitude.md) matrix is a [nilpotent matrix](../../../../../../nilpotent-matrix.md), so the leading solution can grow linearly in $T$ and does not decide the exact exponential instability. For completeness, set $\omega=1/2+\beta\epsilon+\gamma\epsilon^2$. The periodic or antiperiodic edge calculation uses a pure cosine when $\beta=-1/2$ and a pure sine when $\beta=1/2$, with the third-harmonic correction just found. The next resonant coefficient is $-(\gamma+3/8)y_0$, so

$$
\omega_-=\frac12-\frac\epsilon2-\frac38\epsilon^2+O(\epsilon^3),\qquad
\omega_+=\frac12+\frac\epsilon2-\frac38\epsilon^2+O(\epsilon^3).
$$

Thus the exact growing interval is between these shifted edges. In particular, for positive small $\epsilon$ the fixed leading value $k=-1/2$ lies just inside it, whereas $k=1/2$ lies just outside. Interior detunings bounded away from the edges are already resolved by the leading [method of multiple scales](../../../../../../method-of-multiple-scales.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
