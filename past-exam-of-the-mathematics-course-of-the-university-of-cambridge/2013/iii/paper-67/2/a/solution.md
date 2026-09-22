<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $0<\epsilon\ll1$ and $X,Y,\alpha=O(1)$. For $n=2$, use the [method of multiple scales](../../../../../../method-of-multiple-scales.md) with $T=\epsilon t$ and [complex amplitudes](../../../../../../complex-amplitude.md)

$$
x_0=A(T)e^{it}+\overline A(T)e^{-it},\qquad y_0=B(T)e^{2it}+\overline B(T)e^{-2it}.
$$

At first order the forcing equations are

$$
(\partial_{t_0}^2+1)x_1=-2\partial_{t_0}\partial_Tx_0-\alpha x_0-x_0y_0,\qquad
(\partial_{t_0}^2+4)y_1=-2\partial_{t_0}\partial_Ty_0-x_0y_0.
$$

The product has [frequencies](../../../../../../frequency.md) $\pm1,\pm3$. Its $e^{it}$ coefficient is $\overline A B$, while it has no $e^{2it}$ coefficient. Removing the [secular terms](../../../../../../secular-term.md) gives

$$
2iA_T+\alpha A+B\overline A=0,\qquad B_T=0.
$$

The leading initial conditions give $A(0)=X/2$ and $B=Y/2$. Put $b=Y/2$, $A=p+iq$. The [primary parametric resonance of a two-to-one oscillator pair](../../../../../../primary-parametric-resonance-of-a-two-to-one-oscillator-pair.md) is governed by

$$
p_T=-\frac{\alpha-b}{2}q,\qquad q_T=\frac{\alpha+b}{2}p,\qquad
\lambda^2=\frac{b^2-\alpha^2}{4}.
$$

For $b^2>\alpha^2$, choose $\lambda>0$. Solving with $p(0)=X/2,q(0)=0$ yields

$$
\boxed{x(t)=X\left[\cosh(\lambda\epsilon t)\cos t-\frac{\alpha+b}{2\lambda}\sinh(\lambda\epsilon t)\sin t\right]+O(\epsilon),\quad
y(t)=Y\cos2t+O(\epsilon)}.
$$

If $b^2<\alpha^2$, let $\nu=\sqrt{\alpha^2-b^2}/2$; replace $\cosh(\lambda T)$ by $\cos(\nu T)$ and $\sinh(\lambda T)/\lambda$ by $\sin(\nu T)/\nu$. On the boundary $b^2=\alpha^2$, take the continuous limit:

$$
x(t)=X\left[\cos t-\frac{\alpha+b}{2}\epsilon t\sin t\right]+O(\epsilon).
$$

Thus **exponential growth occurs when $|Y|>2|\alpha|$ and $X\ne0$**, on the scale $t=O(\epsilon^{-1})$. Equality is a marginal case that can produce linear slow growth: for $b=\alpha\ne0$ the displayed initial phase excites it, whereas for $b=-\alpha$ it does not. If $X=0$, $x$ stays identically zero and the other oscillator is exactly uncoupled. The leading $y$ [amplitude](../../../../../../wave-amplitude.md) is constant; its backreaction is a higher-order effect on this time scale.

These are leading approximations for bounded [slow time](../../../../../../slow-time.md) $T$, hence $t=O(\epsilon^{-1})$, while the [amplitudes](../../../../../../wave-amplitude.md) stay $O(1)$. First-order corrections can enforce the initial velocities exactly; the leading formula alone has an $O(\epsilon)$ initial-velocity mismatch. In the unstable case the expansion must not be extrapolated through arbitrarily large amplification, where weak coupling and omitted terms cease to be uniform.

For $n=1$, both leading oscillations have [frequencies](../../../../../../frequency.md) $\pm1$, so their quadratic product contains only [frequencies](../../../../../../frequency.md) $0,\pm2$. There is no first-order resonant coupling: the [solvability condition in the method of multiple scales](../../../../../../solvability-condition-in-the-method-of-multiple-scales.md) gives $A_T=i\alpha A/2$ and $B_T=0$, a [frequency](../../../../../../frequency.md) shift without first-order [amplitude](../../../../../../wave-amplitude.md) growth. The constant and second-harmonic corrections can feed back into the fundamental at second order. Consequently the first possible growth scale from this [second-order resonance from quadratic oscillator coupling](../../../../../../second-order-resonance-from-quadratic-oscillator-coupling.md) is

$$
\boxed{T_2=\epsilon^2t=O(1),\qquad t=O(\epsilon^{-2})}.
$$

This identifies the possible slow scale, not a guaranteed instability for every parameter or initial state. In particular, the first-order $\alpha$ [frequency](../../../../../../frequency.md) shift may detune the second-order resonance unless appropriately tuned; a second-order [amplitude](../../../../../../wave-amplitude.md) analysis would decide actual growth.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
