<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Throughout this solution $c=1$ and $a>0$.

**Null [metric tensor](../../../../metric-tensor.md) and boost.** Inverting the coordinate definitions gives $t=(p+q)/2$, $x=(q-p)/2$, and hence

$$
\boxed{ds^2=dp\,dq,\qquad
(g_{AB})_{p,q}=\begin{pmatrix}0&1/2\\1/2&0\end{pmatrix}}.
$$

For a frame moving at speed $v$ along positive $x$, use $t'=\gamma(t-vx)$, $x'=\gamma(x-vt)$. Their difference and sum give

$$
\boxed{p'=\alpha p,\qquad q'=q/\alpha,\qquad
\alpha=\gamma(1+v)=\sqrt{\frac{1+v}{1-v}}}.
$$

The reciprocal [scale factors](../../../../scale-factor-cosmology.md) preserve $dp\,dq$. They are $e^{\pm\eta_v}$ in [rapidity](../../../../rapidity.md) notation.

**[acceleration](../../../../acceleration.md) invariants.** Proper-time normalization gives $\dot t^2-\dot x^2=1$, so $\dot p\dot q=1$. The [four-acceleration](../../../../four-acceleration.md) has squared norm $\ddot t^2-\ddot x^2=-a^2$; therefore

$$
\boxed{\dot p\dot q=1,\qquad\ddot p\ddot q=-a^2}.
$$

For future motion write $\dot p=e^{-\eta}$ and $\dot q=e^\eta$. Then the second equation is $-(\dot\eta)^2=-a^2$. [acceleration](../../../../acceleration.md) toward positive $x$ selects $\eta=\eta_0+a\tau$.

**[hyperbolic motion from an initial event and rapidity](../../../../hyperbolic-motion-from-an-initial-event-and-rapidity.md).** The stated initial event fixes $p(0)=-1/a$, $q(0)=1/a$, but not the initial [rapidity](../../../../rapidity.md) $\eta_0$. Integrating with positive signed [acceleration](../../../../acceleration.md) gives the general family

$$
p=-\frac1a+\frac{e^{-\eta_0}}a(1-e^{-a\tau}),\qquad
q=\frac1a+\frac{e^{\eta_0}}a(e^{a\tau}-1).
$$

The initial event alone does not fix the initial [velocity](../../../../velocity.md) or signed [acceleration](../../../../acceleration.md). The trajectory explicitly requested in the next paragraph selects the additional conditions $\eta_0=0$ and positive-$x$ [acceleration](../../../../acceleration.md). With that convention,

$$
\boxed{p(\tau)=-\frac1ae^{-a\tau},\qquad
q(\tau)=\frac1ae^{a\tau}},
$$

and consequently

$$
\boxed{t(\tau)=\frac1a\sinh a\tau,\qquad
x(\tau)=\frac1a\cosh a\tau}.
$$

With arbitrary $\eta_0$ the equivalent expressions are $t=[\sinh(\eta_0+a\tau)-\sinh\eta_0]/a$ and $x=1/a+[\cosh(\eta_0+a\tau)-\cosh\eta_0]/a$. Thus position data alone do not select the displayed special [hyperbola](../../../../hyperbola.md). The following calculations use that intended [hyperbola](../../../../hyperbola.md), which is also explicitly given by the paper.

**Diagram and horizon.** The selected [world line](../../../../world-line.md) is the right-hand branch $x^2-t^2=a^{-2}$. Its future asymptote $x=t$ is a reception horizon: rightmoving signals have constant $p=t-x$, whereas the observer has $p<0$ and approaches zero only as $\tau\to\infty$. Events with $p\geq0$ cannot send a future signal to this observer if the [acceleration](../../../../acceleration.md) continues indefinitely. This is an observer-dependent causal restriction in flat spacetime, not a [curvature singularity](../../../../curvature-singularity.md).

**[photon reception by a uniformly accelerated observer](../../../../photon-reception-by-a-uniformly-accelerated-observer.md).** A rightmoving [photon](../../../../photon.md) from the stationary source has [four-momentum](../../../../four-momentum.md) $P^\mu=h\nu_0(1,1)$. Contracting with the observer's [four-velocity](../../../../four-velocity.md) gives

$$
\boxed{\nu(\tau)=\nu_0(\dot t-\dot x)=\nu_0\dot p=\nu_0e^{-a\tau}}.
$$

The same result follows by differentiating its emission-time relation. A [photon](../../../../photon.md) emitted at $x=L$ and time $t_e$ has $p=t_e-L$, so intersection requires

$$
\boxed{t_e=L-\frac1ae^{-a\tau}<L}.
$$

Thus **$t_e=L$ is the supremum of receivable emission times**, reached only in the limit of infinite receiver [proper time](../../../../proper-time.md). A [photon](../../../../photon.md) emitted exactly then lies on the horizon and is never received at finite time; later [photons](../../../../photon.md) cannot catch the ship. Restoring dimensions gives the limiting emission time $L/c$ for this chosen origin and trajectory.

**[Rindler coordinates](../../../../rindler-coordinates.md).** Substitution of the selected trajectory into the [coordinate transformation](../../../../smooth-transition-map.md) gives

$$
\boxed{\xi(\tau)=\tau,\qquad\zeta(\tau)=0}.
$$

Differentiating the transformation also gives $ds^2=e^{2a\zeta}(d\xi^2-d\zeta^2)$. Curves of fixed $\zeta$ are hyperbolae, while curves of fixed $\xi$ are straight rays $t/x=\tanh(a\xi)$ within the right wedge. The coordinate $\xi$ is the selected ship's proper clock; at another fixed $\zeta$, [proper time](../../../../proper-time.md) obeys $d\tau_\zeta=e^{a\zeta}d\xi$. The spatial coordinate is logarithmic in $\rho=\sqrt{x^2-t^2}=e^{a\zeta}/a$, rather than being proper distance itself. Fixed-$\zeta$ observers have [proper acceleration](../../../../proper-acceleration.md) $a e^{-a\zeta}$.

<a id="3/image-original-accelerated-worldline-reception-horizon-and-stellar-photon-rays-with-a-separate-rindler-coordinate-grid"></a>
![](../../../../past-exam-of-the-relativity-course-of-the-university-of-cambridge/2013/paper-1-rindler-signals.png)

**[Figure 2](#3/image-original-accelerated-worldline-reception-horizon-and-stellar-photon-rays-with-a-separate-rindler-coordinate-grid). Original accelerated worldline, reception horizon and stellar photon rays, with a separate Rindler coordinate grid**.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
