<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Apply the [method of multiple scales](../../../../../../method-of-multiple-scales.md) with independent fast time $t$ and [slow time](../../../../../../slow-time.md) $T=\varepsilon t$, and write $x=x_0(t,T)+\varepsilon x_1(t,T)+\cdots$. The chain rule gives $d/dt=\partial_t+\varepsilon\partial_T$. At leading order,

$$
(\partial_t^2+1)x_0=0,\qquad x_0=R(T)\cos\theta,\qquad \theta=t+\phi(T).
$$

At first order,

$$
(\partial_t^2+1)x_1=f(R\cos\theta,-R\sin\theta)+2R_T\sin\theta+2R\phi_T\cos\theta.
$$

A forcing component at the natural [frequency](../../../../../../frequency.md) produces a [secular term](../../../../../../secular-term.md) in $x_1$. Thus the [solvability condition in the method of multiple scales](../../../../../../solvability-condition-in-the-method-of-multiple-scales.md) is orthogonality to both $\sin\theta$ and $\cos\theta$. Define the fast-phase average, holding $R,\phi,T$ fixed, by

$$
\langle h\rangle=\frac1{2\pi}\int_0^{2\pi}h(\theta;R,T)\,d\theta.
$$

Since $\langle\sin^2\theta\rangle=\langle\cos^2\theta\rangle=1/2$ and $\langle\sin\theta\cos\theta\rangle=0$, the [amplitude-phase equations](../../../../../../amplitude-phase-equations-for-a-weakly-perturbed-oscillator.md) are

$$
\boxed{R_T=-\langle f\sin\theta\rangle,\qquad R\phi_T=-\langle f\cos\theta\rangle.}
$$

They are leading averaged equations, not exact equations for a purely sinusoidal solution of a general nonlinear oscillator.

For the cubic conservative force, $f=-R^3\cos^3\theta$, odd symmetry gives $\langle\cos^3\theta\sin\theta\rangle=0$, while $\langle\cos^4\theta\rangle=3/8$. Hence

$$
\boxed{R(T)=R_0,\qquad\phi(T)=\phi_0+\frac38R_0^2T.}
$$

If $x(0)=x_*$ and $x'(0)=v_*$, leading initial matching gives

$$
R_0=\sqrt{x_*^2+v_*^2},\qquad \phi_0=\operatorname{atan2}(-v_*,x_*),
$$

and therefore

$$
x(t)=R_0\cos\!\left(t+\phi_0+\frac38\varepsilon R_0^2t\right)+O(\varepsilon)
$$

on bounded [slow time](../../../../../../slow-time.md) intervals for fixed bounded initial data. The positive [frequency](../../../../../../frequency.md) shift agrees with the increased restoring force of $x''+x+\varepsilon x^3=0$. The zero initial state is the exact zero solution, with irrelevant phase. If a first waveform correction is desired, the remaining first-order forcing is $-R_0^3\cos3\theta/4$, so $x_1=R_0^3\cos3\theta/32$ plus a homogeneous correction chosen to match the initial data at the next order. This exhibits explicitly why the leading harmonic ansatz is approximate.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
