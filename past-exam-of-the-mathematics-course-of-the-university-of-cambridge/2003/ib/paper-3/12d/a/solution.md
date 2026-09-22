<h1 id="12d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the impulse point is in the interior, $0<a<l$. Expand the displacement in the fixed-end [Fourier sine series](../../../../../../fourier-sine-series.md)

$$
y(x,t)=\sum_{n=1}^{\infty}T_n(t)\sin\frac{n\pi x}{l},\qquad \alpha_n=\frac{n\pi c}{l}.
$$

[Orthogonality](../../../../../../orthogonal-vectors.md) gives the initial velocity coefficient by applying the [Dirac delta](../../../../../../dirac-delta-function.md) to the sine function:

$$
T_n(0)=0,\qquad T_n'(0)=\frac2l\int_0^l\delta(x-a)\sin\frac{n\pi x}{l}\,dx=\frac2l\sin\frac{n\pi a}{l}.
$$

Substitution in the [wave equation](../../../../../../wave-equation-split.md) yields $T_n''+2kT_n'+\alpha_n^2T_n=0$. For $k<\alpha_n$, its roots are $-k\pm i\omega_n$, where $\omega_n=\sqrt{\alpha_n^2-k^2}$. The two initial conditions determine

$$
T_n(t)=\frac2l\sin\frac{n\pi a}{l}\,e^{-kt}\frac{\sin(\omega_nt)}{\omega_n}.
$$

Hence the normalized [velocity-impulse Green function for a damped string](../../../../../../velocity-impulse-green-function-for-a-damped-string.md) is

$$
\boxed{y(x,t)=\frac2l\sum_{n=1}^{\infty}\sin\frac{n\pi a}{l}\sin\frac{n\pi x}{l}\,e^{-kt}\frac{\sin\bigl(\sqrt{\alpha_n^2-k^2}\,t\bigr)}{\sqrt{\alpha_n^2-k^2}}.}
$$

For a mode with [critical damping](../../../../../../critical-damping.md), use the limit $e^{-kt}t$ in place of the time factor. For $k>\alpha_n$, put $\eta_n=\sqrt{k^2-\alpha_n^2}$ and use $e^{-kt}\sinh(\eta_nt)/\eta_n$. These choices solve the same modal [ordinary differential equation](../../../../../../ordinary-differential-equation.md) and initial conditions, so the formula covers arbitrary $k>0$. The impulse initial velocity is a [distribution](../../../../../../distribution-mathematical-analysis.md), so initial differentiation of the [series](../../../../../../series-mathematics.md) is interpreted distributionally.

**The printed formula requires correction:** the factor depending on $n$ must lie inside the sum, and sine-mode normalization requires $2/l$, rather than $2$. The printed slash after the final sine is also stray. Direct differentiation at $t=0$ verifies the corrected normalization: the initial sine coefficients are exactly those of $\delta(x-a)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12D](../../12d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
