<h1 id="11/solution">Solution</h1>

↑ **Parent:** [11](../11.md)

For a [plane wave](../../../plane-wave.md), $\partial_t$ acts as $-i\omega$ and $\partial_x$ as $ik$. Substitution gives

$$
\omega^2(\omega-\omega_n)-c^2k^2(\omega-\omega_d)=0,
$$

so, for $\omega\ne\omega_d$, the [dispersion relation](../../../dispersion-relation-split.md) is

$$
\boxed{k^2=\frac{\omega^2(\omega-\omega_n)}{c^2(\omega-\omega_d)}.}
$$

Assume $\omega_n>\omega_d>0$ and real [angular frequency](../../../angular-frequency.md). The ratio is negative exactly on $\omega_d<\omega<\omega_n$, giving imaginary [wavenumbers](../../../wavenumber.md) and an [evanescent wave](../../../evanescent-wave.md). Thus **the propagating frequency gap is $(\omega_d,\omega_n)$**. At $\omega_d$ there is no finite-$k$ solution, while $\omega_n$ has $k=0$; neither endpoint is an ordinary finite-wavelength propagating mode.

Choose the branch $k=(\omega/c)\sqrt{(\omega-\omega_n)/(\omega-\omega_d)}$, so the [phase velocity](../../../phase-velocity.md) is positive in the allowed bands. Direct differentiation gives the [phase velocity](../../../phase-velocity.md) and [group velocity](../../../group-velocity.md)

$$
v_p=c\sqrt{\frac{\omega-\omega_d}{\omega-\omega_n}},\qquad
v_g=\frac{v_p}{1+\dfrac{\omega(\omega_n-\omega_d)}{2(\omega-\omega_n)(\omega-\omega_d)}}.
$$

The opposite spatial branch reverses both signs. On the chosen branch, the requested [limits](../../../limit-of-a-function.md) are

$$
\boxed{\begin{array}{c|cc}
\text{frequency limit}&v_p&v_g\\\hline
\omega\to0&c\sqrt{\omega_d/\omega_n}&c\sqrt{\omega_d/\omega_n}\\
|\omega|\to\infty&c&c\\
\omega\to\omega_n^+&+\infty&0^+\\
\omega\to\omega_d^-&0^+&0^+
\end{array}}
$$

The band-edge limits are taken from their propagating sides. More precisely, with $\epsilon=\omega-\omega_n\downarrow0$ and $\delta=\omega_d-\omega\downarrow0$,

$$
v_p\sim c\sqrt{\frac{\omega_n-\omega_d}{\epsilon}},\quad
v_g\sim\frac{2c}{\omega_n}\sqrt{(\omega_n-\omega_d)\epsilon};\qquad
v_p\sim c\sqrt{\frac\delta{\omega_n-\omega_d}},\quad
v_g\sim\frac{2c\delta^{3/2}}{\omega_d\sqrt{\omega_n-\omega_d}}.
$$

For the final case, set $K=k_0c>0$. Substitution of $T(t)e^{ik_0x}$ at $\omega_d=0$ gives $T^{(3)}+(3iK/2)T''+K^2T'=0$. Its [characteristic polynomial](../../../characteristic-polynomial.md) factors as $r(r+2iK)(r-iK/2)$, hence

$$
T=A+Be^{-2iKt}+Ce^{iKt/2}.
$$

The initial data give $A+B+C=1$, $-2B+C/2=0$ and $-4B-C/4=-5$. Thus $B=1$, $C=4$, $A=-4$, and

$$
\boxed{\phi(x,t)=e^{ik_0x}\left[-4+e^{-2ik_0ct}+4e^{ik_0ct/2}\right].}
$$

The time-independent contribution is essential: [static modes lost by cancelling frequency](../../../static-mode-lost-by-cancelling-frequency.md) would be missed if one divided the $\omega_d=0$ [dispersion relation](../../../dispersion-relation-split.md) by $\omega$ and retained only its two nonzero-frequency roots.

## ↑ Ancestors (11)

1. [11](../11.md)
2. [2018](../../2018-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
