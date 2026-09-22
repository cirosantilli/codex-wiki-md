<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [oscillator coupled to slow damping feedback](../../../../../../oscillator-coupled-to-slow-damping-feedback.md), expand $y=Y(T)+\varepsilon y_1(t,T)+\cdots$, alongside the [method of multiple scales](../../../../../../method-of-multiple-scales.md) oscillator expansion. The leading equation $\partial_tY=0$ makes $Y$ independent of fast time. The oscillator force evaluated on $x_0=R\cos\theta$ is $2YR\sin\theta$. The [amplitude-phase equations](../../../../../../amplitude-phase-equations-for-a-weakly-perturbed-oscillator.md) therefore give

$$
R_T=-YR,\qquad \phi_T=0.
$$

The next equation for the damping variable is

$$
\partial_ty_1+Y_T=g(R\cos\theta).
$$

A bounded periodic $y_1$ exists only when the mean of its right side vanishes. Thus the full leading averaged system is

$$
\boxed{R_T=-YR,\qquad \phi_T=0,\qquad Y_T=\langle g(R\cos\theta)\rangle.}
$$

Set $R_0=\sqrt{x_*^2+v_*^2}$, $\phi_0=\operatorname{atan2}(-v_*,x_*)$, and $Y_0=y_*$. These specify the arbitrary leading initial conditions.

For $g(x)=x$, the phase average is zero. Consequently

$$
\boxed{Y(T)=Y_0,\qquad R(T)=R_0e^{-Y_0T},\qquad\phi(T)=\phi_0.}
$$

Thus $x(t)=R_0e^{-Y_0\varepsilon t}\cos(t+\phi_0)+O(\varepsilon)$ and $y(t)=Y_0+O(\varepsilon)$. Positive $Y_0$ damps the oscillator, negative $Y_0$ amplifies it, and zero $Y_0$ leaves the leading amplitude unchanged. The fast correction $y_1=R\sin\theta$ plus an initial-matching constant confirms that $y$ can oscillate slightly even though $Y$ is constant. For $R_0=0$, the exact solution is $x=0$, $y=y_*$.

For the logarithmic feedback, assume $R_0>0$. Its phase singularities are integrable, and the supplied integral gives

$$
\left\langle\frac12\log(R^2\cos^2\theta)\right\rangle=\log R-\log2=\log(R/2).
$$

Writing $L=\log(R/2)$ turns the nonlinear [amplitude-phase equations](../../../../../../amplitude-phase-equations-for-a-weakly-perturbed-oscillator.md) into the linear pair

$$
L_T=-Y,\qquad Y_T=L,
$$

so $L_{TT}+L=0$. With $L_0=\log(R_0/2)$,

$$
\boxed{\begin{aligned}
R(T)&=2\exp\!\left(L_0\cos T-Y_0\sin T\right),\\
Y(T)&=L_0\sin T+Y_0\cos T,\\
\phi(T)&=\phi_0.
\end{aligned}}
$$

The [first integral](../../../../../../first-integral.md) $L^2+Y^2=L_0^2+Y_0^2$ provides a direct check, and the amplitude remains positive on every finite [slow time](../../../../../../slow-time.md) interval. At the retained averaged order, the physical approximation is $x\simeq R(\varepsilon t)\cos(t+\phi_0)$, $y\simeq Y(\varepsilon t)$.

**The logarithmic case needs an interpretation at oscillator zeros.** The original right side is undefined at $x=0$, so a globally classical solution through each crossing, or a solution from $x_*=v_*=0$, cannot be asserted. At a transverse crossing, $\log|x|\sim\log|t-t_*|$ is locally integrable; $y$ can be interpreted as absolutely continuous, with its equation holding away from the crossings and almost everywhere. In that integrable interpretation the displayed averaged formulas apply formally for nonzero leading amplitude. The standard smooth-forcing averaging theorem cannot be invoked without addressing this singularity. The phrase arbitrary initial conditions must exclude the identically zero state for this logarithmic problem.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
