<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Introduce the slow time $T=\epsilon t$ and expand $y=y_0(t,T)+\epsilon y_1(t,T)+\cdots$. At leading order write

$$
y_0=R(T)\cos\psi,\qquad \psi=t+\varphi(T),\qquad R(0)=1,\quad\varphi(0)=0.
$$

The first-order equation is

$$
(\partial_t^2+1)y_1=-2\partial_t\partial_Ty_0-(\partial_ty_0)^n
=2R_T\sin\psi+2R\varphi_T\cos\psi-(-1)^nR^n\sin^n\psi.
$$

Its resonant sine and cosine components must vanish by the [solvability condition in the method of multiple scales](../../../../../../solvability-condition-in-the-method-of-multiple-scales.md). Let angle brackets denote a full-period average. The cosine projection of the nonlinear term is zero, since $\langle\sin^n\psi\cos\psi\rangle=0$. The sine projection gives

$$
\boxed{\varphi_T=0,\qquad R_T=(-1)^nR^n\langle\sin^{n+1}\psi\rangle}.
$$

This is the [averaged oscillator damping by a power of velocity](../../../../../../averaged-oscillator-damping-by-a-power-of-velocity.md).

If $n$ is odd, define

$$
C_n=\langle\sin^{n+1}\psi\rangle=\frac{1}{2^{n+1}}\binom{n+1}{(n+1)/2}>0.
$$

Then $R_T=-C_nR^n$, giving

$$
\boxed{y(t)=e^{-\epsilon t/2}\cos t+O(\epsilon)\quad(n=1)},
$$



$$
\boxed{y(t)=\left[1+(n-1)C_n\epsilon t\right]^{-1/(n-1)}\cos t+O(\epsilon)\quad(n>1\text{ odd})}.
$$

For every fixed $n$, these leading [multiple-scale expansions](../../../../../../method-of-multiple-scales.md) are uniform on bounded slow-time intervals $0\le\epsilon t\le T_0$. The unforced phase remains $t$ to this order. A bounded first-order correction supplies the small adjustment to the initial derivative and initial displacement; it does not change this leading result.

If $n$ is even, the average of the odd power $\sin^{n+1}\psi$ vanishes. Thus $R_T=0$ and

$$
\boxed{y(t)=\cos t+O(\epsilon)\quad(n\text{ even},\ t=O(\epsilon^{-1}))}.
$$

The first-order forcing has only a constant and even harmonics, so it produces no fundamental resonance. Its bounded particular solution can be supplemented by homogeneous sine and cosine terms to satisfy the initial conditions. There can be an $O(\epsilon^2)$ [frequency](../../../../../../frequency.md) correction, but its phase accumulation is only $O(\epsilon)$ on the present time scale. In contrast to the odd case, the even-power force is invariant under [velocity](../../../../../../velocity.md) reversal and the equation is reversible; calling it positive damping for both signs of [velocity](../../../../../../velocity.md) would be wrong. The [mechanical energy](../../../../../../mechanical-energy.md) identity makes the distinction clear:

$$
\frac{d}{dt}\frac{(y')^2+y^2}{2}=-\epsilon(y')^{n+1}.
$$

This is nonpositive for odd $n$ and changes sign for even $n$; its cycle average reproduces the [amplitude](../../../../../../wave-amplitude.md) equation above.

For large odd $n$, the central binomial coefficient gives

$$
C_n\sim\sqrt{\frac{2}{\pi n}},\qquad L_n=(n-1)C_n\sim\sqrt{\frac{2n}{\pi}},\qquad
R=\exp\left[-\frac{\log(1+L_n\epsilon t)}{n-1}\right].
$$

This form reveals several time regimes. For $L_n\epsilon t\ll1$, $R=1-C_n\epsilon t+\cdots$; at $t=O(1/(\epsilon\sqrt n))$, the [amplitude](../../../../../../wave-amplitude.md) change is only $O(1/n)$. For $L_n\epsilon t\gg1$ but $\log(L_n\epsilon t)\ll n$, the leading change is $R\simeq1-\log(L_n\epsilon t)/n$. In particular, at $t=O(1/\epsilon)$ it is only $O(\log n/n)$, despite the long elapsed time. High powers damp mainly near [velocity](../../../../../../velocity.md) maxima, and even a small [amplitude](../../../../../../wave-amplitude.md) reduction strongly suppresses subsequent damping.

An order-one [amplitude](../../../../../../wave-amplitude.md) reduction in the averaged law requires $\log(L_n\epsilon t)=O(n)$. Formally, $t=e^{(n-1)\sigma}/(\epsilon L_n)$ gives $R\sim e^{-\sigma}$, and for fixed odd $n>1$ its late envelope is an algebraic power $t^{-1/(n-1)}$. These exponential-in-$n$ time scales are predictions of extending the averaged law; the fixed-$n$, bounded-$\epsilon t$ multiple-scale error estimate alone does not establish uniform accuracy that far. A joint large-$n$, small-$\epsilon$ approximation also needs control of the increasingly sharp nonlinear peaks, rather than assuming fixed-$n$ error constants are uniform. Taking $n$ fixed first and then examining the large-$n$ envelope avoids that unsupported interchange of limits.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
